## ワークフロー名
name: に記載する

## イベント
on: に記載
on: push, on: [push, pull_request]

## ジョブ
ワークフローの実行単位

## ランナー
runs-on: ジョブの実行環境

## ステップ
steps: 上から順に処理。シェルコマンドとアクションを実行できる

### シェルコマンド
yml記法でシェルを実行できる
run: |
  git log -1
  tree -a .

### アクション呼び出し
Github Actionのモジュール
- uses: actions/checkout@v4
  with:
    ref: main
