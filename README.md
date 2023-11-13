## 参加メンバー
[kano](https://github.com/SouthernMinami) <br>
[mish](https://github.com/daxchx) <br>
[morio](https://github.com/m0rio0818) <br>

## 技術スタック
* 使用言語　typescript
* 使用フレームワーク Pharse
* 使用する CI 導入はする
* Linter とコードフォーマッターの設定 eslint、prettier を使う。
* 使用する APIなし
* ライブラリなど　なし

## 作るゲーム
プロトタイプとして、blackjackを作成
BlackJackをメンバー全員で作成.
その後、ポーカー等のゲームモードを追加する。


## 機能要件

## 非機能要件

## deploy環境
フロントエンド　Vercelを使用 <br>
バックエンド チーム開発終了後に集まって、拡張機能の構築（ランキングシステム、オンライン対戦等）の実装を行う。その時に技術選定をする。

## ワイヤーフレーム
Figmaを使用

## 技術スタックの構成図

## クラス・アクティビティ図
メンバーみんな書く機会を設ける。

## 毎週末にその週行った作業をまとめて全チームと共有する
* logファイル名は以下で統一。
    yyyymmdd(月)-yyyymmdd(日).md
* 毎週末チームメンバーに報告するlogは、各自のフォルダを作成し、.mdファイルを作成、記録する。


## チームでの決まり
わからないことがあったら、discordのチャットに投稿　→ 顔合わせで話したり返信したりする。

## タスク管理
Trello, github issueの連携を行う

## ミーティング日程
月曜、木曜 21時〜22時

# 2023/11/12 チームCミーティング
2023/11/12 20:30(JST) <br>
記録: [morio](https://github.com/m0rio0818) <br>
参加者: [kano](https://github.com/SouthernMinami) [mish](https://github.com/daxchx)

* ToDo
    * 最初の一週間でPhaserのキャッチアップををする。
    * ワイヤーフレームはみんなそれぞれ一回作ってみる。

* 明日までにやること
    * Trelloとgituhub連携の調査
    * Linter とコードフォーマッターの設定 eslint、prettierの設定を調べる。
    * [Phaser](https://dev.classmethod.jp/articles/phaser-js-typescript-vite/), [TypeScrpit](https://qiita.com/uhyo/items/e2fdef2d3236b9bfe74a) のキャッチアップ
    * typescriptのバージョン統一するには、Docker必要か考える。

* 確認したいこと
    * logファイルを作成する際のブランチを切り方。 → 練習込みで自分のブランチを切って、コミットしていく。
    * また、練習込みで、開発リポジトリでdevelopブランチをdefaultにする。
    * おそらくTrelloのpowerupの機能を使えば、Github issueとtrelloの連携ができるのではないか。[URL](https://support.atlassian.com/ja/trello/docs/using-the-github-power-up/)<br>
 
# 2023/11/13 チームCミーティング
 → 練習込みで自分のブランチを切って、コミットしていく。
    * また、練習込みで、開発リポジトリでdevelopブランチをdefaultにする。

*　dockerの使用
　　　とりあえず、ローカルで環境構築を行なってみて、軽く動かしてみる。　今週日曜までに、いじってみていけそうだったら使用、無理そうだったら手動で合わせる。（morio, kano）

* phaserの進捗
  * 木曜日に、みんなでわからない箇所等話し合う（勉強会）

* eslint, pritter
  * kanoさんが、個人のblackjackでeslint, prittierの経験あり。
  * 初回、eslint、 prittierの設定を行えば、他の人にも反映される。[eslint設定方法](https://typescriptbook.jp/tutorials/eslint) (mish)
  * docker考慮なしで、dockerでいけそうだったら、dokcer上に設定にする。
    
* クラス図
  * 今週中に抽象クラス等を考慮したものを作成(kano)

* シーケンス図
  *　後付け
  
* Trelloをもう少し触ってみる。
* github issueテンプレ作成
    * bug, 新規機能で作成。

