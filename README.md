# Paper

该仓库已加入一套可用于 Codex 进行论文 LaTeX 写作的基础环境配置。

## 已配置内容

- 新增 `.github/workflows/copilot-setup-steps.yml`
- 在 Copilot/Codex 会话启动前预装：
  - `latexmk`
  - `texlive-latex-base`
  - `texlive-latex-extra`
  - `texlive-fonts-recommended`
  - `texlive-xetex`
  - `texlive-lang-chinese`
  - `biber`
- 安装后自动执行版本检查，确保工具可用。

## 使用方式

1. 将上述 workflow 合并到默认分支。
2. 在仓库 Actions 中可手动触发 **Copilot Setup Steps** 验证安装。
3. 之后使用 Codex 在本仓库进行 LaTeX 论文编写时，会先执行该环境准备步骤。
