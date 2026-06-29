# 🎨 PixelGlyph Pro

**将任何图像、文字或涂鸦实时转换为炫酷的 ASCII / 彩色字符画 — 企业级增强版**

[![Status](https://img.shields.io/badge/status-production-success)](https://github.com)
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)](https://github.com)

---

## ✨ 功能特性

### 核心功能
- 📷 **图片转 ASCII** – 上传或拖放任意图片，实时生成黑白或彩色字符画
- 📝 **文字转字符画** – 输入文字，自由选择字体、大小、粗体/斜体，即刻渲染
- 🎨 **自由手绘模式** – 在画布上随意涂鸦，支持画笔、橡皮擦、调节粗细与颜色
- 📹 **摄像头捕获** – 调用摄像头，实时捕获画面并转换为字符艺术

### 🎞️ 滤镜系统（10种）
- **灰度** / **反相** / **棕褐色** — 经典色彩变换
- **边缘检测** — 同时检测水平+垂直边缘，消除行边界伪影
- **边缘增强** — Laplacian 内核强化细节
- **锐化** / **模糊** — 3×3 卷积核
- **浮雕** — 3×3 Emboss 核，偏移 128 保留亮度
- **像素化** — 自适应块大小马赛克

### 🔤 字符集（8种预设）
- **标准** ` .:-=+*#%@` / **方块** ` ░▒▓█` / **精细**（96 级灰度） / **Emoji**
- **盲文**（64 级 Braille 图案） / **十六进制** / **二进制**
- 支持**自定义字符集**输入

### ⚙️ 高级参数
- **亮度** / **对比度** — 独立滑动调节，实时预览
- **Floyd-Steinberg 抖动** — 误差扩散算法，减少量化损失，提升细节表现
- **反转映射** — 一键交换黑白映射方向

### 📦 批量处理
- **多图上传** — 支持同时拖放或选择多张图片
- **缩略图切换** — 点击缩略图切换当前编辑图片，支持删除
- **批量生成** — 一键生成所有图片的 ASCII 字符画
- **ZIP 导出** — 纯 JavaScript 实现的 ZIP 打包，每张图片输出 TXT + SVG

### 💾 多格式导出
- 📋 **复制** — 纯文本或彩色 HTML（Clipboard API + fallback）
- 📄 **TXT 下载** — 纯文本文件
- 🖼️ **PNG 下载** — 渲染为位图图片
- 📐 **SVG 下载** — 保留颜色的矢量格式
- 🌐 **HTML 下载** — 彩色 HTML 独立页面，可在线分享

### 🖼️ 本地作品画廊
- 基于 `localStorage` 的收藏系统，可保存、加载、清空作品（最多 20 幅）

### 🎲 随机灵感
- 一键生成随机文字或彩色抽象画，激发创作灵感

### 🎨 界面主题
- 🌓 **深色/浅色主题** — 手动切换
- ⛶ **全屏沉浸模式** — 专注创作环境
- 📤 **社交分享** — 一键复制分享文本
- ⌨️ **键盘快捷键** — `Ctrl+Enter` 快速生成，`Ctrl+Shift+R` 随机灵感
- 📱 **移动端适配** — 触摸绘图，响应式布局

---

## 🚀 在线演示

直接打开 `PixelGlyph.html` 即可使用，无需任何构建步骤。  
推荐使用现代浏览器（Chrome / Edge / Firefox / Safari）。

---

## 🛠️ 快速开始

```bash
git clone https://github.com/mrtransition/PixelGlyph.git
cd PixelGlyph
```

用浏览器打开 `PixelGlyph.html` 即可。  
如需摄像头功能，建议通过本地服务器启动（如 VS Code Live Server）。

---

## 📖 使用说明

| 区域 | 操作 |
|------|------|
| **左侧控制面板** | 切换模式、上传图片、调整参数（宽度/高宽比/滤镜/字符集/高级参数） |
| **右侧输出区** | 查看生成的字符画，支持"纯文本"和"彩色渲染"两种视图 |
| **底部操作栏** | 复制、收藏画廊、下载 TXT / PNG / SVG / HTML |
| **顶部工具栏** | 随机灵感、主题切换、全屏、分享 |

> 💡 **提示**：在文字模式下，字体输入框支持 `datalist` 建议列表，也可直接输入本机已安装的任意字体名称。批量处理时支持多选文件上传和拖放。

---

## 🧰 技术栈

- **前端**：纯 HTML5 + CSS3 + Vanilla JavaScript（IIFE 模块化）
- **图形处理**：Canvas API、卷积核滤镜、Floyd-Steinberg 抖动算法
- **存储**：localStorage（画廊收藏）
- **压缩**：纯 JavaScript ZIP 实现（Store 模式 + CRC32）
- **字体**：系统原生字体 + 等宽字体回退
- **响应式**：CSS Grid + 媒体查询
- **零依赖**：单个 HTML 文件即可运行，无需任何外部库或框架

---

## 📁 项目结构

```
pixelglyph/
├── PixelGlyph.html       # 完整应用（HTML + CSS + JS）
└── README.md             # 项目说明
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
