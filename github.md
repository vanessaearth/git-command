
1.or create a new repository on the command line

echo "# cc" >> README.md

git init

git add README.md

git commit -m "first commit"

git remote add origin https://github.com/vanessaearth/xxx.git

git push -u origin master


2.…or push an existing repository from the command line

//添加远程git仓库

git remote add origin https://github.com/vanessaearth/xxx.git

//将分支提交到远程

git push -u origin master

//添加远程git仓库报错，删除远程git仓库

git remote rm origin

(如果报错) vi .git/config 删除[remote "origin"]

//增加远程git仓库

git remote add origin https://github.com/..../test.git

3.…or import code from another repository

You can initialize this repository with code from a Subversion, Mercurial, or 
TFS project.
