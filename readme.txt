使用说明：

创建仓库：
git init  可将当前目录变为git可以管理的仓库

添加文件或修改
（1）步骤一：使用 git add readme.txt 添加特定文件到暂存区或者 git add . 添加所有文件
（2）步骤二：使用 git commit -m "第一次修改"   提交修改，即将暂存区的所有内容提交到当前分支

git status 查询文件是否被更新
git diff readme.txt 查询特定文件的修改内容


版本管理
（1）查看提交的历史记录 ： git log  或者 git log -pretty=oneline
（2）版本回退：git reset --hard HEAD^  ，几个^代表上几个版本，或者  git reset --hard HEAD~1
（3）回退到最新版本： git reset --hard 版本号
（4）获取版本号：git reflog 

提交前撤销修改
（1）git checkout -- readme.txt 中的 -- 很重要，如果没有 -- 的话，那么命令变成创建分支了

删除文件
（1）rm test.txt  删除后使用commit命令提交后就从版本库中彻底删除了
（2）git checkout  -- test.txt   可以从版本库中恢复文件

git和github进行关联
（1）在github上创建新仓库，按照提示  git remote add origin https://github.com/...
（2）git push -u origin master 输入github的邮箱和密码   将当前分支推送到远程
    第一次推送分支时，加上 -u参数还会把本地的master分支和远程分支关联起来，
    之后只有本地提交，使用git push origin master即可
