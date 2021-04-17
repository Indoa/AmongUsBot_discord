# AmongUsBot_discord

## 内容
- このプログラムはAmongUsをdiscordで行う際に、ミュート・解除、部屋の移動を半自動で行ってくれるbot
  - Herokuで実装しなくても、環境をPCで再現できれば誰かのPCでプログラムを実行すると使用できる 
  - 実装のチェックはローカル環境のデバッグで確かめる必要あり

## 基本操作
このプログラムは2つのテキスト「.start」・「.end」と、5つのリアクション「探索状態」・「会議中」・「スタートボタン」・「幽霊」・「生存者」を使用する。
  (リアクションは各々が作成し、リアクションのIDを取得する必要がある。)

1. 所定のテキストチャンネルに「.stert」を入力すると、botが起動し、専用のメッセージが発せられる。（同時にミーティング部屋に参加者が集められる）
   - 発せられたテキストに 設定したリアクション「生存者」・「スタートボタン」が付属する。（botがリアクションをつけている） 
   - 「生存者」リアクションに参加者はリアクションをつける（「生存者」のリアクションをクリックする）
     - 「生存者」のリアクションをつけるとロールに生存者が追加される
   - 全員がリアクションをつけると「スタートボタン」のリアクションを誰かがクリックする。（全員が生存者になっていないと開始しない）
  



## 以下はHerokuでdiscord.pyを実行するための手順
（サンプルのReadmeを引用）
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

- Herokuでdiscord.pyを始めるテンプレートです。
- Use Template からご利用ください。
- 使い方はこちら： [Discord Bot 最速チュートリアル【Python&Heroku&GitHub】 - Qiita](https://qiita.com/1ntegrale9/items/aa4b373e8895273875a8)

## 各種ファイル情報

### discordbot.py
PythonによるDiscordBotのアプリケーションファイルです。

### requirements.txt
使用しているPythonのライブラリ情報の設定ファイルです。

### Procfile
Herokuでのプロセス実行コマンドの設定ファイルです。

### runtime.txt
Herokuでの実行環境の設定ファイルです。

### app.json
Herokuデプロイボタンの設定ファイルです。

### .github/workflows/flake8.yaml
GitHub Actions による自動構文チェックの設定ファイルです。

### .gitignore
Git管理が不要なファイル/ディレクトリの設定ファイルです。

### LICENSE
このリポジトリのコードの権利情報です。MITライセンスの範囲でご自由にご利用ください。

### README.md
このドキュメントです。
"# AmongUsBot_discord" 
