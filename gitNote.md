### 基础操作

```shell
# 查看当前分支代码修改情况 ：
git status   
# 拉取远程分支代码： 
git pull 
# 提交本地的代码到本地分支：
git add  xxx  或者 git add . (add . 是所有有修改的文件）
# 给本次提交写备注：
git commit -m "注释"；
# gitK 查看修改的详细情况【gitK 乱码解决】
git config --global gui.encoding utf-8
# 切换分支：
git checkout mater；
# 拉取切换分支后的代码：
git pull；
# 把自己分支合并到当前分支（将dev-suibin合并到当前所在分支） 
git merger dev-suibin；
# 提交合并后的代码：
git push；
# 切换到本地自己分支：
git checkout dev-suibin;
# 使自己的分支保持最新：
git merge dev
# git push origin master :master (如果前面的master没有就是删除)
git push 本地分支:远程分支（直接 git push  就是将本地的项目推送到对应的远程目录） 
git checkout  master （切换分支到master）
git merge dev （将dev合并到master分支）
# 拉分支到本地：
git pull origin master:master
# 合并指定的commit到当前分支
git cherry-pick 82ecb31 
# git查看只commit没有push的文件或者提交记录
git cherry -v
# 创建本地分支
git checkout -b newBranch
# 推送到远程
git push origin newBranch
# 分支名 推送本地分支到远程仓库
git push --set-upstream origin 
# 将远程git仓库里的指定分支拉取到本地（本地不存在的分支）
git checkout -b 本地分支名 origin/远程分支名
# 删除本地分支，git branch -D dev_temp  -D强制删除
git branch -d  dev_temp
# 删除远程分支
git push origin --delete dev_temp 
# 同步本地分支信息和远程分支信息保持一致（解决：git branch -r 显示了实际远程不存在的分支问题）
git fetch origin --prune
```