---
id: RX-USECASE-0037
title: "EUR/USDのRSI戦略をパラメータ別・アウトオブサンプルで検証する"
type: use-case
asset_class:
  - "FX"
roles:
  - "FX運用"
  - "クオンツ運用"
analysis_type:
  - "バックテスト"
  - "ウォークフォワード分析"
  - "ロバストネス検証"
language: ja
locale: ja
published: 2026-09-15
updated: 2026-09-15
status: published
original_language: en
source_text_status: interpreted_from_platform_research
---

# EUR/USDのRSI戦略をパラメータ別・アウトオブサンプルで検証する

**主な運用資産:** FX（EUR/USD）  
**想定利用者:** FX PM、クオンツ、システマティック運用  
**分析タイプ:** バックテスト、ウォークフォワード分析、ロバストネス検証

> 以下は特定時点のプラットフォーム出力をもとにした説明用の事例です。バックテスト結果は将来の運用成績を保証するものではありません。

## どのような業務に使えるか

テクニカル指標を使った戦略を評価する際、最も良いパラメータだけを選ぶと過剰適合しやすくなります。実務では複数パラメータを同じ条件で比較し、取引コストを含め、さらに学習期間とアウトオブサンプル期間を分けて結果が維持されるかを確認する必要があります。

この例ではEUR/USDのRSI平均回帰戦略について、複数のlookback、閾値、entry/exit ruleを組み合わせて検証し、1年目でのcalibrationと2年目のout-of-sample performanceを比較しています。

## Reflexivityでの進め方

1. 検証する戦略ルールとパラメータ・グリッドを定義します。
2. 利用可能な価格・RSI時系列を取得します。
3. look-aheadを避けた売買ルールを適用します。
4. スプレッド等の取引コストを差し引きます。
5. CAGR、Sharpe、Sortino、最大ドローダウン、turnover等を比較します。
6. calibration期間で良かった戦略がout-of-sampleでも維持されるかを確認します。

## 得られるアウトプットのイメージ

- 全パラメータ組み合わせのperformance table
- 戦略とbuy-and-holdのequity curve比較
- calibrationとout-of-sampleのSharpe比較
- 最大ドローダウン、turnover、time in market等のリスク指標
- 過剰適合の可能性が高いパラメータの識別

## この例のポイント

バックテストを「良い結果を出すため」に使うのではなく、**仮説がアウトオブサンプルでも残るかを検証するために使う**例です。元の分析では、calibrationで非常に良かった組み合わせのSharpeがout-of-sampleで大きく低下し、過剰適合のリスクが明確になりました。

また、要求された4時間足データが実際には取得できず日次データしか利用できなかったため、合成した4時間足を作らず、日次のみの結果として制約を明示しています。

## 注意点

元の分析は2年間の日次データという短いサンプルで、slippage、financing、詳細なposition sizing等は含みません。ライブ運用可能性の証明ではなく、戦略仮説の比較・反証・ロバストネス確認のワークフローとしてご参照ください。

---

[← FXユースケース](README.md) · [ユースケース一覧](../../README.md)

ご質問や詳細については **gtm@reflexivity.com** までお問い合わせください。
