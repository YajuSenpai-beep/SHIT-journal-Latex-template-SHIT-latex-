<div align="center">
  <p>
    <a href="./README.md">English</a> |
    简体中文
  </p>
  <img src="./fig/S.H.I.T.png" alt="SHIT Journal Template" width="240">
  <h1>SHIT 构石期刊 LaTeX 模板</h1>
  <p><strong>S.H.I.T. = Sciences · Humanities · Information · Technology</strong></p>
  <p>
    一个面向虚构期刊 <strong>SHIT / 构石</strong> 的中英双语学术论文模板
  </p>
  <p>
    <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-blue.svg">
    <img alt="Engine: XeLaTeX" src="https://img.shields.io/badge/engine-XeLaTeX-0F6CBD.svg">
    <img alt="Bibliography: Nature" src="https://img.shields.io/badge/bibliography-Nature-orange.svg">
    <img alt="Language: Chinese + English" src="https://img.shields.io/badge/language-Chinese%20%2B%20English-green.svg">
    <img alt="Status: Available" src="https://img.shields.io/badge/status-Available-success.svg">
  </p>
  <p>
    <a href="#about">简介</a> •
    <a href="#features">特性</a> •
    <a href="#quick-start">快速开始</a> •
    <a href="#build">编译方法</a> •
    <a href="#license">许可协议</a>
  </p>
</div>

---

## 简介

本仓库提供虚构期刊 **SHIT / 构石** 的 LaTeX 模板。
模板目标是提供一套接近期刊成稿体验的写作流程，包括中英双语支持、自定义首页、结构化摘要、标准交叉引用，以及 Nature 风格参考文献系统。

---

## 特性

### 期刊式首页

- 自定义 SHIT 刊头与元信息区
- Subject Section 与摘要上下横线
- 题目、作者、单位、摘要与编辑信息按期刊样式组织

### 可直接写作的正文结构

- `Introduction`
- `Related Work`
- `Methods`
- `Results`
- `Discussion`
- `Conclusion`

### 标准论文组件

- 基于 `./fig/` 的图片示例
- 表格示例
- 公式示例
- 基于 `algorithm` + `algpseudocode` 的伪代码示例
- 类似出版社规范的 AI statement 区块
- 图、表、算法、公式的交叉引用示例

### 引用系统

- 文献数据维护在 `references.bib`
- 使用 `biblatex + biber` 实现 Nature 风格参考文献
- 正文引用为蓝色上标编号

---

## 仓库结构

```text
SHIT/
├─ fig/                # 正文与 README 共用图片资源
│  ├─ S.H.I.T.png
├─ references.bib
├─ shit_journal_template.tex
├─ README.md
├─ README.zh-CN.md
├─ LICENSE
└─ .gitignore
```

---

## 快速开始

1. 编辑 `shit_journal_template.tex`。
2. 将正文所需图片放入 `./fig/`。
3. 在 `references.bib` 中维护参考文献条目。
4. 使用 XeLaTeX 与 Biber 编译。

---

## 编译方法

```bash
xelatex shit_journal_template.tex
biber shit_journal_template
xelatex shit_journal_template.tex
xelatex shit_journal_template.tex
```

如果编译后编辑器仍然显示旧的 PDF 预览，手动刷新一次预览窗口即可。

---

## 写作规则

- 中文正文字体配置为 `SimSun`
- 英文正文字体配置为 `Times New Roman`
- 模板正文图片目录为 `./fig/`
- 参考文献条目统一写在 `references.bib`
- 默认引用命令已经映射为 Nature 风格蓝色上标

---

## 许可协议

本项目采用 **MIT License**。  
详见 [LICENSE](./LICENSE)。

---

<div align="center">
  <sub><i>"Truth Fades, S.H.I.T Lasts."</i></sub>
  <br>
  <sub><i>"真理会过时，构石永恒。"</i></sub>
</div>
