# 仓库上传github  使用终端 Git Bash

# 1. 进入 finance_cli 目录

cd finance_cli

# 2. 初始化独立的 git 仓库

git init

# 3. 添加所有文件并提交

git add *
git commit -m "first commit"

# 4. 重命名分支为 main（如果默认是 master）

git branch -M main

# 5. 创建仓库 关联远程仓库（替换成你的仓库地址）

git remote add origin https://github.com/你的用户名/finance_cli.git

# 6. 推送

git push -u origin main

# 若github上传失败 去Clash找代理端口号6666

git config --global http.proxy http://127.0.0.1:6666

git config --global https.proxy http://127.0.0.1:6666

git push -u origin main

# 日常更新三步曲

git add *
git commit -m "描述这次改了什么"
git push
