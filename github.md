#githubでよく使用するコマンドのチートシート   

## Gitで使う名前とアドレスの作成
```
# グローバル設定
git config --global user.name "username"
git config --global user.email "email"

# 該当リポジトリ
git config user.name "username"
git config user.email "email"
```
## ファイルをインデックスに登録
```
git add filename

#カレントディレクトリの指定
git add .

#全てのファイルを登録
git add --all

```

## 変更をローカルリポジトリにコミット
インデックスに登録されているファイルの変更をリポジトリにコミットする。   
```
#コミット
git commit -m 'message'

```
```
## ローカルリポジトリやワーキングツリーの状態を確認する。   
```
git status
```
## ファイルの移動、変更、削除
```
#移動・変更
git mv

#削除
git rm
```
## ローカルリポジトリにリモートリポジトリのデータを反映する
githubからぷるしてくる
```
git pull origin リモートブランチ
```
## リモートリポジトリにローカルリポジトリのデータを送信する
```
#リモートリポジトリ「origin」に「master」ブランチを送信
git push origin ローカルブランチ名

#反映先のブランチを指定
git push origin ローカルブランチ名:リモートブランチ名
```

## ブランチのチェックアウト
```
git checkout ブランチ名
```
## 特定のタグのブランチを作りチェックアウトする
```
このコマンドでv2.2.5という名前のtag2.2.5のブランチができる
git checkout -b v2.2.5 refs/tags/2.2.5
```
