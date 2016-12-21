1.git add  提交一个文件到暂存区
	git add README.txt

2.git commit 提交到仓库
	git commit -m "readme.txt文件提交"
	
3.git status 查看仓库状态


远程版本库
1.创建SSH key
	ssh-keygen -t rsa -C "yougensai@icloud.com"
	会在.shh目录下生产两个文件
	
2.github与 本地git同步
	git remote add origin https://github.com/WikiDown/git-push.git
	
3.push到github 
	git push -u origin master

查看当前所在分支
	git branch

查看remote使用的传输协议
	git remote -v
	
设置为ssh
	git remote rm origin
	git remote add origin git@github.com:username/repository.git
	git push -u origin master
	
如需简短命令使用 git push
需要配置: git config --global push.default simple
			or 
		  git config --global push.default matching 
		（前者只会提交当前所在分支，后者会提交本地所有分支）	
	

http://blog.csdn.net/u013647382/article/details/47832559	