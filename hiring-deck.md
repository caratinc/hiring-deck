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

<span class="note">2021.06 updated</span>

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
- 正社員は4名、業務委託の方を入れると12名
  - うち、エンジニア・デザイナーはCTO含めて5名
- 本社は東京都渋谷区代々木にありますが、全員リモート勤務
- 詳しくはこちら↓<br>https://www.notion.so/Carat-3fdf975a11c24bc98e5a0274c0c05b31

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
- 2021年5月に大幅リニューアル

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
- レコメンデーション: Python
- インフラ: AWS, GCP(BigQuery)

---

### Tech Stack & Tools

- ソースコード管理: GitHub
- チケット管理: JIRA
- ドキュメンテーション・仕様管理: Confluence
- デザイン: Figma
- コミュニケーション: Slack, Zoom
- CI/CD: Bitrise, CircleCI
- モニタリング: Datadog, Sentry

---

### Architecture

<div style="width: 470px">

- 現在は2つのサービスで1つのAPIを共用しています
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

### Next Architecture

<div style="width: 370px">

- サービス毎に独立して開発を進められるよう、現在APIのリファクタリングを進めています

</div>

<img src="images/next_architecture.png" class="arch" />

<style scoped>
img.arch {
  position: absolute;
  width: 800px;
  top: 180px;
  right: 40px
}
</style>

---

### Team

<div style="width: 400px">

- 現在は1つのチームで2つのサービスの開発・運営を行っています

</div>

<img src="images/team.png" class="team" />

<style scoped>
img.team {
  position: absolute;
  width: 680px;
  top: 160px;
  right: 70px
}
</style>

---

### Future Team

<div style="width: 400px">

- 年内を目処にサービス毎にチームを分け、よりスピーディに開発を進められる体制にしたいと考えています

</div>

<img src="images/future_team.png" class="team" />

<style scoped>
img.team {
  position: absolute;
  width: 680px;
  top: 160px;
  right: 70px
}
</style>

---

### Development Flow

- 週次のプロダクトミーティングでアサインなどを決めます
- コードレビューはCTO + 同じ職種のエンジニアが実施しています
- ソフトウェアテスト会社出身のメンバーが多いのでQAが充実しています

<img src="images/flow.png" class="flow" />

<style scoped>
img.flow {
  width: 1100px;
  position: absolute;
  bottom: 120px;
  left: 84px;
}
</style>

---

### Selling Points

<span class="bold">1. 大きな裁量権</span><br>まだ小さなチームのため、大きな裁量権を持ってサービス開発に携わることができます。

<span class="bold">2. ビジネスサイドの開発への理解度</span><br>CEOやPdMのエンジニアリングへの理解度が高いです。ビジネスサイドとの意思疎通が難しいなどのストレスが少なく、働きやすい環境だと思います。

<style scoped>
span.bold {
  font-weight: bold;
  font-size: 1.1rem;
  line-height: 2rem;
}
</style>
