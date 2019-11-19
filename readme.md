一
git config --global user.name ""
git config --global user.email ""
第二次
git add ./    提交文件路径
git commit -m "说明信息"
第三步
git status 查询当前储仓状态  出现modified （红色：文件项目修改，但未提交仓库 ，绿色：已保存提交，但未说明） 
第四步
git add ./    提交全部文件
git commit --all -m   --all:提交全部文件夹  -m：说明  （一次性完成）
第五步
git log   打印详细修改日志记录
git log --oneline   打印简洁修改日志记录
第六步
git reset --hard Head~0  回到上一次代码文件的状态 0上一级   1上两级 ....
git reset --hard xxxxxxx（版本号）  回到指定位置状态，先git log --oneline 再git reset --hard 52fb501  ==回到第六步    
el:$ git log --oneline
	52fb501 (HEAD -> master) 第六步
	ba286dd 第四步更新
	6b3e035 第四步+registry.html
	8d57404 第四次修改
	0349e3b 第三步
	b246091 第二步
	0bbb89e 完成第一步
版本号是唯一的，可以前后切换
第七步
git reflog  打印历史所有的操作记录
第八步
git branch 名字   创建分支，分支名字
git branch   查看分支结构
git checkout 名字   切换分支路线
切换分支后其他人无法访问分支，只有合并分支
第九步
git merge 分支名字     合并分支
git branch -d 分支名字    删除分支
***代码提交到GitHub上
  列：git push https://github.com/briefness-z/text01.git master
 ****下拉代码
 创建文件夹，初始化仓储，git pull
 git pull  地址  分支