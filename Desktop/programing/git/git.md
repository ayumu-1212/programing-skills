# gitに関して

## ローカルリポジトリ作成後、リモートリポジトリにpushする際の手順
```
git init
git add [file]
git commit -m "コメント"
git remote add [urlの名前] [リモートリポジトリのurl]
git push [urlの名前] [branchname]
```

## remoteとは
'''
git remote add urlにつける名前 url  # remoteとlocalをurlでつなぐ
git remote                          # url一覧
git remote rm urlの名前             # urlを削除
git remote set-url urlの前の名前 urlの新しい名前 #urlの名前変更
'''

## 取り消しコマンド一覧
```
git reset HEAD                    # 1つ前のaddを取り消す
git reset [addしたファイル名]     # 特定のaddしたファイルを取り消す
git commit --amend -m "ミスったよ"  # 一つ前のcommitメッセージを変更する
git reset コミット番号            # 特定のコミットまで戻る
git revert コミット番号           # 特定のコミットを消す
git stash save                    # 変更を退避する
git stash list                    # 退避リストを見る
git stash apply [stash名]         # 退避を戻す
git stash drop [stash名]          # 退避を消す
git stash clear                   # 退避を全部消す
git stash pop [stash名]           # 退避を戻すのと同時に消す
```
