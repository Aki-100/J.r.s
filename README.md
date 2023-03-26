<p align="center">
    <img src="logo.png" width="258px">
</p>

# &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Find Japanese regional sweets!

## 制作背景
現在、訪日外国人観光客は少ないが、コロナ禍以前は3188万人以上と非常に多かったので、今後再び増加していくと考えられる。この強い需要に対して、より楽しく充実した観光をしてほしいと思い、観光に欠かせないお土産（ご当地お菓子）に関するサービスを作りたいと思った。

お菓子を選んだ理由は、観光庁の訪日外国人の消費動向調査（2019年）から、観光・レジャー目的で訪日した際の、菓子類の購入率は73.45％で費目別で最も高かったからである。また、最も満足した購入商品は菓子類で、全体の21.5％だった。

加えて、外国人向けのサイトで、お土産としてのお菓子をランキング形式で紹介しているサイトは散見されるが、「ご当地お菓子」を紹介しているサイトはほぼなかったので制作しようと考えた。

## 概要
「Find Japanese regional sweets!(日本のご当地お菓子を見つけよう!)」

本アプリは以下に示すポイントに根差して設計されています。

・お菓子投稿機能<br>
・お菓子に対するコメント機能 <br>
・いいね機能 <br>
・いいね数に応じたランキング機能 <br>

「日本のお菓子で幸せに」をコンセプトとしています。

アプリへGo！⇒ https://find-japanese-sweets.herokuapp.com/

## 開発環境
### 使用言語：
PHP <br>
HTML <br>
CSS <br>

### 環境:
Laravel(ver.9) <br>
AWS(EC2＋Cloud9) <br>
MySQL(MariaDB) <br>
Github <br>

### デプロイ：
Heroku

## データ構成
### ER図：
<img src="ER diagram.png" width="500px">

### 各テーブル詳細:
<img src="users_table.png" width="500px">
<img src="sweets_table.png" width="500px">
<img src="likes_table.png" width="500px">
<img src="comments_table.png" width="500px">
<img src="prefectures_table.png" width="500px">
<img src="regions_table.png" width="500px">

## 機能
・CRUD <br>
・ログイン <br>
・画像アップロード＆表示（Cloudinary） <br>
・いいね <br>
・コメント <br>

## こだわり

### いいね数に応じたランキング機能：
それぞれのお菓子の投稿に対して各ユーザーが「いいね」をすることができ、Home画面には「いいね」が多い順に投稿が表示されます。
<img src="Home.png" width="500px">

### 地域・都道府県ごとのお菓子表示機能：
<img src="regions.png" width="500px">
<img src="prefectures.png" width="500px">
<img src="Hokkaido.png" width="500px">

## 利用方法
### お菓子を検索したいユーザー：
お菓子を検索したいユーザーは、ランキングが表示されたHomeページやSweetページ（お菓子の一覧ページ）上のお菓子の名前を選択することで、そのお菓子の簡単な説明と、お菓子に関する書き込みが全て見ることができるページにたどり着きます。また、特定の地域や都道府県に関連するお菓子を探したい場合は、ヘッダーの「Region」「Prefecture」にいき、そこでお菓子を探したい地域や都道府県を選択すると、各地域や都道府県に関連するお菓子の一覧が表示され、お菓子を探すことができます。なお、各お菓子記事内の地域名や都道府県を選択することによっても、同様のお菓子一覧ページが表示されます。

### 新しくおすすめのお菓子を投稿するユーザー：
新しくおすすめのお菓子を投稿するユーザーは，HomeページやSweetページ（お菓子の一覧ページ）の上部にある「register」からお菓子投稿を行うことができます。お菓子の投稿では、「お菓子の名前」「お菓子についての説明」「お菓子の画像」「地域」「都道府県」を記入、アップロードします。なお、画像はアップロードしなくても投稿できます。また、投稿を編集・削除することも可能です。

### 食べたお菓子についての感想等を共有したいユーザー：
食べたお菓子についての感想等を共有したいユーザーは、Commentページ（コメント一覧ページ）の上部にある「Let's Comment!」から「お菓子の名前」「お菓子の画像」「コメント内容」を記入・アップロードし、コメントを登録することができます。なお、画像はアップロードしなくても登録できます。また、コメントは削除することが可能です。

## 今後の計画
・
・地域や都道府県ごとのランキング機能


・同じお菓子名の登録制限機能
