#gitを導入したときにやるべき最初の設定
##ユーザー名とメールアドレス設定
https://help.github.com/articles/setting-your-email-in-git/
メールアドレスは非公開にし、githubのアカウントと紐付けたいときは以下のようにする
```
$ git config --global user.name "githubusername"
$ git config --global user.email "username@users.noreply.github.com"
```

他にもエディタの指定とかやったほうが良さそうな設定はありそう