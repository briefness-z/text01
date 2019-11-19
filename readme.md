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