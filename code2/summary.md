# git
## 常用命令
- 配置用户信息
    + git config --global user.name 用户名
    + git config --global user.email 邮箱
- 初始化本地仓库
    + git init
- 初始化远程仓库
    + git init --bare
- 把工作目录文件添加到暂存区
    + git add 文件列表
    + git add *
- 把暂存区中文件添加到本地仓库
    + git commit -m 备注信息
    + git commit -a -m 备注信息 （-a只能提交已修改的文件，不能提交未跟踪文件）
- add的逆操作
    + git rm --cached 文件列表
- 回滚修改的内容
    + git checkout 文件列表
    + git checkout . (回滚所有的修改，慎重使用)
- 使用本地仓库的快照进行回滚
    + git reset
        * --hard
        * --soft
        * --mixed (默认参数)
    * 回滚最后一次提交
        - git reset --hard HEAD^
    * 回滚所有的工作目录和暂存区内容
        - git reset --hard HEAD
- 克隆远程仓库的项目
    + git clone 远程仓库地址 项目名称
- 拉取远程的分支
    + git pull 远程仓库地址 远程分支名称:本地分支名称
- 推送分支到远程仓库
    + git push 远程仓库地址 本地分支名称:远程分支名称
- 添加远程仓库别名
    + git remote add 别名 远程仓库地址
- 删除远程仓库别名
    + git remote remove 别名
- 查看远程仓库别名的详细信息
    + git remote show 别名
- 查看所有别名
    + git remote

## 分支操作
- 创建分支
    + git branch 分支名称
- 切换分支
    + git checkout 分支名称
- 创建并切换分支
    + git checkout -b 分支名称
- 删除本地分支
    + git branch -d 分支名称（如果没有被合并，无法删除）
    + git branch -D 分支名称（强制删除）
- 查看本地分支
    + git branch
- 查看远程分支
    + git branch -r
- 查看所有分支
    + git branch -a
- 删除远程分支
    + git push 远程仓库地址 :远程分支名称
    + git push 远程仓库地址 --delete 远程分支名称
-  保存当前状态
    +  git stash
- 恢复当前状态
    + git stash pop