# ============================================
# 完整的 Git 文件上传流程
# ============================================

# 第1步：查看当前状态，确认哪些文件未被跟踪
git status

# 第2步：添加你要上传的文件（三种方式任选其一）

# 方式A：添加单个文件
git add 文件名.txt

# 方式B：添加多个文件
git add 文件1.txt 文件2.txt

# 方式C：添加所有未跟踪和修改的文件
git add .

# 第3步：提交文件到本地仓库
git commit -m "添加新文件的说明"

# 第4步：查看远程仓库配置
git remote -v

# 第5步：推送到 GitHub
git push

# 如果是第一次推送或者没有设置上游分支，使用：
git push -u origin master
# 或者（如果你的远程仓库名是 km_plot_analysis）
git push -u km_plot_analysis master
