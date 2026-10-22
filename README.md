# 李昕潼中文简历（LaTeX）

该仓库用于通过 GitHub 与 Overleaf 同步维护简历。

当前为一页中文版，排版改编自 [billryan/resume](https://github.com/billryan/resume)。
保留其黑白分节、FontAwesome 图标、姓名与联系方式居中、经历日期右对齐的样式，
并针对中文及一页长度调整字体、间距与照片布局。
模板宏内嵌于 `main.tex`，方便单文件编辑器编译；无需外部 `resume.cls`。
原模板许可证见 `TEMPLATE-LICENSE`，其许可范围不涉及个人简历正文与证件照。

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
英文字体使用 TeX Gyre Termes，联系方式使用 TeX Gyre Heros；无需 Adobe 字体。
Overleaf 无需另行安装中文字体或宏包；项目设置中的编译器请选择 XeLaTeX。

## 简历版本与切换

- `main.tex`：原版简历，保留原有内容与排版。
- `cv_codeagent_minionerec.tex`：Code Agent 算法方向与 MiniOneRec 生成式推荐项目版本（2026-10-22）。
- `cv_codeagent_cookiebench.tex`：Code Agent 与 Cookie-Bench 网页交互质量评测版本（2026-10-22）；Cookie-Bench 标为复现进行中。

三个文件都是可以独立编译的完整简历，共用 `assets/resume_photo.png`。更新任一版本时，编辑对应文件即可。

在已关联本仓库的 Overleaf 项目中，使用 GitHub 同步的 Pull 拉取更新，然后在项目设置的 **Main document（主文档）** 中选择要使用的 `.tex` 文件，编译器使用 **XeLaTeX**。切换主文档不会删除其他版本。

三个文件用于并行维护；Git 提交记录或 Overleaf History 标签用于回溯每个版本的修改。
