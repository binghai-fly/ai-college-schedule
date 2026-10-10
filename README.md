# AI 大学生课表 · 手机网页版

一个纯前端、单文件的大学生课表应用。上传课表文件，AI 自动解析整理成手机端课表网格。

![Version](https://img.shields.io/badge/version-v7.7-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![HTML](https://img.shields.io/badge/HTML-5-orange)
![JS](https://img.shields.io/badge/JavaScript-Vanilla-yellow)

## ✨ 功能特性

- **🤖 AI 智能解析** — 接入 DeepSeek API，自动识别课表文本，无需手动整理
- **👁️ 视觉识别** — 支持通义千问（DashScope）API，直接拍课表照片就能识别
- **📥 多格式导入** — 支持 HTML、Excel(.xlsx)、TXT、CSV、图片
- **📱 手机原生体验** — 仿原生课表网格 UI，移动端优先设计
- **✍️ 手动编辑** — 点击空白格直接添加课程，点课程可编辑
- **💾 本地存储** — 课表数据保存在浏览器 localStorage，无需服务器
- **🌙 深色主题** — 深色渐变 UI，护眼好看
- **📤 导出功能** — 一键导出课表
- **📅 周次切换** — 支持按周查看课程，自动高亮今天

## 🛠️ 技术栈

- 纯 HTML / CSS / JavaScript（单文件，无框架）
- [XLSX.js](https://sheetjs.com/) — Excel 文件解析
- [Tesseract.js](https://tesseract-ocr.github.io/) — 浏览器端 OCR 识别
- DeepSeek API — AI 文本解析
- 通义千问 DashScope API — 图片视觉识别

## 🚀 快速开始

### 在线使用

直接下载 `index.html`，用手机浏览器打开即可使用。

### 本地运行

```bash
# 方式一：直接用浏览器打开
双击 index.html

# 方式二：启动本地服务器
npx serve .
```

## ⚙️ 配置说明

### DeepSeek API Key（必需）

1. 前往 [DeepSeek 开放平台](https://platform.deepseek.com/) 注册并获取 API Key
2. 在应用首页输入你的 API Key（`sk-` 开头）
3. Key 仅保存在浏览器 localStorage，不会上传到任何服务器

### 通义千问视觉识别 Key（可选）

用于图片课表的更精准识别：

1. 前往 [阿里云百炼](https://bailian.console.aliyun.com/) 获取 DashScope API Key
2. 在「视觉识别 Key」一栏填入

## 📖 使用方法

1. **导入课表** — 上传课表文件或直接粘贴课表文本
2. **AI 解析** — 点击「开始解析课表」，AI 自动整理成结构化课表
3. **查看课表** — 切换周次，查看每日课程安排
4. **编辑调整** — 点击课程格子可修改时间、地点、周次等信息

## 📂 项目结构

```
ai-college-schedule/
├── index.html          # 主应用文件（单文件包含所有 HTML/CSS/JS）
└── README.md
```

## 🔒 隐私安全

- 所有数据均存储在你自己的浏览器中
- API Key 仅保存在本地，不会被上传
- AI 解析只处理你主动上传/粘贴的课表内容
- 请不要在课表文本中放入密码等敏感信息

## 📄 更新日志

### v7.7
- 优化手机端课表网格显示
- 提升 AI 解析准确率
- 修复已知 bug

## 📄 License

MIT License
