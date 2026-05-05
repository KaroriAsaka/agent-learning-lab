# Repository Setup

当前本地项目路径：

```text
/Users/autumn/PycharmProjects/agent-learning-lab
```

## 推荐 GitHub 仓库名

```text
agent-learning-lab
```

建议长期学习仓库设置为 private，等内容成熟后再考虑公开。

当前远程仓库：

```text
https://github.com/KaroriAsaka/agent-learning-lab
```

## 如果你之后安装了 GitHub CLI

```bash
brew install gh
gh auth login
cd /Users/autumn/PycharmProjects/agent-learning-lab
gh repo create agent-learning-lab --private --source=. --remote=origin --push
```

## 如果你手动创建 GitHub 仓库

在 GitHub 页面创建一个空仓库：

```text
agent-learning-lab
```

然后在本地执行：

```bash
cd /Users/autumn/PycharmProjects/agent-learning-lab
git remote add origin git@github.com:KaroriAsaka/agent-learning-lab.git
git push -u origin main
```

## 推上 GitHub 后

可以把 `tasks/github-issues.md` 里的每个条目创建成 issue。
