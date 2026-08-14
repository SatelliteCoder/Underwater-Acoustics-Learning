# GitHub 发布指南

本目录已经初始化为 Git 仓库。推荐仓库名：

```text
Underwater-Acoustics-Learning
```

## 首次提交

```bash
git add .
git commit -m "init underwater acoustics learning resources"
```

## 创建 GitHub 远程仓库

如果你使用 GitHub CLI：

```bash
gh repo create Underwater-Acoustics-Learning --public --source=. --remote=origin --push
```

如果你在网页端创建仓库：

```bash
git remote add origin https://github.com/<your-name>/Underwater-Acoustics-Learning.git
git branch -M main
git push -u origin main
```

## 推荐仓库设置

- Description：A curated learning platform for underwater acoustics, sonar, ocean acoustic propagation, underwater communication, and passive acoustic monitoring.
- Topics：`underwater-acoustics`, `ocean-acoustics`, `sonar`, `acoustic-propagation`, `underwater-communication`, `passive-acoustic-monitoring`, `bellhop`, `kraken`
- Website：可暂时留空，后续如果做 GitHub Pages 再补。
- Issues：开启，用于收集新资源。
- Discussions：可选，适合后续做论文/源码阅读讨论。

## 维护节奏

建议按月维护：

- 检查外部链接是否失效。
- 给新增项目补许可证和学习价值。
- 每月精读 1 个重点项目并添加源码阅读笔记。
- 将“待补充方向”逐步拆成独立页面。

