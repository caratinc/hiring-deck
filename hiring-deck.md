---
marp: true
theme: gaia
paginate: true
backgroundColor: white
color: '#333333'
---

<style>
* {
  /* font-family: "Hiragino Maru Gothic ProN"; */
  font-family: YuGothic;
  letter-spacing: -0.01em;
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

## 株式会社Carat会社紹介資料

for Engineers

<span class="note">2022.01 updated</span>

<style scoped>
span.note {
  color: gray;
}
</style>

<!--
Also supports multiline.
We bet these comments would help your presentation...
-->

---

### Company

- 2016年12月にCEO松本・CTO斎藤によって創業
- 正社員は4名、業務委託の方を入れると10名ほど
  - うち、エンジニア・デザイナーはCTO含めて5名
- 本社は東京都渋谷区代々木にありますが、全員リモート勤務
- 詳しくはこちら↓<br>https://caratinc.notion.site/Carat-3fdf975a11c24bc98e5a0274c0c05b31

---

### About CTO

- 斎藤陽介( @saitoxu )
- 1989年生まれ東京在住
- 2014年京都大学大学院修了
- 新卒で株式会社SHIFTに入社し、<br>業務用Webアプリケーションの開発に従事
- 2016年12月にCEO松本と株式会社Caratを共同創業
- 2021年4月に京都大学大学院情報学研究科博士課程に入学

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

### Services

<img src="images/glit.webp" class="glit" />
<img src="images/glit_admin.webp" class="glit_admin" />

<span class="glit_caption">レコメンド型転職サービスGLIT(グリット)</span>
<span class="glit_admin_caption">AIを活用した<br>企業向け採用ソリューションGLIT Admin</span>

<style scoped>
img.glit {
  width: 500px;
  position: absolute;
  top: 200px;
  left: 100px;
}
img.glit_admin {
  width: 500px;
  position: absolute;
  top: 200px;
  right: 100px;
}
span.glit_caption {
  position: fixed;
  width: 500px;
  top: 480px;
  font-weight: bold;
  left: 100px;
}
span.glit_admin_caption {
  position: fixed;
  width: 500px;
  top: 480px;
  font-weight: bold;
  right: 100px;
}
</style>

---

### GLIT

<div style="width: 540px">

- https://glit.io
- 20以上の求人サイトの求人情報を掲載した転職サービス
- 求人情報のアグリゲーションとレコメンデーションが特徴
- iOS/Android/Webの3プラットフォームで展開

</div>

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

### GLIT Admin

<div style="width: 540px">

- https://lp.glit.io/enterprise
- 機械学習を活用した採用候補者のレコメンデーションが特徴

</div>

<img src="images/admin.webp" class="admin" />

<style scoped>
img.admin {
  width: 500px;
  position: absolute;
  bottom: 100px;
  right: 80px;
}
</style>

---

### Tech Stack & Tools

- GLIT
  - iOS/Android: React Native(TypeScript 90%), Firebase
  - Web: Next.js(TypeScript 100%)
- GLIT Admin
  - Web: Next.js(TypeScript 100%)
- API: Ruby on Rails
- 推薦API: FastAPI, Amazon SageMaker
- インフラ: AWS, GCP(BigQuery)

---

### Tech Stack & Tools

- ソースコード管理: GitHub
- チケット管理: JIRA
- ドキュメンテーション・仕様管理: Notion
- デザイン: Figma
- コミュニケーション: Slack, Zoom
- CI/CD: Bitrise, CircleCI
- モニタリング: Datadog, Sentry

---

### Architecture

<div style="width: 470px">

- 現在は2つのサービスで1つのAPIを共用するモノリスな構成です
- レコメンド機能はPrivate APIとして提供しています

</div>

<img src="images/architecture.png" class="arch" />

<style scoped>
img.arch {
  position: absolute;
  width: 700px;
  top: 180px;
  right: 40px
}
</style>

---

<!-- ### Team

<div style="width: 500px">

- 1チームですべてのサービスの開発・運営を行っています

</div>

<img src="images/team.png" class="team" />

<style scoped>
img.team {
  position: absolute;
  width: 600px;
  top: 150px;
  right: 30px
}
</style>

--- -->

### Development Flow

- PdMからチケットがアサインされます
- コードレビューはCTO + 同じ職種のエンジニアが実施しています
- ソフトウェアテスト会社出身のメンバーが多いのでQAが充実しています
- 週次のプロダクトミーティングでは今後のタスクに関するディスカッションや振り返りなどを行っています

<img src="images/flow.png" class="flow" />

<style scoped>
img.flow {
  width: 1000px;
  position: absolute;
  bottom: 36px;
  left: 134px;
}
</style>

---

### Ticket Examples

- フロントエンド
  - アプリストアへのレビュー機能追加
  - おすすめ画面から直接求人応募できるような導線追加
  - etc.
- バックエンド
  - 雇用形態で検索できるように求人検索APIを改修
  - 求人の重複判定バッチ開発
  - etc.

---

### Challenges

<span class="bold">1. 膨大な求人数の活用</span><br>パートナー企業から提供を受けている百万件近くの求人を、ニアリアルタイムでユーザーに提供する必要があります。単純に求人をストアするだけでなく、データの構造化や特徴量の抽出など数々のチャレンジがあります。

<span class="bold">2. 様々なパートナー企業とのシステム連携</span><br>今後更に連携パートナーを増やしていけるよう、システム連携の仕組み化・抽象化を念頭に置きつつアーキテクチャの設計や開発業務を推進する必要があります。

<style scoped>
span.bold {
  font-weight: bold;
  font-size: 1.1rem;
  line-height: 2rem;
}
</style>

---

### Selling Points

<span class="bold">1. 大きな裁量権</span><br>まだ小さなチームのため、大きな裁量権を持ってサービス開発に携わることができます。

<span class="bold">2. ビジネスサイドの開発への理解度</span><br>CEOやPdMのエンジニアリングへの理解度が高いです。ビジネスサイドとの意思疎通が難しいなどのストレスが少なく、価値創造に集中できる環境だと思います。

<style scoped>
span.bold {
  font-weight: bold;
  font-size: 1.1rem;
  line-height: 2rem;
}
</style>
