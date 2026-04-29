<div align="center">

<img src="pic/cover.jpg" alt="Shandong University" width="400"/>

# SDU-Thesis-LaTeX

**山东大学本科毕业论文（设计）LaTeX 模板**

**An Unofficial LaTeX Template for SDU Undergraduate Thesis**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![XeLaTeX](https://img.shields.io/badge/Compiler-XeLaTeX-green.svg)](https://tug.org/xetex/)
[![ctex](https://img.shields.io/badge/Package-ctex-red.svg)](https://ctan.org/pkg/ctex)
[![GB/T 7714](https://img.shields.io/badge/Reference-GB%2FT%207714--2015-orange.svg)](https://www.chinesestandard.net/default.aspx/GB/T7714-2015)

</div>

---

## 简介 | Introduction

### 中文

本项目是**山东大学本科毕业论文（设计）的非官方 LaTeX 模板**，格式严格对照山东大学本科毕业论文写作规范制作。

> ⚠️ **为什么要做这个模板？**
> Overleaf 和 TeXPage 上现有的山大毕业论文模板存在不同程度的错误，包括：中文标点全半角混乱、`tocloft` 与 `ctex` 目录冲突导致编译报错、`bicaption` 双语题注配置异常等，**实测无法直接编译通过**。本模板从零整理，修复了上述全部已知问题，开箱即用。

模板以 `main.tex` 为核心入口，所有格式设置均在其中完成，**每一个宏包都附有详细的中文注释**，适合 LaTeX 初学者边用边学。

### English

This is an **unofficial LaTeX template** for the Shandong University (SDU) undergraduate thesis, strictly following the university's formatting guidelines.

> ⚠️ **Why this template?**
> Existing SDU thesis templates on Overleaf and TeXPage contain various bugs — including mixed Chinese punctuation styles, compilation failures caused by `tocloft`/`ctex` conflicts, and broken `bicaption` bilingual caption configurations — making them **unusable out of the box**. This template was built from scratch with all known issues fixed.

The template is centered around `main.tex`, which contains detailed Chinese annotations for every package, making it beginner-friendly.

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

## 文件结构 | Repository Structure

```
SDU-Thesis-LaTeX/
│
├── main.tex                     # 主文件，含所有格式配置与详细中文注释
│                                # Main file with full formatting & per-package annotations
├── ref.bib                      # 参考文献数据库 | Bibliography database
├── gbt7714-numerical.bst        # GB/T 7714 顺序编码制样式文件
│                                # GB/T 7714 numerical citation style file
│
├── pic/
│   └── cover.jpg                # 封面校徽图片 | University logo for cover page
│
├── cover/
│   └── cover_cyber.tex          # 封面页（填写姓名、学号、专业等）
│                                # Cover page — fill in your name, ID, major, etc.
├── abstractC/
│   └── abstractC.tex            # 中文摘要 | Chinese abstract
│
├── abstractE/
│   └── abstractE.tex            # 英文摘要 | English abstract
│
├── body/
│   ├── 1.tex                    # 第一章示例 | Chapter 1 sample
│   └── 2.tex                    # 第二章示例 | Chapter 2 sample
│
├── acknowledge/
│   └── acknowledge.tex          # 致谢 | Acknowledgements
│
└── appendix/
    └── appendix.tex             # 附录 | Appendix
```

---

## 格式规范 | Formatting Specifications

| 项目 | 规范 |
|------|------|
| 纸张 | A4 |
| 页边距 | 上下 2.5 cm，左右 3 cm |
| 正文字号 | 小四（12 pt） |
| 英文字体 | Times New Roman |
| 行间距 | 1.5 倍行距 |
| 页眉 | 居中"山东大学本科毕业论文（设计）"，小五字号，0.6 pt 横线 |
| 前置页码 | 罗马数字（Ⅰ、Ⅱ、Ⅲ……） |
| 正文页码 | 阿拉伯数字（1、2、3……） |
| 一级标题 | 黑体，三号，加粗 |
| 二级标题 | 黑体，四号，加粗 |
| 三级标题 | 黑体，小四，加粗 |
| 图编号 | 节号.图号（如 图 2.1） |
| 表编号 | 节号-表号（如 表 2-1） |
| 题注字体 | 五号 Times New Roman |
| 参考文献 | GB/T 7714-2015，著者-年制，五号宋体 |
| 中文标点 | 全角（`\punctstyle{quanjiao}`） |

---

## 快速开始 | Quick Start

### 第一步：获取模板 | Get the Template

```bash
git clone https://github.com/your-username/SDU-Thesis-LaTeX.git
cd SDU-Thesis-LaTeX
```

### 第二步：填写个人信息 | Fill in Your Information

打开 `cover/cover_cyber.tex`，将占位符替换为您的真实信息：

```latex
\textbf{\kaishu 姓\qquad 名} & 你的姓名 \\    % → 替换为真实姓名
\textbf{\kaishu 学\qquad 号} & 你的学号 \\    % → 替换为真实学号
\textbf{\kaishu 学\qquad 院} & 你的学院 \\    % → 替换为所在学院
\textbf{\kaishu 年\qquad 级} & 你的年级 \\    % → 如：2022 级
\textbf{\kaishu 专\qquad 业} & 你的专业 \\    % → 替换为专业名称
\textbf{\kaishu 指导老师}    & 你的指导老师 \\ % → 如：张三\quad 教授
```

同时修改封面中的**论文题目**和**日期**（年/月/日）。

### 第三步：撰写各章内容 | Write Your Chapters

在 `body/` 目录下编辑章节文件，并在 `main.tex` 中用 `\input{}` 引入：

```latex
\newpage\input{"body/1.tex"}   % 第一章
\newpage\input{"body/2.tex"}   % 第二章
% 根据实际章节数量增减
```

### 第四步：编译 | Compile

**必须使用 XeLaTeX**，完整编译须执行四次以正确生成目录与参考文献：

```bash
xelatex main
bibtex  main
xelatex main
xelatex main
```

---

## 主要特性 | Key Features

- ✅ **中文全角标点** — `\punctstyle{quanjiao}` 强制全角，彻底解决半角标点混入问题
- ✅ **双语图表题注** — `bicaption` 宏包，`\bicaption{中文题注}{English caption}` 一行搞定
- ✅ **代码高亮** — 内置 `listings`（支持 Python / JSON）与 `minted` 双方案
- ✅ **算法排版** — `algorithm2e`，支持带框、带行号、带结构竖线的算法浮动体
- ✅ **矢量绘图** — `tikz` + `positioning` 库，直接在 `.tex` 中绘制流程图/结构图
- ✅ **国标参考文献** — `gbt7714` 宏包，附带 `.bst` 文件，同时支持著者-年制与顺序编码制
- ✅ **三级目录自动生成** — 含图目录、表目录、代码目录（注释一行即可开启）
- ✅ **每包详细注释** — `main.tex` 中每个 `\usepackage` 均有中文说明，适合 LaTeX 新手

---

## 切换引用格式 | Switching Citation Style

模板默认使用**著者-年制**（如 `[Smith, 2020]`）。

如需切换为**顺序编码制**（如 `[1]`），修改 `main.tex` 中的以下一行：

```latex
% 默认：著者-年制
\usepackage[authoryear, square]{gbt7714}

% 修改为：顺序编码制
\usepackage[numerical, square]{gbt7714}
```

---

## 环境要求 | Requirements

| 工具 | 要求 | 备注 |
|------|------|------|
| TeX 发行版 | TeX Live 2022+ 或 MiKTeX | 推荐 TeX Live |
| 编译引擎 | **XeLaTeX** | 必须，不支持 pdfLaTeX |
| 英文字体 | Times New Roman | 需已安装于操作系统 |
| Python（可选） | 3.x + `pygments` | 使用 `minted` 代码高亮时需要；编译须加 `-shell-escape` 参数 |

### 推荐编辑器 | Recommended Editors

| 编辑器 | 说明 |
|--------|------|
| **VS Code** + [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) | 推荐。配置 `xelatex` 编译链后可一键构建 |
| **TeXstudio** | 开箱即用。Options → Build → Default Compiler 改为 XeLaTeX |
| **Overleaf** | 在线使用。上传全部文件后，Menu → Compiler → 选 **XeLaTeX** |
| **TeXPage** | 同 Overleaf，上传后切换编译器为 XeLaTeX |

---

## 常见问题 | FAQ

**Q：报错 `fontspec error: "font-not-found"`？**

A：系统未安装 Times New Roman。Windows 通常已预装；macOS / Linux 用户请手动安装，或将 `main.tex` 中的字体声明替换为免费替代：
```latex
\setmainfont{TeX Gyre Termes}   % 已内置于 TeX Live，效果与 Times 相近
```

**Q：中文显示为方块或乱码？**

A：请确认使用的是 **XeLaTeX**，而非 pdfLaTeX 或普通 LaTeX 编译。

**Q：参考文献不显示，或格式不正确？**

A：请严格按顺序执行完整的四步编译：`xelatex → bibtex → xelatex → xelatex`。

**Q：目录出现 `??` 或页码全为 0？**

A：同上，通常只执行了一次编译导致。完整四步编译后即可解决。

**Q：如何开启图目录和表目录？**

A：`main.tex` 中已预留，取消注释即可：
```latex
\listoffigures      % 图目录
\listoftables       % 表目录
\lstlistoflistings  % 代码目录
```

**Q：在 Overleaf 上字体报错怎么办？**

A：Overleaf 无法使用本地安装字体。将 `main.tex` 中所有 Times New Roman 替换为：
```latex
\setmainfont{TeX Gyre Termes}
```
该字体已内置于 Overleaf，无需额外上传。

---

## 贡献 | Contributing

欢迎通过 Issue 反馈问题，或通过 Pull Request 贡献改进。

Feedback and contributions are welcome via Issues or Pull Requests.

1. Fork 本仓库
2. 新建分支：`git checkout -b fix/your-fix`
3. 提交改动：`git commit -m 'fix: describe your fix'`
4. 推送分支：`git push origin fix/your-fix`
5. 发起 Pull Request

---

## 许可证 | License

本项目以 [MIT License](LICENSE) 开源，可自由使用、修改与分发。

This project is released under the [MIT License](LICENSE) — free to use, modify, and distribute.

---

<div align="center">

Made with ❤️ for SDU students &nbsp;·&nbsp; 为山大学子而作

如果这个模板帮到了你，欢迎点一个 ⭐

If this template helped you, a ⭐ would be greatly appreciated!

</div>
