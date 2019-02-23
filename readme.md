### git的基本命令手记

> `git add 文件名`

添加文件到待提交队列

<br/>

> `git commit -m "描述"` 

将待提交队列中的文件提交至暂存区

<br/>

> `git push` 

将暂存区的所有文件提交至远程相应分支

<br/>

> `git pull` 

将远程分支合并至本地相应分支中

<br/>

> `git branch 分支名` 

创建本地分支

<br/>

> `git checkout 分支名` 

切换本地分支

<br/>

> `git checkout -b 分支名` 

创建并切换到相应本地分支

<br/>

> `git push --set-upstream origin 分支名` 

该命令用于将本地分支提交到远程仓库(用于第一次本地分支的提交)

<br/>

> `git branch -d 分支名`

删除本地分支

<br/>

> `git branch -D 分支名`

强制删除本地分支

<br/>

> `git push origin -d 分支名`

删除远程分支

<br/>

> `git merge 分支名`

将指定分支合并到当前分支中，如有冲突，需要手动解决再提交。

