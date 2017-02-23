主要是用来总在在学习使用git过程中使用到的命令行！

#在进行任务git操作之前都要先切换到git仓库
#git init 初始化本地仓库 
#git status 查看仓库状态: 
#git add <file> 将文件添加到暂存区（并没有真正的提交，可以被移除）
#git rm --cached 将移除暂存区的缓存
git commit -m 'first commit' 提交并配置提交信息
git log 查看所有产生的 commit 记录
git branch 查看下当前分支情况
git branch a  新建了一个名字叫 a 的分支
git checkout a  切换到a分支
git checkout -b a  新建一个a分支，并且自动切换到a分支
git merge a 合并分支，注意：要先切到要合并的分支上，比如主干合并分支a，就先切到主干上
git branch -d a 删除a分支
git branch -D a 强制删除a分支
git tag v1.0 新建一个标签
git tag 查看历史 tag 记录
git checkout v1.0  切换到 v1.0 tag

ssh-keygen -t rsa 指定 rsa 算法生成密钥，用于与github进行匹配！
ssh -T git@github.com  测试匹配是否成功
git push origin master 把本地代码推到远程仓库，注意这个origin是可以变的
git pull origin master  更新远程仓库的代码到本地仓库
git clone git@github.com:stormzhang/test.git 把 test 项目 clone 到了本地

git remote add origin git@github.com:stormzhang/test.git 添加一个远程仓库，origin 是给这个项目的远程仓库起的名字，这个名字和
git push origin master、git pull origin master名字是相对应的！为什么要给远程仓库取名字？因为我们可能一个项目有多个远程仓库？比如 GitHub 一个，比如公司一个，这样的话提交到不同的远程仓库就需要指定不同的仓库名字了。

git remote -v 查看我们当前项目有哪些远程仓库
