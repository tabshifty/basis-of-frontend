## git是什么
**分布式**、**版本控制**软件

现今的版本控制包括：
* 文件拷贝
* 本地版本控制
* 集中式版本控制，可以进行多人协作，所有的版本文件都放在一个地方，如SVN。
* 分布式，所有的版本除了放在一个集中的仓库外，协作方本地也会有所有的版本

### 为啥要使用版本控制
* 功能版本回滚迭代
* 协作开发

## git的初始使用步骤
先配置好个人信息`git config --global user.name "name"`和user.email

* 初始化文件所在的文件夹`git init`
* 使用`git status`检测当前所有文件的状态
* 使用`git add`命令添加想要管理的文件
* 用`git commit`来生成一个版本

查看所有的版本commit信息`git log`

文件状态： 
* 新增的文件或这修改后的版本里的文件
* 已经放在git版本里的文件
* 已经add未commit的文件

## git里面的文件状态区域
工作区|暂存区|版本库
--|:--:|--:
新增的文件或这修改后的版本里的文件|已经add未commit的文件|已经放在git版本里的文件

状态区域可以切换
 * `git commit --amend` 修改commit的提交信息
 * `git reset --soft HEAD^` 撤销commit到暂存区 soft仅移动版本库HEAD指针
 * `git reset --mixed HEAD^`撤销至工作区 mixed移动版本库指针并重置暂存区
 * `git reset HEAD <file>` 取消暂存的文件
 * `git checkout --<file>`撤销文件的修改（存在于工作区的文件，未被暂存）
### 版本回滚
使用`git reflog` 查看版本号 
三种方式
 * 使用版本号 `git reset --hard <version number>`
 * 只能后退 `HEAD^`，`^`的个数表示回退多少个版本
 * 只能后退 `HEAD~n` `n`表示回退多少个版本
## 删除文件找回 

## 比较文件差异

## 分支
 * `git branch` 新建分支， `git checkout`切换到分支上去
 * `git checkout -b`新建并切换到分支上去
 * `git branch -d`删除分支
 * `git merge`合并分支， `git merge --abort`取消合并

## 远程仓库
 * `git clone`
 * `git remote add -u origin <url>` 添加远程地址别名
 * `git push -u origin <branch>`
 * `git pull origin <branch>`拉取更新，非常重要
 * `git pull` = `git fetch` + `git merge`

## rebase 应用
 * 多个记录合并
 * 合并分支 `git rebase`, `git checkout`, `git merge`
 * 合并远程 `git fetch`, `git rebase`, `git merge` or `git fetch --rebase`
产生冲突：解决冲突， `git add`, `git rebase --continue`

## 工作流（简易）

