学习git：
*以下的file都实指文件名称
1.版本修改可以用git reset --hard HEAD^ //--hard是上一个版本的已提交内容，--soft是上个版本已添加但未提交的内容，--mixed是未添加内容
2.找不到版本号的时候用git reflog
3.当第一次修改后add，第二次修改，commit，只会有第一次的修改在文件里面。
4.git diff HEAD -- file  可以查看工作区和版本库里面最新版本的区别
5.git checkout -- file 可以丢弃工作区的修改
6.git reset HEAD file 可以把暂存区的修改撤销掉（unstage），重新放回工作区
7.New-Item -Path file -ItemType File来创建一个新的文件
8.rm file 来删除文件
9.git checkout其实是用版本库里的版本替换工作区的版本，无论工作区是修改还是删除，都可以“一键还原”。
10.git push 直接推送 //前提：你已经 git push -u origin main 建立过关联
11.在10的操作后，每次文件进行了提交都可以用git push origin main，把本地main的分支推送道github
12.（很重要），每次编辑完文本要进行crtl+s进行保存，否则在powershell里面的添加和提交将没有意义。
13.当在校园网、公司网络等环境下，22 端口很可能会被防火墙策略屏蔽，这时测试ssh连接：ssh -T git@github.com ,然后找deepseek要代码
14.以后克隆远程库只能用https克隆（因为我的电脑用户名是中文，是非ASCII）公式：git clone https://github.com/用户名/仓库名.git
15.看完log，处在分页器阶段，按q退出分页器
16.git checkout命令加上-b参数表示创建并切换分支
17.用git branch命令查看当前分支
18.git merge命令用于合并指定分支到当前分支
19.git branch -d 分支 表示删除分支 //git branch 表示创建一个分支，用git checkout 切换到那个分支
20.git checkout <branch> 切换分支
21.git switch -c <branch> 也可以表示创建并切换到这一个分支

test