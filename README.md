# GitHub Actions 使用玩具

### 一些概念

- workflow （工作流程）：持续集成一次运行的过程，就是一个 workflow。
- job （任务）：一个 workflow 由一个或多个 jobs 构成，含义是一次持续集成的运行，可以完成多个任务。
- step（步骤）：每个 job 由多个 step 构成，一步步完成。
- action （动作）：每个 step 可以依次执行一个或多个命令（action）。

### 存放位置与格式

- GitHub Actions 的配置文件叫做 workflow 文件，存放在代码仓库的.github/workflows 目录。
- workflow 文件采用 YAML 格式，GitHub 会自动运行.yml 文件

### 简单案例

[main 分支推送和拉取时触发下载 node 环境并打印 node 版本的 ci](https://github.com/szm8991/github-action-toy/blob/main/.github/workflows/simple.yml)

### 部署案例

[婷婷哥的 ci 参考-lint、typecheck、test](https://github.com/antfu/starter-ts/blob/main/.github/workflows/ci.yml)
