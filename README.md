# 李昕潼中文简历（LaTeX）

该仓库用于通过 GitHub 与 Overleaf 同步维护简历。

## Overleaf 使用方法

1. 在 Overleaf 中选择 **New Project → Import from GitHub**。
2. 选择本仓库 `licns657/CV`。
3. 将编译器设为 **XeLaTeX**，主文档设为 `main.tex`。
4. 已关联本仓库的项目，需要使用 GitHub 同步中的 Pull 操作拉取更新，再重新编译。

## 文件

- `main.tex`：中文简历正文。
- `assets/resume_photo.png`：简历证件照。
- `.latexmkrc`：默认使用 XeLaTeX 的编译配置。

模板仅使用 Overleaf/TeX Live 中的常见宏包，并采用 Fandol 中文字体，避免依赖本机字体。
Overleaf 无需另行安装中文字体或宏包；项目设置中的编译器请选择 XeLaTeX。
