# 🎨 PixelGlyph

**将任何图像、文字或涂鸦实时转换为炫酷的 ASCII / 彩色字符画**

[![Status](https://img.shields.io/badge/status-production-success)](https://github.com)
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)](https://github.com)

---

## ✨ 功能特性

- 📷 **图片转 ASCII** – 上传或拖放任意图片，实时生成黑白或彩色字符画
- 📝 **文字转字符画** – 输入文字，自由选择字体、大小、粗体/斜体，即刻渲染
- 🎨 **自由手绘模式** – 在画布上随意涂鸦，支持画笔、橡皮擦、调节粗细与颜色
- 📹 **摄像头捕获** – 调用摄像头，实时捕获画面并转换为字符艺术
- 🌈 **彩色字符渲染** – 基于 Canvas 的高性能彩色输出，完美保留原图颜色
- 🎞️ **图像滤镜** – 内置边缘检测、反相、灰度增强等滤镜，拓展创作可能
- 🔤 **丰富字符集** – 预设标准、方块、精细、盲文、Emoji、二进制等，支持自定义
- 📏 **灵活参数调节** – 输出宽度、字符高宽比实时可调，改变画面密度
- 💾 **多格式导出** – 一键复制纯文本或彩色 HTML，也可下载为 TXT 或 PNG
- 🖼️ **本地作品画廊** – 基于 localStorage 的收藏系统，可保存、加载、清空作品
- 🎲 **随机灵感** – 一键生成随机文字或彩色抽象画，激发创作灵感
- 🌓 **深色/浅色主题** – 手动切换或跟随系统，保护视力
- ⛶ **全屏沉浸模式** – 点击按钮进入全屏，获得更专注的创作环境
- 📤 **社交分享** – 一键复制包含作品预览的分享文本，轻松发布到社交平台
- ⌨️ **键盘快捷键** – `Ctrl+Enter` 快速生成，`Ctrl+Shift+R` 随机灵感
- 📱 **移动端适配** – 支持触摸绘图，响应式布局完美兼容手机和平板

---

## 🚀 在线演示

直接打开 `index.html` 即可使用，无需任何构建步骤。  
推荐使用现代浏览器（Chrome / Edge / Firefox / Safari）。

---

## 🛠️ 快速开始

```bash
git clone https://github.com/mrtransition/pixelglyph.git
cd pixelglyph
```

用浏览器打开 `index.html` 即可。  
如果需要使用摄像头功能，建议通过本地服务器启动（如 VS Code Live Server）。

---

## 📖 使用说明

| 区域 | 操作 |
|------|------|
| **左侧控制面板** | 切换模式、上传图片、调整参数（宽度、高宽比、滤镜、字符集） |
| **右侧输出区** | 查看生成的字符画，支持“纯文本”和“彩色渲染”两种视图 |
| **底部操作栏** | 复制、收藏到画廊、下载 TXT / PNG |
| **顶部工具栏** | 随机灵感、主题切换、全屏、分享 |

> 💡 **提示**：在文字模式下，字体输入框支持 `datalist` 建议列表，也可以直接输入本机已安装的任意字体名称。

---

## 🧰 技术栈

- **前端**：纯 HTML5 + CSS3 + Vanilla JavaScript（IIFE 模块化）
- **图形处理**：Canvas API、FileReader、MediaDevices
- **存储**：localStorage（画廊收藏）
- **字体**：系统原生字体 + 等宽字体回退
- **响应式**：CSS Grid + 媒体查询
- **零依赖**：单个 HTML 文件即可运行，无需任何外部库或框架

---

## 📁 项目结构

```
pixelglyph/
├── pixelglyph.html       # 完整应用（HTML + CSS + JS）
└── README.md        # 项目说明
```

---

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！  
如果您有新的字符集预设、滤镜创意或功能建议，请随时告诉我们。

---

## 📄 许可证

本项目采用 [MIT License](LICENSE) 开源，您可以自由使用、修改和分发。

---

<div align="center">
  <sub>Made with 🎨 by PixelGlyph Team</sub>
</div>
