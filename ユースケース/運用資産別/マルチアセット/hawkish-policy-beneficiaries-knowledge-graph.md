<!--
id: RX-USECASE-0034
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
# 金融政策のタカ派転換から恩恵を受ける資産・業種・企業をたどる
**著者:** Reflexivity Research  
**主な運用資産:** 株式、債券、FX、クロスアセット  
**想定利用者:** マクロPM、マルチアセットPM、株式PM  
**分析タイプ:** Knowledge Graph、テーマ分析、投資ユニバース構築
> 本ページは、Reflexivity上で実際に生成されたResearch出力を日本語で読みやすくしたものです。結論だけに要約せず、問い、データ、途中の判断、反証、前提・留意点、最終的な読みまで元のストーリーをできる限り保持しています。数値・市場環境は原Research実行時点のものです。
## 調査の問い
Hawkishな金融政策転換を「金利が上がる」で終わらせず、**1st orderのMacro Channel → 2nd orderのSector → 3rd orderのNamed Company**までKnowledge Graphで落としていく例です。
## 一次効果: マクロの伝達経路
原資料はBeneficiaryを生む主要な伝達経路を3つに整理しています。
1. **Higher-for-longer yields**
2. **Energy / inflation**
3. **Geopolitical spend**
## 二次効果: セクター
- Higher-for-longer → 銀行・Diversified Financials、保険、Asset / Money Managers
- Energy / Inflation → Energy Producers
- Geopolitical Spend → Aerospace & Defense
特に金利Channelは、銀行のNIM、保険会社のFloat再投資利回り、Money Fund / Cash Yield等を通じて最も広いBeneficiary群へつながるという読みです。
政策ショックからテーマ、セクター、企業へとつながる経路は、ナレッジグラフ上では次のように可視化されます。
![ナレッジグラフによる波及経路](../../../画像/ユースケース/reflexivity/RX-USECASE-0034/chart-1.webp)
*タカ派的な政策ショックが、テーマやセクターを経由して企業へ波及する経路。*
## 三次効果: 企業
原資料で上位KG Constituentとして挙げられた例:
- Financials: **CBOE、SCHW、Morgan Stanley**
- Insurers: **Chubb、Progressive、Swiss Re**
- Asset Managers: **BlackRock、Franklin Resources、Invesco**
- Energy: **ConocoPhillips、SLB、Saudi Arabian Oil**
- Defense: **Lockheed Martin、Northrop Grumman、RTX**
原資料にはさらにConsumer Lending、Sustainable Utilities、Commercial Real Estate、Homebuilding、Automakers、Credit & Lending等、多数のKG候補が表示されています。
## サンキー図の読み方
Link Widthは実際のCash FlowやEarnings Sensitivityではありません。
- Root → Channel: そのChannelが何Sectorへ波及するか
- Sector → Company: Knowledge GraphのExposure Rank
という**説明用Proxy**です。
## 分析上の留意点
- 1st / 2nd / 3rd orderという階層はAnalyst側のFrameであり、KG自体が「一次効果」を保証しているわけではない
- KG Linkは企業の利益感応度を直接測定しない
- Higher-for-longerは金融機関のMarginに追い風でも、同時にCredit Qualityや需要悪化リスクを伴う
- Constituentごとの実際の感応度は異なる
つまりこのResearchは、Macro Viewから**「次に読むべき会社のUniverse」**を作り、その後Fundamental Researchへ渡すための探索です。
## このユースケースで確認できること
このResearchは、最終結論だけでなく、**どの問いから始め、どのデータを組み合わせ、途中で何を支持・反証材料とし、どの前提・留意点を明示したか**まで含めて再利用できる調査プロセスとして掲載しています。
---
[← 運用資産別ユースケース](../README.md) · [ユースケース一覧](../../README.md)
