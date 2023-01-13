Git is a version control system.
Git is a free software.
--20230113
--20121906

Help:

1. 初始化仓库：
   git init
2. 添加文件到Git仓库：
   step 1: git add <file>
	e.g. git add readme.txt
   step 2: git commit -m <message>
	e.g. git commit -m "added xxx"
3. 查看工作区状态（是否有修改、是否待commit、是否已commit）：
   git status
4. 查看修改内容：
   git diff <file>

【关于版本管理】
————已经commit到本地版本库————
5. 回到过去某个版本：
   git reset --hard <commit_id> (前几位数即可）
   回到最新版本：
   git reset HEAD <file.x>
6. 查看commit历史：
   git log
7. 查看命令历史：
   git reflog （用于找回“未来”）
————还未commit到本地版本库————
8. 丢弃工作区修改//让这个文件回到最近一次git commit或git add时的状态:
   git checkout -- <file>
9. 丢弃暂存区修改：
   git reset HEAD <file>

【关于删除文件】
1. 删除file（手动or rm test.txt）
2. 把变化添加到暂存区：
   git rm <file>
3. 把变化添加到版本库：
   git commit -m "remove xxx"

