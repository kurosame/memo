# Initial Setup

## Mac

## Homebrew

以下のコマンドを実行し、必要なアプリケーションのみを移行する

- `brew list`
- `brew cask list`

## Google Backup and Sync

1. `~/Google Drive`フォルダーを作成
1. `Google のバックアップと同期.app`を実行
1. 同期させるフォルダーを`~/Google Drive`に変更
1. Google Drive 上の`Sync`フォルダーのみを同期する

## SSH Key

### Public Key

`~/Google Drive`フォルダーにある

### Private Key

USB メモリから PC 上にコピーする

## ghq

1. 移行元 PC から`ghq list`の結果を送ってもらう
1. `ghq list`の GitHub リポジトリをすべてクローンする
   - `ghq get https://github.com/kurosame/[リポジトリ名].git`

## Visual Studio Code

1. UI 左下の設定から`Turn on Settings Sync...`を実行
   - 同期対象はすべてチェックしておく
1. `Replace Local`を実行

---

# _`~/`配下の`.`ファイル_

## 常日頃から GitHub リポジトリで管理しておくようにする

[https://github.com/kurosame/dotfiles:embed:cite]

## シンボリックリンクを貼る
