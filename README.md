# vue-vuetify-example
# 概要
Vuetify.jsを使用したサンプルアプリです。
いつの間にか、D&D５版アプリのプロジェクトになってしまいました。

# TODOs
## 全体
・呪文検索アプリなど、D&D５版アプリを別プロジェクト化する

## 機能単位
### 呪文検索アプリ
#### 優先高
* モバイル対応
> grid幅の調整、モバイル時にデータテーブルをやめてカード表示にするなど。  
> D&D Beyondのレイアウトを参考にしたい。  
> 呪文データのローカルストレージ保存対応（毎回ロードしなくても済むようにする）  
> 呪文データの初回ロードをドラッグドロップではなく、ファイル選択ダイアログを出すようにする。  
> 呪文表示をテーブルのexpandをやめてダイアログにする  
* 呪文表示をテーブルのexpandをやめてダイアログにする（非モバイルでも）
* 追加・編集ボタンがうざいので隠す。もしくは別画面にわける
* 一覧表示時のレイアウト変更
>詠唱時間の表示が長いと見切れるので、短縮表示可能に
>クラス表示が横に長いと見切れるので工夫したい。表示対象外とするほうが良いかもしれない。  
>「集中」の表記を「持続時間」と合わせて、以下のような表示で見せたい  
>「精神集中、最大１分まで」  
>呪文の種類（占術、召喚術など）を表示したい
* 検索条件について、詳細検索ができるようにしたい
* 全文テキスト検索ができるとうれしい
* レベル順のデフォルトソートはいまいち（CANTRIPのつぎに9-levelになる）のでできれば直したい
* コンポーネントがでかくなったので、ダイアログと別ファイルに分けたい

#### 優先低
* 呪文名のソートがなんかおかしいのでできればなおしたい。デフォルトのデータテーブルでは使えないのでいまいちなんだが・・
* 画面の色やGIFを変えてもうちょっといい感じにする

### イニシアチブアプリ
#### 優先低
* ニーズないからけすか？それかさぼりっこさんがいいって言ってたやつの仕様を見てパクるか。

### 能力値編集
#### 優先低
* 見た目がいまいちすぎるので何とかしたい

### 運用TODO
* URL変えたい。URLがgithubpages-testはいまいちすぎる。安いし、遊びでドメイン取る？
* アフェリエイトを張りたい。
* 宣伝したい。
>日本語呪文データをどうするか。公開したほうがアクセス数は増えるが、まずかろうという感じ。相談先はあるか？  
>SRD範囲内でも翻訳データを用意したら需要は増えそうだが、それ自体グレー。  

## 新機能TODO
* キャラクター単位の呪文書作成機能
>サーバーサイドが必要になるのでどうしようか？ローカルストレージでもいいが。。。  
* キャラクター・ビルダー
>いきなりつらいので、キャラクター単位の呪文書作成機能を作ってから、流用を考える。  

## 技術検証・学習観点
* せっかくなのでvuexには触れておきたい。
* サーバーサイドをもし組むなら、kotlinを試してみたい。理想はkotlin+SpringBoot。もしくはfirebard。
* 開発ノウハウをブログにまとめたい。

==================

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# run unit tests
npm run unit

# run e2e tests
npm run e2e

# run all tests
npm test
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

