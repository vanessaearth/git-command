# git pull 或者 其他命令出现以下错误 
一. error: bad index file sha1 signature fatal: index file corrupt
###  解决方法：
 1.在项目中有。git的目录下打开git bash 输入：rm -f .git/index
 
 2.输入：git reset
 出现
~~~
Unstaged changes after reset:
M       Public/css/mobile/Ambitus/detail.css
M       Public/css/mobile/Ambitus/index.css
~~~
 3.重启开发工具
 二.当git pull提示：fatal: refusing to merge unrelated histories
使用以下命令：
 ~~~
 git pull origin master --allow-unrelated-histories
 ~~~
 
 
