# Git

在 [OI-Wiki](https://oi-wiki.org/tools/git/) 中有对于 Git 的详细介绍，但笔者认为这些介绍过于复杂了，所以在这里简短介绍一下 Git。

> Git 可以在集成了 Git 的 IDE 中使用，也可以在命令行中使用。对于命令行的使用可以参考：[命令行](../../Common/Tool/Command-Line.md)

## Git 简介

Git 是一个分布式版本控制系统，广泛用于源代码管理和协作开发。它允许多个开发者在同一项目上并行工作，同时跟踪和管理代码的历史更改。

### [Git 下载](https://git-scm.com/downloads)

> 下载完就可以直接在命令行/IDE 里运行 Git 命令了

### 常用命令

* `git init`：初始化一个新的 Git 仓库。
* `git clone <repository>`：克隆一个远程仓库到本地。
* `git add <file>`：将文件添加到暂存区。
* `git commit -m "message"`：提交更改并添加提交信息。
* `git push`：将本地提交推送到远程仓库。
* `git pull`：从远程仓库获取并合并更改。
* `git branch`：查看或管理分支。
* `git merge <branch>`：合并指定分支到当前分支。

> 详细的用法可以参考 [Git 的常用命令](../../Common/Command/Git.md)

### Git 与 GitHub

```
echo "# example" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/Freakz3z/example.git
git push -u origin main
```

### 使用场景

* **软件开发**：广泛用于开源和商业软件项目的版本控制。
* **文档管理**：用于管理文档版本和变更。
* **团队协作**：支持多个开发者在同一项目上工作的工具。
