## Git 的最基本的工作模型
* 从 GitHub 把中央仓库 clone 到本地（使用命令： git clone）
* 把写完的代码提交（先用 git add 文件名 把文件添加到暂存区，再用 git commit交）
    > 在这个过程中，可以使用 git status 来随时查看工作目录的状态
    > 每个文件有 "changed / unstaged"（已修改）, "staged"（已修改并暂存）, "commited"（已提交） 三种状态，以及一种特殊状态"untracked"（未跟踪）
* 提交一次或多次之后，把本地提交 push 到中央仓库（git push）


## 基本指令
- git log 查看历史提交记录 键盘英文状态下按字母q，退出git log
- git status 随时查看工作目录的状态
- git clone '地址' 下拉到本地
- git add 文件名 把文件添加到暂存区
- git commit -m 'xxx' 提交
- git push -u origin master 提交到中央仓库
Creating a new branch is quick and simple.
