### 课程链接[https://www.bilibili.com/video/BV1vy4y1s7k6](url)
### IDEA集成github与gitlab未学习

git 分布式版本控制工具 （从远程库clone，在自己电脑上做版本控制）
svn 集中式（客户端连接，统一修改中央服务器代码） 

工作区 （写代码）
暂存区 （临时存储）
本地库 （历史版本）

代码托管中心
局域网 gitlab
互联网 github/gitee

### 开始写git
设置用户签名，明白是谁提交了代码
git config --global user.name .../user.email ...
git init初始化
git status查看状态（目前分支，提交情况，工作区/暂存区追踪文件）
git add <file>
ls 查看工作区
ll/ls -l 详细查看
git commit -m "日志信息" <file>
git reflog 提交记录
git log 详细，包括提交人
git reset --soft/mixed/hard ...（版本号） 版本穿梭（改变指针位置即可）(更改保留/仅暂存区更改移除/移除)


### 分支（指针的引用）
git branch 创建
git branch -v 查看
git checkout 切换
git merge （其他分支） 合并（在主分支上将其他分支合并）

### 合并冲突
提交不要带文件名，系统不知道是哪个文件

git push 别名 分支
git pull 别名 分支==git fetch+git merge
git fork 创建远程库副本

### 远程库
git remote -v 查看所有远程库别名
git remote add 别名 远程库
git clone (拉取代码，初始化本地库，创建别名origin)

### ssh免密登陆
公私钥通常保存在~/.ssh/中
公钥 id_rsa.pub
私钥 id_rsa

### gitlab
使用git作为代码管理工具搭建的web服务

补充
rm 文件名 删除
rmdir 文件夹 删除
touch <file> 创建
mkdir <directory> 创建
mv <source> <destinaton> move
cp <...> <...> copy
. 所有文件，如git add . 跟踪当前文件夹的所有文件