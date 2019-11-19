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