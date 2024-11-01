---
# try also 'default' to start simple
theme: apple-basic
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://cover.sli.dev
# some information about your slides, markdown enabled
title: DXビジネスゴール・戦略デザイン講座
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply any unocss classes to the current slide
class: text-center
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# https://sli.dev/guide/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/guide/syntax#mdc-syntax
mdc: true

layout: center

---

# DXビジネスゴール・戦略デザイン講座
<br>

## ガイド①：ケーススタディ〜VPC作成まで

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" alt="GitHub" title="Open in GitHub"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
transition: fade-out

layout: two-cols
---

# 概要説明

本講座の流れ、各種用語を解説します。

**①DXとは**<br> - DXの理解<br> - ビジネスモデルの理解

**②本講座について**<br> - 重要な概念<br> - 問題・課題・論点について<br> - 作成ツールの紹介

**③検証・ディスカッションの流れ**<br> - 1~2回目の内容<br> - 課題整理表作成の流れ<br> - VPC作成の流れ

::right::

<br>
<br>
<br>

**④ケーススタディ紹介**<br> - 事例の紹介(別資料参照のこと)<br>

**⑤ツール紹介**<br> -VPC<br> -CVCA <br> -GQM+Strategies

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/guide/syntax#embedded-styles
-->

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<!--
Here is another comment.
-->

---
transition: slide-up
level: 2
layout: center
---

## ①DXとは

- デジタル技術を活用し、ビジネスモデルやプロセスを根本から変革すること
- 顧客体験の向上、業務効率化、新たな価値創造を目指す
- 単なるIT化ではなく、組織文化や働き方改革も伴う

 -> ITの浸透が、人々の生活をあらゆる面でより良い方向に変化させること (ストルターマン, 2004)

 **-> ビジネス環境の激しい変化に対応し、
データとデジタル技術を活用して、顧客や社会のニーズを基に製品やサービス、ビジネスモデルを変革するとともに、
業務そのものや、組織・プロセス・企業文化・風土を変革し、競争上の優位性を確立すること**

---
transition: slide-up
level: 2
---

## ①DXとは：DXの理解
DXには大きく分けて2つの方向性が存在する

| **分野** | **実行例**                                         | **評価軸**                               |
|---|---|---|
| 既存事業の生産性向上 | 自動化、AI活用による業務効率化 | 計画達成に向けた「効率・実行内容」 |
|                       | データ分析による意思決定の最適化 |                                 |
|                       | クラウド移行による柔軟なシステム構築|                                 |
| 新規事業創出・<br>イノベーション創出 | MVP開発による迅速な検証               | 仮説検証による「学習量・学習内容」 |
|                       | デザイン思考による顧客視点の製品開発     |                                 |


---
layout: center
layoutClass: gap-16
---

## ①DXとは：DXの理解_続き

従来の業務効率化とDXは根本的に思想・対応が異なる

以下に従来企業との方針の違いを列挙する

| 方針                | 従来型効率化企業                                          | 収益力向上企業                                             |
|---------------------|------------------------------------------------------|------------------------------------------------------|
| DXの取り組み          | 個別部門から順番                                              | 全社対象にトップダウンで一斉に実施                                 |
| 従業員への働きかけ      | ビジョンや戦略を示す                                             | 判断の拠りどころとなる行動指針を示す                                 |
| 競争優位性の考え        | 製品・サービス中心                                              | 顧客志向で顧客行動をデータで可視化                                    |
| 競争優位性の考え(組織)  | 個人単位の強み                                                 | 組織や業務を横断して広範囲にデータ 共有と活用                            |

## **DXとは、部署や部門単位での業務効率化とは異なり、組織的に、明確な行動指針をもって、顧客体験に沿った改善活動を継続して行うことである** 

---
layout: center
---


## ①DXとは：ビジネスモデルの理解
<br>

**◽️モデルの定義**<br>
本来は複雑な事象に対して<br>ある側⾯に注⽬して整理し、可視化すること

**◽️ビジネスモデルの定義**<br>
複雑な事象の関係性を把握し、ビジネスの構造を可視化<br>顧客にとっての価値、価値提供の仕組みを整理すること

**◽️ビジネスモデルの必要性**<br>
複雑な事象に対し、手当たり次第に対応しないため<br>現状で判断できる最も効果的な仮説を構築・検証するために用いられる

---
level: 2
---

## ②本講座について

DXを推進するにあたり、より効果的なビジネスモデルを構築・検証を行う手法を理解する

また、参加者同士のディスカッションを通じて、様々なビジネスの可能性を探る

以下、本講座において重要な概念、事前知識を記載する

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    <Link to="8">DXに重要な概念<carbon:arrow-right class="inline"/></Link>
  </span>
</div>

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    <Link to="9">問題・課題(論点)について<carbon:arrow-right class="inline"/></Link>
  </span>
</div>

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    <Link to="11">ツールの紹介<carbon:arrow-right class="inline"/></Link>
  </span>
</div>

---

## ②本講座について:DXに重要な概念

<br>

## **1.** DXによって生み出される最大の価値は「顧客との共感」である。
<br>

## **2.** 新たな顧客への提供価値はエコシステムによって生み出される。
<br>

## **3.** エコシステムが成功するためには、顧客だけでなくビジネスに関係するステークホルダ全員がWinWinになる必要がある
<br>

## 学習してほしい内容
①ビジネス上の課題設定の考え方
<br>
②ステークホルダへの提供価値とステークホルダ間の価値連鎖のデザイン
<br>
③提供価値を中心としたビジネスのゴールと戦略のデザイン
<br>
④デザインした結果の評価方法（デザインの評価、及び戦略実行時の評価）

---
layout: image
image: image03.png
title: ②本講座について:問題・課題(論点)について
---

---
layout: image
image: image04.png
title: ②本講座について:問題・課題(論点)について
---

---
layout: image
image: image02.png
title: ②本講座について:作成ツールの紹介
---

---
layout: two-cols
---

## ③検証・ディスカッションの流れ
<br>

## 1回目の内容
- 講座説明・インプット
- ケーススタディ理解
- 課題整理表作成
- ディスカッション①
- VPCインプット
- VPC作成
- 成果発表
- ディスカッション②

::right::
<br>
<br>

## 2回目の内容
- 前回の振り返り
- 講座説明・インプット
- GQM+Strategies作成
- ディスカッション①
- プレゼンテーション資料作成
- 成果発表
- ディスカッション②


---
layout: image-right
image: image05.png
---

## ③検証・ディスカッションの流れ:課題整理表作成の流れ

1.ケーススタディの読み込み(別資料)

2.ケーススタディの分析

3.自社との比較

4.課題整理表の作成

5.フィードバックと改善

---
layout: image
image: image06.png
title: ③検証・ディスカッションの流れ:課題整理表作成サンプル
---


---
layout: image
image: image10.png
title: ③検証・ディスカッションの流れ:VPC作成の流れ①
---

---
layout: center
---

## ③検証・ディスカッションの流れ:VPC作成の流れ②

◽️顧客ニーズの分析
```
①Customer Job(s) - 顧客が解決したいこと
課題整理表でまとめた「課題」を参考にして、ステークホルダ(顧客)が解決したいこと・
成し得たいことを記述します。
複数の課題がある場合（多くの場合は複数出るでしょう）、同類の課題は１つにまとめ
顧客が本質的に解決したい課題となるよう意見を集約します。

②Gain, Pain – 顧客の利得, 痛み
a.で出した各Jobに対応するGainとPainを洗い出します。
このとき、1つのJobに対して1つ以上のGainとPainを考え、結び付けます。
```

以下のように考えてみると良いでしょう。
```
Gain … この課題を解決したら顧客はどんな状態になるか？

Pain … この課題を現状、解決できない理由(障壁)は何か？
```
---
layout: center
---

## ③検証・ディスカッションの流れ:VPC作成の流れ③

つぎに、顧客が積極的に受けいれそうな価値の仮説を考えます。
```
③ Gain Creators, Pain Relievers - 利得を作るもの, 痛みを取り除くもの

②で出したGain, Painのそれぞれに紐づくGain Creators, Pain Relieversを考えます。
Gain Creators, Pain Relieversは顧客への提供価値で考えます。（手段ではない！）
価値を考えるときは「～ができる」や「～な状態」で考えると良いでしょう。
これが、ソリューション提供者の達成目標になります。
```

さいごに、実現手段を考えます。
```
④Products & Services – 製品やサービス

③で考えたGain Creatorsを達成しPain Relieversを解決する手段を検討します。
Products & Servicesという名前ですが、機能で表現すると良いでしょう。
```
---
layout: center
---

## ③検証・ディスカッションの流れ:VPC作成の流れ_Tips

◽️アイディアを数多く出して最適なものを選ぶ
③④のアイディアはたくさんあるはずです。数多く出して最適なものを選ぶことが重要です。
（例えば、価格が高いというPainに対して、低価格にする以外にも付加価値を上げる策もあるは
ずです）

◽️時には前のステップを修正することも必要
③④を検討しているうちに①②の誤りや新しい事実を発見する場合があります。
試行錯誤が重要です。前のステップに戻ってブラッシュアップしてください。

◽️網羅性よりも顧客の課題を解決できるか
Customer Job(s)に対するGain, Painは必ずありますが、それ以降は紐づくものが見つけられな
いことも有ります。また、出したアイディアの全てを実現しようとすると難解なサービスになる
可能性があります。網羅性よりも顧客の課題を本当に解決できるかが重要です。

◽️自分たちだけでは実現できない事がらに気付く
VPCを記載している際に、ソリューション提供者だけでは実現できない課題・機能があることに
気付くと思います。課題・機能を実現するうえで必要な協力者もステークホルダとして追加し検
討をする必要があります。

---
layout: default
---

## ④ケーススタディ紹介(別資料参照)

---
layout: image
image: image07.png
title: ⑤ツール詳細:VPC
---

---
layout: image
image: image08.png
title: ⑤ツール詳細:CVCA
---

---
layout: image
image: image09.png
title: ⑤ツール詳細:GQM+Strategies
---