## 将本地项目上传GitHub
1. cd进入本地项目文件夹
2. 使用git init初始化git项目仓库
3. 将所有文件加入暂存区
```
git add .
```
4. 查看本地仓库状态
```
git status
```
5. 连接远程GitHub并创建仓库
6. 将本地仓库与远程仓库关联
```
git remote add origin git@github.com:ChHerman/learngit.git
```
7. 将本地项目推送到远程仓库，-f为强覆盖
```
git push -f
```

## Git常用命令
git config --global user.name "Your Name" 设置名称  
git config --global user.email "email@example.com" 设置邮箱  
git init 初始化Git仓库  
git add &lt;file&gt; 添加文件到暂存区  
git commit -m &lt;message&gt; 添加文件到Git仓库  
git status 显示Git仓库状态  
git diff 查看修改内容  
git reset --hard commit\_id 回退到commit\_id版本  
git reset --hard HEAD^ 回退到上一版本，^^表示上两个版本  
git log 查看提交历史  
git log -graph 查看分支合并图  
git reflog 查看命令历史  
git checkout -- file 丢弃工作区内容  
git reset HEAD &lt;file&gt; 撤销暂存区修改  
git rm file 删除文件  
git remote add origin git@server-name:path/repo-name.git 关联远程库  
git push -u origin master 第一次推送master分支所有内容  
git push origin master 推送最新修改  
git clone &lt;address&gt; 克隆远程仓库  
git branch 查看分支  
git branch &lt;name&gt; 创建分支  
git checkout &lt;name&gt;或者git switch &lt;name&gt; 切换分支  
git checkout -b &lt;name&gt;或者git switch -c &lt;name&gt; 创建+切换分支  
git merge &lt;name&gt; 合并某分支到当前分支，fast forward模式  
git merge --no-ff -m "merge with no-ff" &lt;branch-name&gt; 以普通模式合并分支，能看出曾经做过合并    
git branch -d &lt;name&gt; 删除分支
git branch -D &lt;name&gt; 强制删除分支，删除未合并分支  
git stash 保存现场  
git stash pop 回到工作现场  
git cherry-pick &lt;commit&gt; 把bug内容复制到当前分支
git remote -v 查看远程库信息  
git push origin branch-name 从本地推送分支  
git pull 抓取远程的新提交  
git checkout -b branch-name origin/branch-name 建立本地分支和远程分支的关联  
git rebase 把本地未push的分支提交历史整理成直线  
git tag &lt;tagname&gt; 新建一个标签  
git tag -a &lt;tagname&gt; -m "comment" 新建标签并指定标签信息  
git tag 列出所有标签  
git tag -d &lt;tagname&gt; 删除标签  
git push origin &lt;tagname&gt; 推送本地标签  
git push origin -tags 推送全部未推送本地标签  
git git push origin :refs/tags/&lt;tagname&gt; 删除远程标签
