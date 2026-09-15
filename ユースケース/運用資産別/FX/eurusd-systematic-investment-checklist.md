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

> 本ページは、Reflexivity上で実際に生成されたResearch出力を日本語で読みやすくしたものです。結論だけに要約せず、問い、データ、途中の判断、反証、制約、最終的な読みまで元のストーリーをできる限り保持しています。数値・市場環境は原Research実行時点のものです。

## 原Researchの出力イメージ

原資料の全ページを順番にまとめています。英語原文の表・チャート・数値を確認できます。

![EUR/USDの投資判断を体系的なチェックリストに落とし込む - Reflexivity Research原資料](../../../画像/ユースケース/reflexivity/RX-USECASE-0032/source-visuals.webp)

## Researchの狙い

原資料は「EUR/USDを調べて」と曖昧に依頼するのではなく、**PMが毎回確認したい論点をチェックリスト化し、同じ順番でResearchを更新する**例です。原資料のLast Updatedは **2025-08-28** です。

## I. Positioning

- CFTC EUR Futures Net: **-15,000 contracts (Net Short)**
- 1か月変化: **-2,000 contracts**
- Historical Percentile: 約**25th percentile**
- 原資料の読み: Speculative positioningはEUR弱気方向で、Shortが増加
- ECB/Fedによる明示的な為替介入・USD targetingは限定的と整理

## II. Economic Fundamentals

### PMI Spread

- EU Manufacturing PMI **46.0** vs US **48.5**。Spread -2.5でUSD優位
- EU Services PMI **51.5** vs US **54.0**。こちらもSpread -2.5

### Employment / Inflation

原資料は失業率、雇用、Core Inflationの差を比較し、単独の指標ではなく**米欧の相対的なMomentum**として評価しています。

## III. Interest-Rate Differential

- German 10Y Bund: **2.69%**
- US 10Y Treasury: **4.24%**
- US-DE Spread: **+1.54%**
- US Real Rate: **1.7%**
- EU Real Rate: **-1.0%**
- Real-rate Spread: **+2.7%**、原資料では強いUSD支援要因と評価

### Rate Differential Regression

- R-squared: **0.349**
- Beta: **-0.1125**
- Model Predicted EUR/USD: **1.1270**
- 当時のActualとのGap: **+0.0369**

原資料は、この差を「Rate Differentialモデル対比でEURが約3.7cent割高」と解釈しています。

## IV. Valuation / Terms of Trade

- EUR REERはTrading Partners対比で概ねFair Value
- Brent **$68.05**で、EURのEnergy Import Costには中立〜やや支援的と評価

## V. Risk Sentiment / Volatility

- EUR/USD 1M Implied Vol: **7.6%**、Historical約40th percentile
- VIX: **16.9**
- Goldとの30日相関: **+0.372**
- DXY: **98.13**
- EUR/USD vs DXY: **-0.916**

## VI. Central Bank Policy

原資料はFedをData-dependentかつ相対的にHawkish、ECBをよりAccommodation寄りと整理し、**Policy DivergenceをUSD支援要因**としています。

## VII. Technical

- EUR/USD Spot: **1.1639**
- 20D MA: **1.1632**
- 50D MA: **1.1655**
- Immediate Support: **1.1405**
- Major Resistance: **1.1806**

## VIII. Scenario Analysis

| Scenario | Target | 原資料のProbability | 主なCatalyst |
|---|---:|---:|---|
| EUR Bull | 1.1800〜1.1900 | 25% | ECB Hawkish、US recession、USD safe-haven低下等 |
| EUR Bear | 1.1200〜1.1300 | 60% | EU recession、Fed higher-for-longer、USD safe-haven |
| Base | 1.1400〜1.1600 | 15% | Policy divergenceによる緩やかなEUR安 |

## 原資料のSummary Assessment

原資料は当時のBiasを**Bearish EUR**、ConvictionをHigh、Time Horizonを3〜6か月と整理し、Rate Differential、US優位のEconomic Momentum、Regression上のEUR割高、Policy Divergence、Technical、Risk Sentimentを同じ方向の根拠として並べています。

原資料には具体的なPosition Size、Stop、Target、Trade Recommendationも含まれますが、これらは**2025-08-28時点のResearch出力の記録**であり、現在の投資助言ではありません。

## このユースケースで確認できること

このResearchは、最終結論だけでなく、**どの問いから始め、どのデータを組み合わせ、途中で何を支持・反証材料とし、どこにLimitationsを置いたか**まで含めて再利用できるResearch workflowとして掲載しています。

---

[← 運用資産別ユースケース](../README.md) · [ユースケース一覧](../../README.md)