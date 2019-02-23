## git的基本命令（手记）

<br/>

#### 初始化仓库

> `git init`

<br/>

#### 添加文件到暂存区

> `git add 文件名`

<br/>

#### 将暂存区中的文件提交到当前本地分支

> `git commit -m "描述"` 

<br/>

#### 撤销对本地分支文件的修改

> `git checkout -- 文件名` 

当在`git commit`提交文件到本地分支又进行修改后，可以使用该命令来撤销对相应文件的所有修改

<br/>

#### 撤销对本地分支文件的修改

> `git reset HEAD 文件名` 

当已经提交到本地分支的文件被修改后又提交到了暂存区(`git commit` -> 修改了文件 -> `git add 该文件`)

使用该命令将该文件移除暂存区，再使用`git checkout -- 文件名`撤销对该文件的所有修改

<br/>

#### 删除已提交文件

> `git rm 文件名` (`rm 文件名`)

当文件已经被提交到本地分支时，可以使用该命令删除文件

<br/>

#### 恢复删除的文件

+ 当文件是通过`rm 文件名`（文件管理器）删除的，可以直接通过`git checkout -- 文件名`恢复到版本最新状态

+ 当文件是通过`git rm 文件名`删除的，先通过`git reset HEAD 文件名`，再通过`git checkout -- 文件名`恢复到版本的最新状态

<br/>

#### 查看版本

> `git log`

<br/>

#### 版本回退

> `git reset 提交的id`

<br/>

#### 检查暂存区各文件的状态

> `git status`

<br/>

#### 检查文件前后对比

> `git diff`

将修改的文件与暂存区的相应文件作对比

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

#### 将本地分支与远程分支关联

> `git branch --set-upstream-to=origin/分支名 分支名` 

<br/>

#### 将本地分支与远程分支关联并切换至该分支

> `git checkout -b 分支名 origin/分支名`

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

#### 将指定分支合并到当前本地分支

> `git merge 分支名`

如有冲突，需要手动解决再提交

<br/>

#### 给版本库标注版本号

> `git tag v版本号` (如`git tag v1.0`)

<br/>

> `git tag v版本号 commit_id` (如`git tag v1.1 b9fd8f92c78b504d627651e018e6e9213b9a7d9d`)

给对应的版本库添加版本号

<br/>

#### 通过版本号查看版本库

> `git show v版本号` (如`git show v1.0`)

<br/>

#### 查看库的所有版本

> `git tag`

<br/>

#### 推送版本号至远程主机

> `git push origin v版本号` (如`git push origin v1.0`)

<br/>

#### 删除本地版本号

> `git tag -d v版本号` (如`git tag -d v1.0`)

<br/>

#### 删除远程主机版本号

> `git push origin :refs/tags/v版本号` (如`git push origin v1.0`)

<br/>

