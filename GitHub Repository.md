# 新規作成

- ghq get [Repository URL]

- GitHub アプリケーションに新リポジトリを紐付ける  
  https://github.com/settings/installations

- セキュリティ関連の機能を有効にする  
  https://github.com/kurosame/memo/settings/security_analysis

# 複製

1. GitHub 上で bk 用の新しいリポジトリを作成
1. 以下のコマンドを実行

```sh
git clone --bare https://github.com/kurosame/[複製元リポジトリ名].git
cd [複製元リポジトリ名]
git push --mirror [複製先リポジトリ名（会社PCの場合は`kurosame@`を付ける）].git
```
