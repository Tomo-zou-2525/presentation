---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://cover.sli.dev
# some information about your slides, markdown enabled
title: Welcome to Slidev
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
---

# DXの観点から見る
# HCPTerraform 

Presentation slides for developers

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
layout: image-left
image: image01.png
---

# 私について
- 名前：とも蔵
- 職業：インフラエンジニア
- 興味のある分野：IaC,CDN,Security
- 好きなAWSサービス：
  S3, CloudFront, GuardDuty
  <br>
  <br>
<div v-click>
<h1>◽️ 特技：鎖骨骨折</h1>
</div>
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
transition: fade-out
layout: two-cols
layoutClass: gap-16
---

# 本講座について

DXとTerraformの特徴・組み合わせについて説明します


-- DXについて -- 
- **DXの概要** - DXとは？
- **昨今のDXを取り巻く状況** - 国内企業の現状
- **DXとの向き合い方** - 個人レベルで出来ること

-- Terraformについて -- 
- **Terraformとは**
- **Terraformのメリット**
- **運用上の課題**
- **HCP Terraformについて**
<br>

DXについて(総務省) [Why DX?](https://www.soumu.go.jp/johotsusintokei/whitepaper/ja/r03/html/nd112210.html)
<br>
DX推進指標について(IPA版) [DX推進指標](https://www.ipa.go.jp/digital/dx-suishin/about.html)
<br>
DX推進指標について(経済産業省版) [DX推進指標](https://www.meti.go.jp/shingikai/mono_info_service/dgs5/pdf/004_s04_00.pdf)

::right::

<Toc v-click minDepth="1" maxDepth="2"></Toc>


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
---

# DXって？

<div v-click>
<h2>- DXとはなんですか？ -</h2>
</div>
<br>
<br>
<div v-click>
<h2>- 「業務ツールを導入すること」の違いは？<br> -> 業務効率化との違いは？ -</h2>
</div>
<br>
<br>
<br>
<div v-click>
<h1>- 明確な定義はないものの、共通した考え方はある -</h1>
</div>


---
transition: slide-left

---

# DXとは

<div v-click>
<h3>
- デジタル技術を活用し、ビジネスモデルやプロセスを根本から変革すること
<br>
- 顧客体験の向上、業務効率化、新たな価値創造を目指す
<br>
- 単なるIT化ではなく、組織文化や働き方改革も伴う
</h3>
</div>
<br>
<div v-click>
<h2>
-> ITの浸透が、人々の生活をあらゆる面でより良い方向に変化させること (ストルターマン, 2004)
</h2>
</div>

<br>
<div v-click>
<h1>
要するに<br>
ツール導入,新規ビジネスモデル構築 + 組織,文化改革
</h1>
</div>



---
transition: slide-left
---

# DXとAIの関係性

- DXの概念は分かったが、結局のところ、お偉いさんやビジネス層が取り組むことじゃないの？
  <br>
  そう思われることもあるでしょうか。

<br>
<div v-click>
<br>
<h2>
私は、明確な意思を持って

<br>
各個人がDXに取り組むべきと考えています。
</h2>
</div v-click>

<br>
<br>
<div v-click>
<h2>
皆さんは「AI」「AGI」「ASI」についてご存知でしょうか？
</h2>
</div v-click>




---
transition: slide-left
---

# AIの進化とAGI達成について

<br>
<br>
<div v-click>
<h2>
人間が金魚に置き換わる時代が来る
</h2>
</div v-click>
<br>
<br>
<br>
<div v-click>
<h1>
新しい価値を創出できるようになろう
</h1>
</div v-click>

---
transition: slide-left
---

# Terraformとは？

<div v-click>
<h2>
</h2>
</div v-click>

---
class: px-20
transition: slide-left
---

# Terraformのメリット
- コードデプロイ〜リソース変更まで
<div v-click>
<h2>
</h2>
</div v-click>

---
transition: slide-left
---

# Terraformの注意点

- 技術習得まできつい

- 自由に書ける分、ルール制約が必要

- tfstateやterraformバイナリファイルのバージョン管理が面倒

---
transition: slide-left
---

# HCP Terraformを使おう

- 様々な使い方
  - VCS Driven
  - CLI Driven
  - API Driven
- tfstateの管理
  - リモートで管理してくれるので、Backendの指定はなし


---
transition: slide-left
---

# DXとTerraformとは

- Terraformは確かに便利

- が、便利すぎるが故に、技術が閉じたり継承されにくいから
結果的に普及しない現状があると思う

- DXの観点を持ち、組織改善のマインドを持てば、便利なツールをみんなが使えるようになり
世の中がもう少しハッピーになるのではないか、というお話

- 皆さんにもそうなっていただけると嬉しい、というお話