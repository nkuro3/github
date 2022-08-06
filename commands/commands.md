```
リポジトリ作成
git init

リモートリポジトリへ追加
git remote add origin [ローカルリポジトリ]
git remote add origin git@github.com:nkuro3/github.git

ステージング
git add [対象パス1] [対象パス2] ...
git add .  # 一括

コミット
git commit -m "コミットメッセージ"
git commit –amend "直前のコミットのメッセージ変更"

プッシュ
git push [マージ先のリモートリポジトリ名] [マージ元のローカルリポジトリ名]
git push  # push to origin

プル
git pull [リモートリポジトリ] [ローカりリポジトリ]
git pull origin main

リポジトリを最適化
git gc

```