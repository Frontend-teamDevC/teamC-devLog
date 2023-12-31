## 参加メンバー
[kano](https://github.com/SouthernMinami) <br>
[mish](https://github.com/daxchx) <br>
[morio](https://github.com/m0rio0818) <br>

## 技術スタック
* 使用言語 typescript
* 使用フレームワーク Pharse
* 使用する CI 導入はする
* Linterとコードフォーマッターの設定 eslint、prettier を使う。
* 使用する APIなし
* ライブラリなど　なし

## 作るゲーム
プロトタイプとして、BlackJackを作成する。<br>
BlackJackをメンバー全員で作成。
その後、ポーカー等のゲームモードを追加する。

## 機能要件
* easy, medium, hardの3つの難易度で、敵のCPUと対戦できること
* ルール、勝利条件、プレイヤー数が異なる複数のトランプゲームモードに対応すること
* 対応するゲームモード：ブラックジャック（2-7人）、ラミー（2-4人）、ウォー（2人）、スピード（2人）、ポーカー、テキサスホールデムポーカー（2-10人）
* 各プレイヤーがゲームに参加するために満たさなければならない最低入札要件があるゲーム。もしプレイヤーが最低入札額を満たすことができなければ、ゲームに負けることになります。：ブラックジャック、ポーカー、テキサスホールデム
点数制のゲームで、最も高い点数を獲得した人が勝者となるゲーム：ラミー、戦争、スピード
* ユーザーの手が有効かどうかをチェックするバリデーションがあること
* 各ゲームモードに、ユーザーがゲームのプレイ方法を学ぶことができる簡単なチュートリアルがあること
* 各ゲームモードに、ユーザーがゲームのルールを理解するためのチートシートメニューがあること
* Webアプリへのリンク、またはアプリの最新バージョンをダウンロードできるホームページを用意すること

## 非機能要件
* コードベースが、将来的にトランプゲームのモードを簡単に追加できるように拡張可能な状態になっていること
* アプリは、ユーザーにとってシンプルでわかりやすく感じられ、混乱や遅延なく効果的に使い始めることができること
* ソフトウェアが、クロスプラットフォームであること。ウェブアプリ（ブラウザ）としてアクセスできるほか、デスクトップアプリ（Windows、Linux、Mac）、モバイルアプリ（iOS、Android）としてダウンロードすることができること。
* インストールするデバイスやオペレーティングシステムの種類にかかわらず、ソフトウェアのインストールプロセスがシンプルで効率的であること。これにより、ソフトウェアはすべてのプラットフォームで簡単かつ迅速にインストールできるようになります。

* ユーザーがソフトウェアをダウンロードできるページには、常に最新のバージョンがダウンロード可能でなければならないこと。
* ソフトウェアのデザインとユーザーインターフェースが最新で視覚的に魅力的であること。


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
* コミットルール　git操作の練習も兼ね、自分のdevlogはブランチを切り、プルリク作成まで行う。

## チームでの決まり
わからないことがあったら、discordのチャットに投稿　→ 顔合わせで話したり返信したりする。

## タスク管理
Trello, github issueの連携を行う

## ミーティング日程
月曜、木曜 21時〜22時

## スケジュール
以下を目標に開発していく。
11/11 ~ 11/18
Phaser学習会、各種セットアップ、技術構成の確認、ワイヤーフレーム。

11/19 ~ 11/25
* blackjackのプロトタイプ(最低限の機能等の実装)のデザイン考慮なしで作成したい。
* Phaserを使って、トランプ等の配置を行なっていきたい。
* ワイヤーフレームのイメージ合わせ(11/22)
* 実装は以下の通りに行う。
    * クラス作成 =(MVCのMode作成)は以下が担当する。
        * Blackjack: Kano
        * War : mishi
        * Poker: Nakatani
    * クラスを作成する人は、ワイヤーフレーム、シーケンス図、クラス図の作成まで行う。
    * Viewはクラス（Model）を作った人以外の二人で作成していく。
* Splint2にクラス図、ワイヤーフレーム、シーケンス図の作成完了を目標にする。

11/26 ~ 12/2
* blackjackの未完成部分を完了させる。 <br>
機能的には、black jackで遊べるくらいまで作成したい。
* デザイン、図、色 ->　スタイリングに関して話し合って検討していく。

12/3 ~ 12/9
* black jack, warのphaeserの実装を行う。
* pokerのプロトタイプを完成させる。
* speedのシーケンス図等の作成を行う。

12/10 ~ 12/16
* black jack, war, speedのphaeserの実装を行う。
* speedのシーケンス図等の作成を行う。

12/17 ~ 12/23

## 進捗
11/11 ~ 11/18
* Phaserのチュートリアルを行った。(必要になったタイミングで再度、確認をする)
* Dockerのセットアップを行った。
* プロトタイプ作成のコーディング担当：現時点ではクラスごとに担当していく。
* クラス図、シーケンス図、ワイヤーフレームの作成担当は以下。
    * Blackjack: Kano
    * War : mish
    * Poker: Nakatani

11/19 ~ 11/25
* Black jackのシーケンス図、ワイヤーフレーム、クラス図の作成
* Blackjackのベースとなるコード(Model)の作成。
* Blackjack, Warの2つを先に作成する方針に変更。(Black Jack: kano, morio, War: mish)

11/26 ~ 12/2
* Blackjackで遊べるくらいまで作成した。
* warに関しても、簡易的なhtmlで遊べるようになっている.
* Pokerは現在、modelの作成中

12/3 ~ 12/9
* war, blackjackに関して、、プロトタイプの作成完了。
* pokerのモデル作成 ほぼ完成
* phaserのinput中。phaerに関して、詰まっており、そこからなかなか進まない状況。
* speedの設計にも着手中。

12/10 ~ 12/17
* blackjackは完成
* war phaserの導入もほとんど完了した
* pokerのプロトタイプの作成完了。現在,phaserの導入中。
* speedも実装中。

## 議事録
* [2023/11/12]("https://github.com/Frontend-teamDevC/teamC-devLog/blob/main/minutes/20231111-1112.md")
* [2023/11/13]("https://github.com/Frontend-teamDevC/teamC-devLog/blob/main/minutes/20231113.md")
* [2023/11/16]("https://github.com/Frontend-teamDevC/teamC-devLog/blob/main/minutes/20231116.md")
* [2023/11/19]("https://github.com/Frontend-teamDevC/teamC-devLog/blob/main/minutes/20231119.md")
* [2023/11/20]("https://github.com/Frontend-teamDevC/teamC-devLog/blob/main/minutes/20231120.md")
* [2023/11/22]("https://github.com/Frontend-teamDevC/teamC-devLog/blob/main/minutes/20231122.md")
* [2023/11/25(admin MTG)]("https://github.com/Frontend-teamDevC/teamC-devLog/blob/main/minutes/20231125_Admin.md")
* [2023/11/27]("https://github.com/Frontend-teamDevC/teamC-devLog/blob/main/minutes/20231127.md")
* [2023/12/03]("https://github.com/Frontend-teamDevC/teamC-devLog/blob/main/minutes/20231203.md")
* [2023/12/10(admin MTG)]("https://github.com/Frontend-teamDevC/teamC-devLog/blob/main/minutes/20231210_Admin.md")