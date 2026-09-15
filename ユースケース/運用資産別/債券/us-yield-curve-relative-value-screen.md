<!--
id: RX-USECASE-0030
type: use-case
language: ja
locale: ja
author: Reflexivity Research
published: 2026-09-15
status: published
translation_status: local-only
original_language: en
source_text_status: faithful_japanese_rendering_from_platform_research
publication_mode: faithful-source-preserving
-->

# 米国イールドカーブからスティープナー／フラットナー候補をスクリーニングする

**著者:** Reflexivity Research  
**主な運用資産:** 債券（米国金利）  
**想定利用者:** 債券PM、Rates PM、相対価値運用  
**分析タイプ:** イールドカーブ、相対価値、スクリーニング

> 本ページは、Reflexivity上で実際に生成されたResearch出力を日本語で読みやすくしたものです。結論だけに要約せず、問い、データ、途中の判断、反証、制約、最終的な読みまで元のストーリーをできる限り保持しています。数値・市場環境は原Research実行時点のものです。

## 原Researchの出力イメージ

原資料の全ページを順番にまとめています。英語原文の表・チャート・数値を確認できます。

![米国イールドカーブからスティープナー／フラットナー候補をスクリーニングする - Reflexivity Research原資料](../../../画像/ユースケース/reflexivity/RX-USECASE-0030/source-visuals.webp)

## この原資料の位置づけ

このPDFはResearch全体ではなく、**前の出力でStrategy色とロジックが一致していなかった点を訂正したフォローアップ**です。そのため、ここでは「完成済みの元Researchがすべて残っている」とは扱わず、提供された訂正表と判断ロジックをそのまま残します。

## 訂正版スクリーニング表

| ペア | Curve Spread | Annualized Spread | Historical Percentile | Roll Down | 判定 |
|---|---:|---:|---:|---:|---|
| 3y-2y | -9.7bp | -9.7bp | 9.6% | 23.6bp | 🟡 Neutral |
| 4y-3y | -0.9bp | -0.9bp | 15.2% | 8.8bp | 🟡 Neutral |
| 5y-4y | 3.3bp | 3.3bp | 28.7% | 4.2bp | 🔴 Steepen (Pay) |
| 7y-5y | 11.8bp | 5.9bp | 37.4% | 8.5bp | 🟡 Neutral |
| 8y-7y | 5.6bp | 5.6bp | 39.9% | -6.2bp | 🟡 Neutral |
| 12y-8y | 20.0bp | 5.0bp | 45.5% | 14.4bp | 🔵 Flatten (Receive) |
| 20y-12y | 20.3bp | 2.5bp | 51.9% | 0.2bp | 🟡 Neutral |
| 25y-20y | -0.7bp | -0.1bp | 21.9% | -21.0bp | 🔴 Steepen (Pay) |
| 30y-25y | -4.7bp | -0.9bp | 12.9% | -4.0bp | 🔴 Steepen (Pay) |

## なぜ3y-2yと4y-3yはNeutralなのか

元の誤りは、低いHistorical Percentileだけを見てSteepen候補の色を付けた一方、**Roll Downが大きく、保有コストが反対方向に効く**ことを表示に反映できていなかった点です。

訂正版では、3y-2yは9.6% percentileでもRoll Down 23.6bp、4y-3yは15.2% percentileでもRoll Down 8.8bpのため、シグナルが相殺されるとしてNeutralに修正されています。

## 訂正版の分布

- **Steepen (Pay): 3組** - 5y-4y、25y-20y、30y-25y
- **Flatten (Receive): 1組** - 12y-8y
- **Neutral: 5組** - 3y-2y、4y-3y、7y-5y、8y-7y、20y-12y

この例の価値は、単に「低percentileだからSteepen」とせず、**歴史的位置とCarry/Roll Downを同時に見て、魅力的に見えるTradeをNeutralへ落とす**ところにあります。

## このユースケースで確認できること

このResearchは、最終結論だけでなく、**どの問いから始め、どのデータを組み合わせ、途中で何を支持・反証材料とし、どこにLimitationsを置いたか**まで含めて再利用できるResearch workflowとして掲載しています。

---

[← 運用資産別ユースケース](../README.md) · [ユースケース一覧](../../README.md)