# git pull或者其他命令出现以下错误 
 error: bad index file sha1 signature fatal: index file corrupt
###  解决方法：
 1.在项目中有。git的目录下打开git bash 输入：rm -f .git/index
 
 2.输入：git reset
 
出现

Unstaged changes after reset:

M       Public/css/mobile/Ambitus/detail.css

M       Public/css/mobile/Ambitus/index.css

 3.重启开发工具
