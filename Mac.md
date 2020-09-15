# Initial Setup

## Mac

- Dock から Finder 以外を削除
- システム環境設定
  - 一般
    - ダークモード
  - デスクトップとスクリーンセーバー
    - スクリーンセーバーを開始しない
  - Dock
    - Dock を自動的に表示/非表示にチェック
  - 通知
    - 通知を許可するアプリの設定（基本的にオフ）
  - キーボード
    - リピート速度を上げる
    - Google 日本語入力を追加して、Mac 標準の入力ソースは削除
  - トラックパッド
    - すべてチェックして、使ってみて邪魔な動作を外していく
    - カーソルの速度調整
  - 省エネルギー
    - バッテリーと電源アダプターのオフ時間を 3 時間にする
    - メニューバーのバッテリーから割合（％）を表示
- Homebrew と Homebrew Cask をインストール

## Finder

- 環境設定
  - 一般
    - 新規 Finder を開いた時の表示を変更
  - サイドバー
    - 表示する項目をチェック
  - 詳細
    - 拡張子を表示
- 隠しファイルを表示
  - `command + shift + .`

## Terminal

- 一般
  - 起動時に開くプロファイルを変更
- プロファイル
  - プロファイルを探してインポートする
    - オススメのプロファイル
      - [Iceberg](https://cocopon.github.io/iceberg.vim)
  - インポートしたプロファイルをデフォルトにする
  - ウインドウ
    - ウインドウサイズを調整
  - シェル
    - シェルの終了時はウインドウを閉じる
    - ウインドウを閉じる前の確認はしない
- デフォルトのシェルを zsh に変更
  - `chsh -s /bin/zsh`

## Zsh

Prezto をインストール  
https://github.com/sorin-ionescu/prezto#installation

## Homebrew

旧 PC で以下のコマンドを実行し、必要なアプリケーションのみを移行する

- `brew list`
- `brew cask list`

## dotfiles

シンボリックリンクを貼る  
`ln -s ~/ghq/github.com/kurosame/dotfiles/[ファイル名] [作成先フォルダー名]`

**作業前に確認**  
すでに`.`ファイルが作られている可能性があるので、それを上書きしないようにする

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
