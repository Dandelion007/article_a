# github

mkdir test创建一个空目录  

git init命令把目录变成Git可以管理的仓库

git add 文件名            把文件添加到仓库：

git add readme.txt

git commit -m文件名           把文件提交到仓库（-m后面输入的是本次提交的说明，可以输入任意内容，简单解释一下git commit命令）

git commit命令执行成功后会告诉你，1 file changed：1个文件被改动（我们新添加的readme.txt文件）；2 insertions：插入了两行内容（readme.txt有两行内容）。

git push                 推送分支

rm read.txt              从版本库中删除

git branch                创建分支

git checkout              切换分支

git checkout master        切换回master分支

git merge dev          合并指定分支到当前分支

git branch -d dev         删除分支

 