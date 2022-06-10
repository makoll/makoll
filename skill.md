# Skill

直近5年で利用・採用した言語・フレームワーク・アーキテクチャ

## Backend

### REST API (JavaScript + TypeScript + Node.js)

- 開発時期: 2020 ~ 2021
- バージョン
  - TypeScript 3 ~ 4
  - Node.js 12 ~ 16
- ライブラリ・フレームワーク
  - Express
  - TypeORM
- インフラ (AWS)
  - ECS + Fargate + RDS (Aurora MySQL)
- アーキテクチャ
  - [こちら](https://blog.spacemarket.com/code/clean-architecture-node/)を参考に実装
  - ビジネスロジックを除いたベース部分は[このリポジトリ](https://github.com/makoll/api-sample)
- 技術選定: 自分
  - 選定理由: 会社にNode.jsエンジニアが多かったためほぼ必然的に決まった

### REST API (Python)

- 開発時期: 2017 ~ 2020
- バージョン
  - Python 3.6 ~ 3.8
- ライブラリ・フレームワーク
  - Flask
  - SQL Alchemy
- インフラ (AWS)
  - ECS + Fargate + RDS (Aurora MySQL) + Cognito
- アーキテクチャ
  `REST API (JavaScript + TypeScript + Node.js)`のPython版  
  TypeScriptのサンプルをPythonならどう読み替えるべきかを悩みながら実装
- 技術選定: 自分を含む数人のリードエンジニア
  - 選定理由: 新規プロダクト開発を高速開発開発するため

## Frontend

### SPA (SSG) (JavaScript + TypeScript + Node.js + Vue.js)

- 開発時期: 2021 ~
- バージョン
  - TypeScript 3 ~ 4
  - Node.js 12
- ライブラリ・フレームワーク
  - Vue.js + Nuxt.js + Vuex
    - Vue.js 2 + Composition API
- インフラ (AWS)
  - Amplify
- 技術選定: 他の人。Joinした時点ですでに実装されていた

### API Aggregation BFF (JavaScript + TypeScript + Apollo Server)

- 開発時期: 2021 ~
- バージョン
  - TypeScript 4
  - Node.js 14
- ライブラリ・フレームワーク
  - Apollo Server
    - apollo-server-lambda
  - Axios
- インフラ (AWS)
  - Lambda + API Gateway
- 技術選定: 自分
  - 選定理由: フルスタックフレームワークからSPA + API構成に  
  マイグレーションするプロジェクトのために採用
    - ドメインやサービスごとにBFFを作り、  
    最終的にApollo Federationで集約するため、Apollo Serverを採用した

### SPA (SSR) (JavaScript + TypeScript + Node.js + React)

- 開発時期: 2018 ~
- バージョン
  - TypeScript 3 ~ 4
  - Node.js 14 ~ 16
- ライブラリ・フレームワーク
  - React + Next.js + Redux
    - 2018 ~ 2021
- インフラ (AWS)
  - ECS + Fargate
- 技術選定: 自分、または自分を含む数人のリードエンジニア
  - 選定理由: Backend1,2に対するFrontendで、  
  SPA - API構成でメンテナンスしやすいフレームワークとしてReactを採用

## Batch

### Serverless (Lambda + Step Functions)

- 開発時期: 2017-2021
- バージョン
  - その当時使っていたバックエンドと同じ言語を利用
  - Python 3.6 ~ 3.8
  - TypeScript 3 ~ 4
  - Node.js 12 ~ 16
- インフラ (AWS)
  - Lambda + Step Functions
- 技術選定: 自分
  - 選定理由: 小規模なバッチをメンテナンス性を考えてServerless構成で構築するため

## Other

### Agile Framework (Scrum)

- 3社、4チームで利用
  - 最初の2チームでは他のメンバーと本を読みながら手探りで導入
  - 次のチームではスクラムマスター資格を持ったスクラムマスターと共に導入、実施
  - 現在のチームでは開発者と兼任のスクラムマスターという形でチームに導入

### Fault Detection

- Sentry: 利用時期: 2017-2021
- New Relic:  利用時期: 2017-2020
- Mackerel: 利用時期: 2021-

### Virtualization (Docker)

- ECSとの組み合わせで利用。軽量化や高速化はTry & Error
- ローカル環境構築にはDocker Composeと組み

### Version Control (Git)

- ヒストリーの操作や復元など、思った通りのツリーを作成可能

### IDE (VSDode)

- Vimプラグインを利用
- Live Shareでモブプロ
- チーム生産性のために.vscodeディレクトリの整備は必ず実施

### Other

その他詳細なライブラリ等の内容については[こちら](skill_summary.md)へ
