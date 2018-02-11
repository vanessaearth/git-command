# Git常用命令和基本理解

ps:工作区有一个.git的隐藏目录，

通过add命令添加工作区的内容到stage暂存区，

然后commit，把暂存区的内容提交到本地仓库的当前分支

然后push，提交本地仓库的内容到远程仓库

1.克隆代码

 git clone github的代码地址

2.新建分支

git branch 分支名(dev)

3.切换分支

git checkout 分支名(dev)

(创建+切换)git checkout -b 分支名(dev)

4.查看所有分支

git branch -a

5.本地新建分支关联到远程

git branch --set-upstream-to=origin/dev dev

 提交前关联

git push --set-upstream origin test

6.删除本地分支

git branch -d dev

7.删除远程分支

git push origin :dev

8.删除远程git仓库

git remote rm origin

(如果报错) vi .git/config 删除[remote "origin"]

9.增加远程仓库

git remote add origin https://github.com/..../test.git

10.更新代码(git pull)

11.查看代码状态(git status)

12.提交代码到暂存区(git add .)

13.提交代码到本地仓库(git commit -m 'fix')

14.git fetch origin develop:develop将远程分支代码拉取到本地.。

15.(当前分支master)git merge dev 合并dev分支到master分支

$ git pull
当拒接pull时，fatal: refusing to merge unrelated histories
使用：git pull --allow-unrelated-histories


-----------over----------
