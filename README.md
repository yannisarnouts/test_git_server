git init .
git add .
git commit -m "Import with merge"
git remote add origin https://github.com/yannisarnouts/test_git_server.git
git fetch origin
git merge origin/master -s recursive -X ours --allow-unrelated-histories -m "merge master to enable the import"
git push -u origin master