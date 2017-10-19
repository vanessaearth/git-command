# Git使用
#### 一.下载和安装
Git官网下载git，https://git-scm.com/
下载完，安装。
安装完成后，在文件夹中右键，会多出Git GUI Here和Git Bash Here个菜单，Git GUI Here是可视化菜单，Git Bash Here是命令行菜单，打开Git bash Here,进入命令行界面，输入git --version，后显示git版本号则安装成功，否则安装失败。


----------


#### 二．本地提交到远程仓库
2.1在github上新建一个仓库

本地新建一个文件夹demo，进入test，打开Git Bash

2.1初始化文件夹，执行后多一个,git文件夹

git init

在文件夹中新建一个readme.md文件

git status//查看本地仓库中文件的状态

2.2添加所有文件到本地仓库

gt add -A

2.3提交到本地仓库

git commit -m ‘remark’ 

第一次需要配置用户名和邮箱

git config --global user.email ‘123456@qq.com’

git config --global user.email ‘summer’

2.4添加远程仓库地址

git remote add origin (github地址)

2.5提交到远程仓库

git push -u origin master

到gitHub上找到仓库，就能看见提交到文件

3.文件修改后执行以下就行

git add -A

git commit -m ‘haha’

git push


----------

#### 三．从远程仓库到本地
git clone (github地址)

如果github地址是https可以直接下载

如果为ssh则需要配置公共秘钥SSH


----------

#### 四．SSH配置公共秘钥
1.设置用户名和邮箱

git config --global user.email ‘123456@qq.com’

git config --global user.name ‘summer’

2.生成密钥

ssh-keygen -t rsa -C “email”

连续3个回车，如果不需要密码的话，最后得到2个文件id_rsa和id_rsa.pub

3.添加秘钥到ssh-agent

ssh-add ~/.ssh/id_rsa

（（报错could not open a connection 
to your authentication agent，执行ssh-agent bash命令））

4.登录github，添加ssh

把id_rsa.pub文件里的内容复制到用户设置下的ssh keys

5.ssh -T git@github.com

看见HI，你的用户名，则成功
 
#### 五．每天好习惯

git pull

git status

git add readme.md

git commit -m 'fix'

git push
