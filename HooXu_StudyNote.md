PR尝试功能尝试，本次PR实验结果提交见文档下。

## 练习内容：

PR项目练习，将下述项目Fork到本地，并PR更新，[Git项目]( https://github.com/2951121599/repo_for_test_pr) ，参考 [知乎 - PR教程](https://zhuanlan.zhihu.com/p/370512818)。

Step 1: 在Git中Fork项目

```shell
# 同步Git项目 将本地develop项目和远程main项目同步
$ git add .

$ ls
README.md lecture08

$ git init
Reinitialized existing Git repository in repo_for_test_pr/.git/

$ git commit -m 'init'
On branch main
Your branch is up to date with 'origin/main'.
nothing to commit, working tree clean

$ git checkout -b develop main
```

Step 2: 修改项目内容并合并

```shell
$ touch LoginUser.html

$ echo "hi, this is user html" > LoginUser.html

$ git add .

$ git commit -m "feat: add LoginUser.html"

$ git status

$ git push --set-upstream origin develop

$ git checkout main

# 合并并删除
$ git merge --no-ff develop

$ git branch -d develop
```

Step 3：PR提交

![PIC 4_01](https://raw.githubusercontent.com/ShawnHoo7256/faster-git/Datawhale202205/StudyNotes/figures/PIC%204_01.png)

![PIC 4_02](https://raw.githubusercontent.com/ShawnHoo7256/faster-git/Datawhale202205/StudyNotes/figures/PIC%204_02.png)

![PIC 4_03](https://raw.githubusercontent.com/ShawnHoo7256/faster-git/Datawhale202205/StudyNotes/figures/PIC%204_03.png)

