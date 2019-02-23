### git的基本命令手记

<br/>

#### 添加文件到待提交队列

> `git add 文件名`

<br/>

#### 将待提交队列中的文件提交至暂存区

> `git commit -m "描述"` 

<br/>

#### 将暂存区的所有文件提交至远程相应分支

> `git push` 

<br/>

#### 将远程分支合并至本地相应分支中

> `git pull` 

<br/>

#### 创建本地分支

> `git branch 分支名` 


<br/>

#### 切换本地分支

> `git checkout 分支名` 

<br/>

#### 创建并切换到相应本地分支

> `git checkout -b 分支名` 


<br/>

#### 将本地分支提交到远程仓库

> `git push --set-upstream origin 分支名` 

该命令用于第一次本地分支的提交

<br/>

#### 删除本地分支

> `git branch -d 分支名`


<br/>

#### 强制删除本地分支

> `git branch -D 分支名`

<br/>

#### 删除远程分支

> `git push origin -d 分支名`


<br/>

#### 将指定分支合并到当前分支

> `git merge 分支名`

如有冲突，需要手动解决再提交

