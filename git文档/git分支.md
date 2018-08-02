##git分支

查看分支：git branch

查看本地和远端分支：git branch -a

创建分支：git branch name

切换分支：git checkout name

创建+切换分支：git checkout –b name

克隆指定分支：git clone -b name url

合并某分支到当前分支：git merge name

删除分支：git branch –d name  
`error: The branch 'name' is not fully merged`  
` 表示当前删除的分支 有没有合并到当前分支的内容`  
 `可以使用 -D 强制删除`  
 `或者使用git merge name 将代码合并到当前分支`


删除远程分支：git push origin --delete name

将本地创建的分支发布到远程仓库：git push origin name:name

推送本地分支代码到远程分支：  `git add . ` `git commit -m message`  `git push origin`  
可能会报错: `fatal: The current branch KSjv has no upstream branch.  本地和远程仓库没有关联`  

将本地分支和远程仓库创建关联：  git push -u 远端仓库地址  分支的名字
