# 1. 配置用户信息
在开始使用 Git 之前，通常需要设置你的用户名和邮箱：
```bash
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

# 2. 创建和克隆仓库
- **创建新的 Git 仓库**：
  ```bash
  git init
  ```

- **克隆现有仓库**：
  ```bash
  git clone <repository-url>
  ```

# 3. 查看状态
- **查看当前工作目录和暂存区的状态**：
  ```bash
  git status
  ```

# 4. 添加和提交更改
- **将更改添加到暂存区**：
  ```bash
  git add <file>
  ```
  - 添加所有更改：
    ```bash
    git add .
    ```

- **提交更改**：
  ```bash
  git commit -m "Commit message"
  ```

# 5. 查看提交历史
- **查看提交记录**：
  ```bash
  git log
  ```

- **查看简洁的提交历史**：
  ```bash
  git log --oneline
  ```

# 6. 分支管理
- **查看所有分支**：
  ```bash
  git branch
  ```

- **创建新分支**：
  ```bash
  git branch <branch-name>
  ```

- **切换到另一个分支**：
  ```bash
  git checkout <branch-name>
  ```
  - 创建并切换到新分支（简写）：
    ```bash
    git checkout -b <branch-name>
    ```

- **删除分支**：
  ```bash
  git branch -d <branch-name>
  ```

# 7. 合并分支
- **将一个分支合并到当前分支**：
  ```bash
  git merge <branch-name>
  ```

# 8. 远程仓库管理
- **查看远程仓库**：
  ```bash
  git remote -v
  ```

- **添加远程仓库**：
  ```bash
  git remote add <remote-name> <repository-url>
  ```

- **推送更改到远程仓库**：
  ```bash
  git push <remote-name> <branch-name>
  ```

- **从远程仓库拉取更改**：
  ```bash
  git pull <remote-name> <branch-name>
  ```

- **获取远程仓库的更新**（不合并）：
  ```bash
  git fetch <remote-name>
  ```

# 9. 撤销操作
- **撤销暂存区的更改**：
  ```bash
  git reset <file>
  ```

- **撤销对工作目录的更改**（恢复到最后一次提交状态）：
  ```bash
  git checkout -- <file>
  ```

- **撤销最近的提交，但保留更改**：
  ```bash
  git reset HEAD~1
  ```

# 10. 标签管理
- **创建标签**：
  ```bash
  git tag -a <tag-name> -m "Tag message"
  ```

- **查看标签**：
  ```bash
  git tag
  ```

- **推送标签到远程**：
  ```bash
  git push <remote-name> <tag-name>
  ```