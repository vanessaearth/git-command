# git版本回退
1.git log 查看所有提交记录
~~~
git log
~~~

ps:查看log的简洁版，添加--pretty=oneline
~~~
git log --pretty=oneline
~~~
2.回退到上一版本
~~~
git reset --hard HEAD^
~~~
3.回退到指定版本
~~~
git reset --hard "版本号"
~~~
ps：版本号就是git log 结果的最前面的一串SHA1计算出来的一个非常大的数字，用十六进制表示
4.版本回退后，且关闭命令行，第二天找不到最新版的版本号使用
~~~
git reflog
~~~
