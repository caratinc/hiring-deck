---
marp: true
theme: gaia
header: 株式会社Carat 会社紹介資料 エンジニア向け
footer: "更新日 2021年3月11日"
paginate: true
backgroundColor: white
color: '#333333'
---

<style>
* {
  font-family: "Hiragino Kaku Gothic ProN";
  /* font-family: "Hiragino Maru Gothic ProN"; */
  /* font-family: YuGothic; */
  letter-spacing: -0.02em;
}
</style>

<style scoped>
h2 {
  margin-top: 200px;
  text-align: center;
}
p {
  text-align: center;
}
</style>

## 株式会社Carat 会社紹介資料

エンジニア向け

<!--
Also supports multiline.
We bet these comments would help your presentation...
-->

---

### 目次

1. 会社概要
1. CTO紹介
1. 提供しているサービス
1. 技術スタックと開発ツール
1. アーキテクチャ
1. チーム
1. 開発フロー
1. 課題
1. 価値観
1. セールスポイント

<style scoped>
li {
  font-size: 30px;
}
</style>

---

### 会社概要

* 2016年12月にCEO松本・CTO斎藤によって創業
* 正社員は4名、業務委託の方を入れると10名ほど
  * うち、エンジニア・デザイナーはCTO含めて3名
* 本社は東京都渋谷区代々木にありますが、全員リモート勤務
* 詳しくはこちら → https://www.notion.so/Carat-3fdf975a11c24bc98e5a0274c0c05b31

#### →コロナ禍で体制を縮小しましたが、安定したビジネス基盤ができつつあるので改めて採用強化中

---

### CTO紹介

* 斎藤陽介( @saitoxu )
* 1989年生まれ東京在住
* 2014年京都大学大学院修了
* 新卒で株式会社SHIFTに入社し、<br>業務用Webアプリケーションの開発に従事
* 2016年12月にCEO松本と株式会社Caratを共同創業
* 2021年4月から京都大学大学院情報学研究科博士課程に進学予定

<img src="images/profile.jpg" class="profile" />

<style scoped>
img.profile {
  width: 300px;
  position: absolute;
  top: 100px;
  right: 80px;
  border-radius: 150px;
}
</style>

---

### 提供しているサービス

* GLIT(グリット) https://glit.io
* 20以上の求人サイトの求人情報を<br>掲載した転職サービス
* 求人情報のアグリゲーション<br>→ レコメンデーションが特徴
* iOS/Android/Webの<br>3プラットフォームで展開

<img src="images/glit1.jpg" class="glit1" />
<img src="images/glit2.jpg" class="glit2" />

<style scoped>
img.glit1 {
  width: 240px;
  position: absolute;
  bottom: 70px;
  right: 350px;
}
img.glit2 {
  width: 240px;
  position: absolute;
  bottom: 70px;
  right: 80px;
}
</style>

---

### 提供しているサービス

* MAUは堅調に伸長中

<img src="images/mau.png" class="mau" />

<style scoped>
img.mau {
  position: absolute;
  width: 1060px;
  bottom: 50px;
  right: 110px;
}
</style>

---

### 提供しているサービス

* GLIT Admin https://glit.io/enterprise
* 企業/エージェント向けの採用サービス
* 採用候補者のレコメンデーション<br>が特徴

<img src="images/admin.png" class="admin" />

<style scoped>
img.admin {
  position: absolute;
  bottom: 80px;
  right: 60px;
}
</style>

---

### 技術スタックと開発ツール

* GLIT
  * iOS/Android: React Native(TypeScript約90%), Firebase
  * Web: Next.js(TypeScript 100%)
* GLIT Admin
  * Web: React(TypeScript約40%)
* API: Ruby on Rails
* インフラ: AWS, GCP(BigQuery)

---

### 技術スタックと開発ツール

* ソースコード管理: GitHub
* チケット管理: JIRA
* ドキュメンテーション・仕様管理: Confluence
* デザイン: Figma
* コミュニケーション: Slack, Zoom
* CI/CD: Bitrise, CircleCI
* 監視: Datadog

---

### アーキテクチャ

<img src="images/architecture.png" class="arch" />

<style scoped>
img.arch {
  position: absolute;
  width: 780px;
  bottom: 20px;
  left: 240px
}
</style>

---

### チーム

* 主にプロダクト開発に関わっているのはCEO, CTO, PdM(COO), エンジニア2名(業務委託)
* エンジニアの方は1人はデザイナー兼フロントエンドエンジニア、もう1人はフロントエンド専任
* 現在はフロントエンドは業務委託の方々に、CTOがバックエンドなどその他全般を担当しています

---

### 開発フロー

* 週次のプロダクトミーティングでアサインなどを決めます(現在は毎週金曜)
* コードレビューはCTOが担当しています
* ソフトウェアテスト会社出身が多いのでQAは比較的厚めです

<img src="images/flow.png" class="flow" />

<style scoped>
img.flow {
  width: 1180px;
  position: absolute;
  bottom: 120px;
  left: 47px;
}
</style>

---

### 課題

* 2021年4月でGLITはサービスインして5年目に入るため、少しずつ負債も目立つようになってきました
* 特にAPIはモノリシックなRuby on Railsアプリケーションとして開発されているため、何かしら方針を立てリファクタリングを進め、次の5年に耐えうるようなアーキテクチャにしたいと考えています

---

### 価値観

<span class="bold">1. 最小人数で最大限の価値を</span><br>ソフトウェアアーキテクチャの目的は求められるシステムを構築・保守するために必要な人材を最小限に抑えることである - Clean Architecture

<span class="bold">2. 職人のこだわりと現実のバランス</span><br>QCDを守りつつも、1ピクセルのこだわりやメソッド・変数の命名などをないがしろにせずにしたいと思っています。

<style scoped>
span.bold {
  font-weight: bold;
  font-size: 1.1rem;
  line-height: 2rem;
}
</style>

---

### セールスポイント

<span class="bold">1. 大きな裁量権</span><br>まだ小さなチームのため、大きな裁量権を持ってサービス開発に携わることができます。

<span class="bold">2. ビジネスサイドの開発への理解度</span><br>CEOやPdMのエンジニアリングへの理解度が高いです。ビジネスサイドとの意思疎通が難しいなどのストレスが少なく、働きやすい環境だと思います。

<style scoped>
span.bold {
  font-weight: bold;
  font-size: 1.1rem;
  line-height: 2rem;
}
</style>
