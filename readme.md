## Git 的最基本的工作模型
* 从 GitHub 把中央仓库 clone 到本地（使用命令： git clone）
* 把写完的代码提交（先用 git add 文件名 把文件添加到暂存区，再用 git commit交）
    - 在这个过程中，可以使用 git status 来随时查看工作目录的状态
    - 每个文件有 "changed / unstaged"（已修改）, "staged"（已修改并暂存）, "commited"（已提交） 三种状态，以及一种特殊状态"untracked"（未跟踪）
* 提交一次或多次之后，把本地提交 push 到中央仓库（git push）
### 基本操作
1. git clone '仓库地址'
2. git add 文件名
3. git commit -m '介绍说明'
4. git push -u origin branch_name


## 多人合作的基本工作模型
1. 多人从Github吧中央仓库clone到自己机器(本地)上（使用命令： git clone）
2. 同事 commit 代码到他的本地，并 push 到 GitHub 中央仓库
3. 你也可以把自己的 commit 代码到他的本地，并 push 到 GitHub 中央仓库
    - 如果你的同事比你先push到GitHub中央仓库，也就是说GitHub中央仓库有你本地仓库没有的commits,此时你需要先pull把远端仓库上的新内容取回到本地和本地合并，然后再把合并后的本地仓库向远端仓库推送
    - 如果 push 失败，就用 pull 把本地仓库的提交和中央仓库的提交进行合并，然后再 push 一次
### 基本操作
1. 同事一：git clone '仓库地址'

   同事二：git clone '仓库地址'

   ...

2. 同事一：git add 文件名
          git commit -m '介绍说明'
          git push -u origin branch_name

3. 自己：git pull origin branch_name
         git add 文件名
         git commit -m '介绍说明'
         git push -u origin branch_name


## 基本指令
- git log 查看历史提交记录 键盘英文状态下按字母q，退出git log
- git status 随时查看工作目录的状态
- git clone '地址' 下拉到本地
- git add 文件名 把文件添加到暂存区
- git commit -m 'xxx' 提交
- git push -u origin master 提交到中央仓库

