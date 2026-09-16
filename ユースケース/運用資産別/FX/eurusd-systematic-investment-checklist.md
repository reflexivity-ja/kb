<!--
id: RX-USECASE-0032
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

# EUR/USDの投資判断を体系的なチェックリストに落とし込む

**著者:** Reflexivity Research  
**主な運用資産:** FX（EUR/USD）  
**想定利用者:** FX PM、マクロPM、マルチアセット運用者  
**分析タイプ:** マクロ分析、投資判断、シナリオ分析
> 本ページは、Reflexivity上で実際に生成された調査結果を日本語で読みやすくしたものです。結論だけに要約せず、問い、データ、途中の判断、反証、前提・留意点、最終的な読みまで元のストーリーをできる限り保持しています。数値・市場環境は元の調査を実行した時点のものです。

## 調査の狙い

原資料は「EUR/USDを調べて」と曖昧に依頼するのではなく、**PMが毎回確認したい論点をチェックリスト化し、同じ順番で調査を更新する**例です。原資料のLast Updatedは **2025-08-28** です。

為替の方向感は、ひとつの指標だけで決めると判断が偏りやすくなります。このチェックリストでは、まず市場参加者の偏りをポジショニングで確認し、次に景気・インフレの相対差、金利差、バリュエーション、リスクセンチメント、中央銀行、テクニカルへ進みます。最後に、それまでの材料が同じ方向を示しているか、どの条件で見方が変わるかをシナリオとして整理します。

この順番にすることで、**市場がすでにどちらに傾いているか → ファンダメンタルズがそれを支持するか → 金利・政策が価格差を説明するか → バリュエーションやテクニカルが反証しないか → どのシナリオで判断を変えるか**を一貫して確認できます。

## I. ポジショニング

最初にポジショニングを見るのは、同じ材料でも市場がすでに大きく傾いている場合と、まだ織り込まれていない場合で価格反応が変わるためです。

- CFTC EUR Futures Net: **-15,000 contracts (Net Short)**
- 1か月変化: **-2,000 contracts**
- Historical Percentile: 約**25th percentile**
- 原資料の読み: Speculative positioningはEUR弱気方向で、Shortが増加
- ECB/Fedによる明示的な為替介入・USD targetingは限定的と整理

## II. 経済ファンダメンタルズ

ポジショニングの偏りを確認したら、その方向に実体経済の相対差があるかを見ます。市場の持ち高だけでは持続性を判断できないためです。

### PMI格差

- EU Manufacturing PMI **46.0** vs US **48.5**。Spread -2.5でUSD優位
- EU Services PMI **51.5** vs US **54.0**。こちらもSpread -2.5

### 雇用とインフレ

原資料は失業率、雇用、Core Inflationの差を比較し、単独の指標ではなく**米欧の相対的なMomentum**として評価しています。

## III. 金利差

景気・インフレの相対差が見えたら、その差が金融政策と金利にどう反映されているかを確認します。為替では相対的な金利差が保有コストや資金フローを通じて価格に直接つながりやすいためです。

- German 10Y Bund: **2.69%**
- US 10Y Treasury: **4.24%**
- US-DE Spread: **+1.54%**
- US Real Rate: **1.7%**
- EU Real Rate: **-1.0%**
- Real-rate Spread: **+2.7%**、原資料では強いUSD支援要因と評価

### 金利差回帰

- R-squared: **0.349**
- Beta: **-0.1125**
- Model Predicted EUR/USD: **1.1270**
- 当時のActualとのGap: **+0.0369**

原資料は、この差を「Rate Differentialモデル対比でEURが約3.7cent割高」と解釈しています。

## IV. バリュエーションと交易条件

金利差だけで説明すると、短期の政策差を長期的な適正価値と混同する可能性があります。そこでREERやエネルギー輸入条件を見て、現在の価格水準が構造的に割高・割安なのかを別軸で確認します。

- EUR REERはTrading Partners対比で概ねFair Value
- Brent **$68.05**で、EURのEnergy Import Costには中立〜やや支援的と評価

## V. リスクセンチメントとボラティリティ

次に、マクロ・金利差で説明できる方向がリスクオン／オフやドル全体の動きでも整合しているかを確認します。

- EUR/USD 1M Implied Vol: **7.6%**、Historical約40th percentile
- VIX: **16.9**
- Goldとの30日相関: **+0.372**
- DXY: **98.13**
- EUR/USD vs DXY: **-0.916**

## VI. 中央銀行政策

原資料はFedをData-dependentかつ相対的にHawkish、ECBをよりAccommodation寄りと整理し、**Policy DivergenceをUSD支援要因**としています。

ここでは、これまで確認した景気・金利差が一時的な市場ノイズなのか、中央銀行の政策方向と整合した持続要因なのかを確認します。

## VII. テクニカル分析

最後に価格そのものを見て、ファンダメンタルズの方向と足元のトレンド・サポート／レジスタンスが一致しているかを確認します。ファンダメンタルズが正しくても、エントリー水準や短期の逆行余地は別問題だからです。

- EUR/USD Spot: **1.1639**
- 20D MA: **1.1632**
- 50D MA: **1.1655**
- Immediate Support: **1.1405**
- Major Resistance: **1.1806**

## VIII. シナリオ分析

ここまでの材料をひとつの方向予想に固定せず、どの前提が変われば見方を修正するかをシナリオに落とします。

| Scenario | Target | 原資料のProbability | 主なCatalyst |
|---|---:|---:|---|
| EUR Bull | 1.1800〜1.1900 | 25% | ECB Hawkish、US recession、USD safe-haven低下等 |
| EUR Bear | 1.1200〜1.1300 | 60% | EU recession、Fed higher-for-longer、USD safe-haven |
| Base | 1.1400〜1.1600 | 15% | Policy divergenceによる緩やかなEUR安 |

## 元資料の総合評価

原資料は当時の方向感を**Bearish EUR**、確信度をHigh、想定期間を3〜6か月と整理し、Rate Differential、US優位のEconomic Momentum、Regression上のEUR割高、Policy Divergence、Technical、Risk Sentimentを同じ方向の根拠として並べています。

原資料には具体的なPosition Size、Stop、Target、Trade Recommendationも含まれますが、これらは**2025-08-28時点のResearch出力の記録**であり、現在の投資助言ではありません。

## 運用上の読み方

このチェックリストの価値は、毎回同じ結論を出すことではありません。同じ順番で更新することで、「前回から何が変わったか」「どの根拠だけが崩れたか」「シナリオ確率を変えるべきか」を比較しやすくすることにあります。

## このユースケースで確認できること

この調査は、最終結論だけでなく、**どの問いから始め、どのデータを組み合わせ、途中で何を支持・反証材料とし、どの前提・留意点を明示したか**まで含めて再利用できる調査プロセスとして掲載しています。

---

[← 運用資産別ユースケース](../README.md) · [ユースケース一覧](../../README.md)
