<div align="center">

# SDU-Thesis-LaTeX

**山东大学本科毕业论文 LaTeX 模板**  
**Shandong University Undergraduate Thesis LaTeX Template**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![LaTeX](https://img.shields.io/badge/LaTeX-XeLaTeX-green.svg)](https://www.latex-project.org/)
[![Standard: GB/T 7714](https://img.shields.io/badge/Reference-GB%2FT%207714-orange.svg)](https://www.chinesestandard.net/default.aspx/GB/T7714-2015)
[![University](https://img.shields.io/badge/University-Shandong%20University-red.svg)](https://www.sdu.edu.cn)

</div>

---

## 目录 / Table of Contents

- [简介 / Introduction](#简介--introduction)
- [效果预览 / Preview](#效果预览--preview)
- [文件结构 / Repository Structure](#文件结构--repository-structure)
- [快速开始 / Quick Start](#快速开始--quick-start)
- [模板说明 / Template Documentation](#模板说明--template-documentation)
- [编译说明 / Compilation](#编译说明--compilation)
- [常见问题 / FAQ](#常见问题--faq)
- [贡献 / Contributing](#贡献--contributing)
- [许可证 / License](#许可证--license)

---

## 简介 / Introduction

### 中文

本项目提供山东大学本科毕业论文（设计）的非官方 LaTeX 排版模板，格式参照山东大学本科毕业论文写作规范，适用于**理科、工科**等专业的毕业论文撰写。

模板核心为 `sduthesis.cls` 自定义文档类，将所有格式设置封装其中，用户只需填写论文内容，无需关心底层排版细节。主文件 `main.tex` 包含详细的中文注释，适合 LaTeX 初学者参考学习。

**主要特性：**
- ✅ 符合山东大学本科毕业论文格式规范（页边距、字体、行距、页眉页脚）
- ✅ 参考文献遵循国家标准 **GB/T 7714-2015**，支持著者-年制与顺序编码制
- ✅ 支持中英文双语题注（`bicaption`）
- ✅ 内置代码高亮（`listings` / `minted`）、算法排版（`algorithm2e`）
- ✅ 图表自动编号（节号.图号 / 节号-表号）
- ✅ 目录、图目录、表目录自动生成
- ✅ 完整注释的 `main.tex`，每个宏包均有中文说明

### English

This project provides an **unofficial** LaTeX template for the Shandong University (SDU) undergraduate thesis, following the university's formatting guidelines. It is suitable for students in **science and engineering** programs.

The core of the template is the `sduthesis.cls` document class, which encapsulates all formatting rules. Users only need to fill in their thesis content without worrying about low-level typesetting details. The `main.tex` file is fully annotated in Chinese for easy reference.

**Key Features:**
- ✅ Complies with SDU undergraduate thesis formatting standards (margins, fonts, line spacing, headers/footers)
- ✅ Bibliography formatted to **GB/T 7714-2015** national standard; supports author-year and numerical citation styles
- ✅ Bilingual captions (Chinese + English) via `bicaption`
- ✅ Built-in code highlighting (`listings` / `minted`) and algorithm typesetting (`algorithm2e`)
- ✅ Automatic figure/table numbering (Section.Figure / Section-Table)
- ✅ Auto-generated table of contents, list of figures, and list of tables
- ✅ Fully annotated `main.tex` with per-package Chinese comments

---

## 效果预览 / Preview

> 封面 · 摘要 · 目录 · 正文 · 参考文献 · 致谢

![山东大学本科毕业论文_设计_模板_01](https://github.com/user-attachments/assets/89ab19ee-90f2-4a2a-a766-ae3d49287cda)
![山东大学本科毕业论文_设计_模板_02](https://github.com/user-attachments/assets/158d1a99-08d5-4958-9d1d-8e936937cdff)
![山东大学本科毕业论文_设计_模板_03](https://github.com/user-attachments/assets/3c5f6f02-1630-448a-8911-a408de4b95b7)
![山东大学本科毕业论文_设计_模板_04](https://github.com/user-attachments/assets/c6096976-1926-4c78-b384-2d96c52e6018)
![山东大学本科毕业论文_设计_模板_05](https://github.com/user-attachments/assets/31d00f98-b731-4a6b-9d30-2aeabe03311b)
![山东大学本科毕业论文_设计_模板_06](https://github.com/user-attachments/assets/9c8ec10a-9eab-46ca-bffb-4d6db83f3ade)
![山东大学本科毕业论文_设计_模板_07](https://github.com/user-attachments/assets/03b8d170-5511-41a1-a2c5-af8d080c48f4)
![山东大学本科毕业论文_设计_模板_08](https://github.com/user-attachments/assets/0dddace4-7b59-4c0d-bdb1-0c71da531092)
![山东大学本科毕业论文_设计_模板_09](https://github.com/user-attachments/assets/75ba9f70-e5f5-4139-b2d4-4e6f63676521)
![山东大学本科毕业论文_设计_模板_10](https://github.com/user-attachments/assets/c51cbea7-3cd1-402c-abda-39afcf72d87f)
![山东大学本科毕业论文_设计_模板_11](https://github.com/user-attachments/assets/20631782-5bf8-4b91-b5d6-1fda68fa3cd6)
![山东大学本科毕业论文_设计_模板_12](https://github.com/user-attachments/assets/c9878f59-0110-4691-8157-3b8c82ca505a)

---

## 文件结构 / Repository Structure

```
SDU-Thesis-LaTeX/
│
├── main.tex                   # 主文件（含详细注释）/ Main file (annotated)
├── ref.bib                    # 参考文献库 / Bibliography database
│
├── pic/
│   └── cover.jpg              # 封面校徽图片 / University logo for cover
│
├── cover/
│   └── cover_cyber.tex        # 封面内容 / Cover page content
│
├── abstractC/
│   └── abstractC.tex          # 中文摘要 / Chinese abstract
│
├── abstractE/
│   └── abstractE.tex          # 英文摘要 / English abstract
│
├── body/
│   ├── 1.tex   # 第一章 
│   ├── 2.tex          # 第二章 
│   └── ...                         # 其余章节 / Other chapters
│
├── acknowledge/
│   └── acknowledge.tex        # 致谢 / Acknowledgements
│
├── appendix/
│   └── appendix.tex           # 附录 / Appendix
│
└── README.md
```

---

## 快速开始 / Quick Start

### 中文

**1. 克隆仓库**

```bash
git clone https://github.com/your-username/SDU-Thesis-LaTeX.git
cd SDU-Thesis-LaTeX
```

**2. 修改论文信息**

打开 `main.tex`，填写你的论文元数据：

```latex
\thesistitle{你的论文题目}
\thesisauthor{你的姓名}
\thesisstuid{你的学号}
\thesiscollege{你的学院}
\thesisgrade{20XX}
\thesismajor{你的专业}
\thesissupervisor{指导老师\quad 职称}
\thesisdate{20XX}{月}{日}
\thesiscover{pic/cover.jpg}
```

**3. 编写各章节内容**

在 `body/` 目录下新建或修改各章节 `.tex` 文件，在 `main.tex` 中用 `\input{}` 引入。

**4. 编译**

按照以下顺序编译（共四次）：

```bash
xelatex main
bibtex  main
xelatex main
xelatex main
```

---

### English

**1. Clone the repository**

```bash
git clone https://github.com/your-username/SDU-Thesis-LaTeX.git
cd SDU-Thesis-LaTeX
```

**2. Fill in your thesis information**

Open `main.tex` and edit the metadata commands (see above).

**3. Write your chapter content**

Create or edit `.tex` files in the `body/` directory and include them via `\input{}` in `main.tex`.

**4. Compile**

Run the following commands in order:

```bash
xelatex main
bibtex  main
xelatex main
xelatex main
```

---

## 模板说明 / Template Documentation

### `sduthesis.cls` 主要命令

| 命令 | 说明 | Example |
|------|------|---------|
| `\thesistitle{}` | 中文论文题目 | `\thesistitle{海洋天然产物…}` |
| `\thesistitleen{}` | 英文论文题目 | `\thesistitleen{Marine Natural…}` |
| `\thesisauthor{}` | 作者姓名 | `\thesisauthor{张三}` |
| `\thesisstuid{}` | 学号 | `\thesisstuid{202200000001}` |
| `\thesiscollege{}` | 学院 | `\thesiscollege{计算机学院}` |
| `\thesisgrade{}` | 年级 | `\thesisgrade{2022}` |
| `\thesismajor{}` | 专业 | `\thesismajor{计算机科学与技术}` |
| `\thesissupervisor{}` | 指导老师 | `\thesissupervisor{李四\quad 教授}` |
| `\thesisdate{}{}{}` | 论文日期（年/月/日） | `\thesisdate{2026}{5}{1}` |
| `\thesiscover{}` | 封面图片路径 | `\thesiscover{pic/cover.jpg}` |
| `\makecover` | 生成封面页 | — |
| `\makefrontmatter` | 生成目录页（摘要后调用） | — |
| `\makebibliography{}` | 生成参考文献（传入 .bib 文件名） | `\makebibliography{ref}` |

### 文档类选项

```latex
\documentclass[<选项>]{sduthesis}
```

| 选项 | 说明 |
|------|------|
| `science`（默认） | 理科论文 |
| `engineering` | 工科论文 |
| `lof` | 生成图目录（List of Figures） |
| `lot` | 生成表目录（List of Tables） |
| `lol` | 生成代码目录（List of Listings） |

### 摘要与致谢环境

```latex
% 中文摘要
\begin{abstractC}{}
  摘要正文……
  \ckeywords{关键词1；关键词2；关键词3}
\end{abstractC}

% 英文摘要
\begin{abstractE}
  Abstract content...
  \ekeywords{Keyword1; Keyword2; Keyword3}
\end{abstractE}

% 致谢
\begin{acknowledge}
  致谢内容……
\end{acknowledge}
```

---

## 编译说明 / Compilation

### 环境要求 / Requirements

| 工具 | 版本建议 | 说明 |
|------|----------|------|
| TeX 发行版 | TeX Live 2022+ 或 MiKTeX | 推荐 TeX Live |
| 编译引擎 | **XeLaTeX** | 必须，支持中文与系统字体 |
| 字体 | Times New Roman | 需已安装于操作系统 |
| Python（可选） | 3.x + pygments | 使用 `minted` 时需要 |

### 编辑器推荐 / Recommended Editors

- **VS Code** + LaTeX Workshop 插件（推荐，可配置一键编译）
- **Overleaf**（在线，需上传全部文件）
- **TeXstudio** / **TeXworks**

### Overleaf 使用说明

1. 将整个仓库打包为 `.zip` 文件上传至 Overleaf
2. 在 Overleaf 设置中将编译器改为 **XeLaTeX**
3. 确保上传了 Times New Roman 字体文件（`.ttf`），或改用 Overleaf 内置的 `libertinus` 等字体

---

## 常见问题 / FAQ

**Q：编译报错 `fontspec error: "font-not-found"` 怎么办？**  
A：系统未安装 Times New Roman 字体。Windows 用户通常已预装；macOS/Linux 用户需手动安装或将 `main.tex` 中 `\setmainfont{Times New Roman}` 改为其他已安装字体（如 `\setmainfont{TeX Gyre Termes}`）。

**Q：中文显示为方块或乱码？**  
A：请确认使用的是 **XeLaTeX** 而非 pdfLaTeX 或 LaTeX 编译。

**Q：参考文献不显示或格式不对？**  
A：检查是否按照 `xelatex → bibtex → xelatex → xelatex` 顺序编译了四次。

**Q：目录中章节标题出现乱码？**  
A：通常由 `tocloft` 与 `ctex` 冲突引起，模板已内置修复，若仍出现请提 Issue。

**Q：如何切换为顺序编码制（数字引用）？**  
A：将 `main.tex` 中的  
`\usepackage[authoryear,square]{gbt7714}`  
改为  
`\usepackage[numerical,square]{gbt7714}`

---

## 贡献 / Contributing

欢迎提交 Issue 或 Pull Request！

If you find any bugs or have suggestions for improvement, feel free to open an Issue or submit a Pull Request.

1. Fork 本仓库
2. 新建分支 `git checkout -b feature/your-feature`
3. 提交更改 `git commit -m 'Add some feature'`
4. 推送分支 `git push origin feature/your-feature`
5. 提交 Pull Request

---

## 许可证 / License

本项目基于 [MIT License](LICENSE) 开源，可自由使用、修改与分发。  
This project is licensed under the [MIT License](LICENSE) — free to use, modify, and distribute.

---

<div align="center">

Made with ❤️ for SDU students · 为山大学子而作

</div>
