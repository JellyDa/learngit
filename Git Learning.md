#git的一些使用命令
---

1. 初始化一个git仓库，使用```git init```命令。
2. 添加文件到git仓库，分两步：  
	>- 使用命令```git add <file>```，注意，可反复多次使用，添加多个文件；  
	>- 使用命令```git commit -m <message>```,完成。

1. 要随时掌握工作区的状态，使用```git status```命令。
2. 如果```git status```告诉你有文件被修改过，用```git diff```可以查看修改内容。
3. ```HEAD```指向的版本就是当前的版本，因此，Git允许我们在版本的历史之间穿梭，使用命令```git reset --hard commit_id.```（HEAD^表示上一个版本，也可以是HEAD~n,前n个版本）
4. 穿梭前，使用```git log```可以查看提交历史，以便确定回到哪个版本。
5. 要重返未来，用```git reflog```查看历史命令，以便确定回到未来的哪个版本。
6. 未添加的状态为```Untracked```
7. ```git add```是放到缓存区，```commit```是将缓存区的内容提交到工作区
8. ```git checkout -- <filename>```撤销工作区更改，回到最上一次的状态
9. ```git reset HEAD -- <filename>```撤销提交到缓存区的文件，回到提交前工作区的状态
10. ```git rm```,删除版本库中的文件，得首先删除工作区的文件，如果删除工作区文件之后，可以用```git checkout <file>```来从版本库中恢复。
11. 要关联一个远程仓库，使用```git remote add origin git @servername.git```
12. 关联后，使用```git push -u origin master```第一次推送master分支的所有内容
13. 以后，每次提交本地的文件之后都可以使用```git push origin master```来推送最新的更改
14. ```git clone```克隆GitHub上的仓库
15. 查看分支：```git branch```
16. 创建分支：```git branch <name>```
17. 切换分支：```git checkout <name>```
18. 创建＋切换分支：```git checkout -b <name>```
19. 合并某分支到当前分支：```git merge <name>```
20. 删除分支：```git beanch -d <name>```
21. 
