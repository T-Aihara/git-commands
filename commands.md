コマンド一覧
===
よくつかうやつ
---
ディレクトリに移動→.git作成→すべてのファイルをステージングへ移動→ローカルリポジトリにコミット
→リモートリポジトリの情報をローカルに保存→リモートへプッシュというながれ
```
$ git init
$ git add .
$ git commit -m "コミットメッセージ”
$ git remote add repositoryname https://github.com/username/repository.git
$ git push -u repositoryname master
```

.gitを作る
---
リポジトリにあげたいディレクトリで作る。これがないと始まらない。
```
$ git init
```

ステージングにファイルをあげる
---
ファイル名を指定する。
ディレクトリ内のすべてのファイルを上げたいときは「add .」
```
$ git hogehoge.py
$ git add .
```

ローカルリポジトリにコミットする
---
コミットメッセージを付けないといけない。
-mとすることでエディタは立ち上がらずターミナル上で入れられる。
```
$ git commit -m "コミットメッセージ”
```

リモートリポジトリの情報を追加
---
```
$ git remote add repositoryname https://github.com/username/repository.git
```

プッシュ
---
masterとすることでデフォルトのブランチにプッシュする。-uはmasterの時はいらない...らしい。
```
$ git push -u repositoryname master
```