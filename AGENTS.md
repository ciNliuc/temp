# 工作约定

这个目录是一个 GitHub 仓库（`ciNliuc/temp`）的本地克隆，你会在这里接需求、改代码、提交和开 PR。

## 接一个需求时怎么做

1. 先看现状：`git status`、`git log --oneline -5`、`git fetch origin`，确认工作区干净、`main` 是最新的。
2. 从 `main` 开新分支，命名 `agent/<简短英文描述>`，例如 `agent/fix-readme-typo`。**不要直接改 `main`。**
3. 改完自己验证一遍（读回文件确认改动真的生效，能跑就跑一下）。
4. 提交，信息用英文、一句话说清改了什么，例如 `docs: append hello line to README`。
5. 推送：`git push -u origin agent/<描述>`。凭据已经配好，直接推即可。
6. 开 PR：`gh pr create --title "<同一句话>" --body "<为什么改、改了什么>"`。
   `gh` 已登录为 `BLUEYOOO0318`，直接可用。
7. 回到发需求的地方，一句话说结果 + 贴 PR 链接。

## 硬性约束

- **不要自己合并 PR**，等人审。也不要 force push、不要删别人的分支。
- 一次只做一件被明确要求的事。没被要求就不要顺手重构、不要改无关文件。
- 需求不清楚就先问一句，别猜着做。
- 报错就把错误原文说出来，不要编造成功。

## 环境

- 仓库根目录：`/Users/zhengke/src/temp`
- `git` 已配置凭据，`gh` 已登录，可直接 push 和开 PR
- 分支前缀统一用 `agent/`
