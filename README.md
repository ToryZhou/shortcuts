# shortcuts
This is the  staple and useful shortcuts for an engineer

Practice the vim is really helpful

这是对大量快捷键优化筛选出来，实用好用的快捷键

****
	
|Author|Tong|
|---|---
|E-mail|522617505@qq.com


****
## 目录
* [vim](#vim)
* [Idea](#idea)
* [VSCode](#vscode)
* [Ubuntu](#ubuntu)
* [Windows](#windows)
* [Chrome](#chrome)
* [tmux](#tmux)
* [CSDN](#csdn)
* [Maven](#maven)
* [Docker](#docker)
* [Js](#Js)
* [Git](#Git)

### vim
-----------
vimtutor   
operator [number] motion 操作+次数+操作对象  

| 操作 | 描述 |
|---|---
|v|选择
|y|复制
|d|删除
|c|修改
|g|移动行

| 操作对象 | 描述 |
|---|---
|w|单词
|e|单词结尾
|0|行首
|$|行尾
|h|左字符
|j|下一行
|k|上一行
|l|右字符

i 当前光标插入  
a 光标后面插入  
o 下一行插入  
:q! 不保存退出  
:wq 保存退出  
:set nu 加上行号  
:set nonu 去掉行号  
:nohl 去掉高亮显示  
/ 查询  
n 向下查询  
shift + n 向上查询  
数字+↑↓ 向上/向下移动n行   
p 粘贴  
dd 删除当前行  
yy 复制当前行  
u 撤销操作  
Ctrl+r 恢复上一步被撤销的操作  
:10,17 s/^/#/    10行到17行行首添加#  
:10,17 s/$/#/    10行到17行行尾添加#  
x    删除光标下的字符 ("dl" 的缩写)  
X    删除光标前的字符 ("dh" 的缩写)  
D    从当前位置删除到行尾 ("d$" 的缩写)  
shift+g 到文件最后一行  
ctrl+g 显示行信息  
% 找对应的括号  
viw 选中光标所在单词  
shift+v 选中光标所在行  
grep -rn "hello,world!" * 搜索文本所在文件  
shift + [ ] 向上/下一个空白行移动  
:%s/字符串//ng 统计字符串出现次数  
:m,ns/字符串//ng  统计指定行出现字符串次数  
du -sh * 查看当前目录文件和文件夹大小，为了解决/dev/sda2满了的问题    
python3 MainMigration.py >> prod_test_big_table.log 2>&1 & 运行python记录日志，标准输出和错误都记录到log文件,并且后台运行   
jobs -l 查看正在运行的后台程序    
sudu su  切换到root用户    
yum install tmux   
emmet    
:reg  查看寄存器
"+y  复制到系统剪切板   
"+p  粘贴系统剪切板   
ctrl+R 寄存器标识， 输入模式下这个命令， 粘贴寄存器内容

### Idea
-----------
windows版 http://idea.lanyus.com/ 里面获取注册码，很长的注册码，在idea第二个单选框内贴入注册码即可，会提示registered by lan yu.  
ctrl + n 查看java文件  
ctrl + shift + n 查看非java文件  
ctrl + space 补全代码  
ctrl + q 查看文档  
alt + f7 查看方法使用  
ctrl +alt + o 去掉没用的引用  
ctrl + alt + l 格式化代码  
ctrl + z 回退操作  
ctrl + shift + z 前进操作 
ctrl +alt + v 生成变量  
ctrl + y 删除一行  
ctrl + d 复制一行  
sout + tab 快速打印  
psvm + tab 快速生成main函数  
ctrl + f9 编译项目  
ctrl + alt + h 查看方法调用  
alt + insert 自动创建getter setter  
Shift+Alt+Up/Shift+Alt+Down 把代码与上面一行/下面一行交换位置  
ctrl + f4 关闭当前tab  
ctrl+shift+space 列出变量  
ctrl+tab 切换文件  
ctrl+shift+tab 切换工具栏  
alt+shift+b Builder Generator(This is a plugin)  
alt+insert 在选中某包是按这个建，创建包和创建类快捷键  
alt+ ←→ 切换工作区文件  
alt+w 打开windows 可以选择项目  
ctrl+alt+\[ \]  左右切换打开的项目 

### VSCode
-----------
ctrl + p  搜索文件  
ctrl + shift + p 功能列表  


### Ubuntu
-----------
ctrl + alt + t 调出新窗口terminal  
ctrl + shift + t 新打开一个tab的terminal  
alt + 数字键 切换terminal的tab  
ctrl + alt + d 打开桌面  
system + l 锁屏  
ctrl +alt + ↑↓←→ 切换虚拟桌面  
ctrl + 1 文件夹文件列表显示  
ctrl + 2 文件夹文件图片显示  
ctrl + r 搜索命令  
history 查看历史记录  
f2 改文件名  
ctrl + a 光标移至行首  
alt  + ↑ 进入上级文件夹  
alt + ↓ 进入下级文件夹  
alt + ← 后退  
alt + → 前进  
alt + · 同类型窗口切换  
bc 计算器  
tail -f 文件名 持续查看该文件  
history | grep  查找关键词  
free -m 查看内存  
df 查看硬盘  
date 查看日期  
pwd 当前路径  
sudo -s 使用root用户  
cd  
ls  
ls -a  
ll  
useradd zhengyang  
passwd zhengyang  
alt+f7 updated to alt+m move window  
/etc/sudoers to let user get the root role  
system+shift+number 另起程序标签  
find <directory> -type f -name "*.c" | xargs grep "<strings>"  linux 多个文件中查找字符串  
find ./ -type f -name "*.xml" | xargs grep "liquibase"    
sudo updatedb 更新linux索引数据库  
locate test.txt 快速查找文件  
file -i companies_test_code.csv 查看文件字符编码  
ngg或nG 跳转到第n行  
lsof -i:32888 查看端口占用程序，kill -9 24029 杀掉对应程序pid  
find . -type f   -exec  sed -i 's/\xEF\xBB\xBF//' {} \;  
这个命令会把当前目录及所有子目录下的BOM头删除掉。
grep -rn 920b8f5ffa8a477282b2c7bf9e530354 app.* 搜索app开头的文件里面的字符串   
grep -rn role1 app* | grep 7199c2a1f7274518a3b4c68aa0ca63c3  
sudo hdparm -i /dev/sda  查看硬盘型号  
echo $LANG  查看系统字符编码  
xz -d ***.tar.xz 解压.xz文件  
tar -xvf  ***.tar 解压.tar文件  
tar -zxvf Python-3.6.1.tgz  解压.tgz文件   
update-alternatives --config python  切换版本  
du -h ./ | sort -n -r | head -n 10 看文件大小  
du -hs 查看但前文件夹大小  
du -lh --max-depth=1 查看深度为1的文件和文件夹大小  
nohup python3 -u migration.py > prod.log 2>&1 &  后台运行脚本，断开远程链接可以继续运行  
ssh-keygen -t rsa -C "zhoutong@patsnap.com" 生成ssh key pair  
mv ~/.ssh/known_hosts ~/.ssh/known_hosts_bak  把hosts冲突删除  
wc -l filename 就是查看文件里有多少行   
ctrl + l  terminal里面新的一屏   
less j 向下， k 向上


### Windows
-----------
system + e 打开文件夹  
alt + space 打开窗口管理  
system + r 调出运行命令行  
f2 改文件名  
f3 向下搜索  
system + 数字 打开开始菜单栏的第n个应用  
system + x 系统管理  
system + x + uu 关机  
shutdown -s -t 2555 2555秒后关机  
services.msc 系统服务  
calc 计算器  
ctrl+system+ ↑  最大化窗口  
ctrl+system+ ↓  缩小窗口  
 

### Chrome
-----------
ctrl + shift + b 打开关闭收藏目录  
ctrl + t 打开新标签页  
ctrl + n 打开新窗口  
ctrl + shift + t 打卡刚关闭的标签页  
ctrl + w 关闭标签页  
ctrl + d 收藏当前页  
ctrl + r 刷新当前页  
alt + ←→ 后退/前进  
ctrl + 数字  打开第n个标签页  
Ctrl+1 到 Ctrl+8 切换到指定位置编号的标签页。您按下的数字代表标签页横条上的相应标签位置。   
Ctrl+9 切换到最后一个标签页   
Ctrl+Tab 或 Ctrl+PgDown 切换到下一个标签页  
Ctrl+Shift+Tab 或 Ctrl+PgUp 切换到上一个标签页  
ctrl + l 光标定位到地址栏  
tab 光标跳到下一个form元素  
shift + tab 光标跳转到上一个form元素  
ctrl + h 查看历史记录  
ctrl + j 查看下载记录  
ctrl+o 选择文件 在谷歌浏览器中打开计算机上的文件  
按住 Ctrl 键，然后点击链接 从后台在新标签页中打开链接，但您仍停留在当前标签页中   
按住 Ctrl+Shift 键，然后点击链接 在新标签页中打开链接，同时切换到新打开的标签页   
按住 Shift 键，然后点击链接 在新窗口中打开链接  
Esc 停止加载当前页  
Ctrl++，或者按住 Ctrl 键并向上滚动鼠标滚轮 放大网页上的所有内容   
Ctrl+-，或者按住 Ctrl 键并向下滚动鼠标滚轮 缩小网页上的所有内容   
Ctrl+0 将网页上的所有内容都恢复到正常大小  
Ctrl + Shift +N 打开安全模式  

### tmux
-----------
tmux  
ctrl+b 进入命令模式后，%左右分屏，“上下分屏，方向键选择屏幕，d退出会话  
tmux new -s redis 新建会话  
tmux a -t redis 进入会话  
tmux ls 列出所有会话  

### CSDN
-----------
shift + enter 换行不分段   

### Maven
-----------
mvn clean install -Dmaven.test.skip=true  通过这样的方式可以跑到checkstyle，直接点击install 按钮 跑不了checkstyle  
java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb -port 10500  dynamodb  

### Docker
-----------
查看docker运行状态的方法:sudo service docker status  
打开/关闭/重启docker服务：sudo service docker start/stop/restart  

### Js
----------
console.log(document.getElementById("password").value) 获取网页密码  
new Date(1557575716243)获取时间戳转换  
new Date().getTime()获取当前Unix时间戳  
decodeURI('%5D%2F')有的解码不了 

### Git
----------    
git tag tag-20210812    
git push origin tag-20210812    
git tag -d tag-name  删除本地tag  
git push origin :refs/tags/tag-name  删除远程tag  
git branch -m master old-master   
git branch -m develop-rds-bak master   
git push -f origin master  

git fetch -a origin-tong 获取远程仓库的所有分支  
	
git checkout -b develop origin/develop  git checkout -b {本地分支} {远程分支}   
	
git branch <new-branch-name> <tag-name>  从branch拉分支 

注意Markdown 锚点里面必须是小写
---------------------

本文来自 ToryChow 的CSDN 博客 ，全文地址请点击：https://blog.csdn.net/changningbuddha/article/details/76167929?utm_source=copy 
