# Markly

> Markdown 桌面端编辑器 · 书写新体验

[![Electron](https://img.shields.io/badge/Electron-桌面端-blue.svg)](https://electronjs.org/)
[![Vue](https://img.shields.io/badge/Vue-3.x-brightgreen.svg)](https://vuejs.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📖 项目简介

Markly 是一款跨平台的 **Markdown 桌面编辑器**，基于 Electron 构建，提供流畅的编辑体验。支持实时预览、语法高亮、云同步等功能，专为写作者和开发者设计。

> 让 Markdown 创作更加专注高效

## ✨ 核心功能

### 📝 编辑体验

| 功能 | 说明 |
|------|------|
| 实时预览 | 编辑与预览同步进行，所见即所得 |
| 双栏布局 | 左侧编辑，右侧预览，可切换单栏 |
| 焦点模式 | 隐藏侧边栏和工具栏，专注写作 |
| 打字机模式 | 当前行始终保持在窗口中央 |

### 🎯 Markdown 支持

| 语法 | 说明 |
|------|------|
| GFM | 完整 GitHub Flavored Markdown 支持 |
| 表格 | 可视化表格编辑，语法自动生成 |
| 代码块 | 100+ 编程语言语法高亮 |
| 数学公式 | LaTeX 数学公式渲染 |
| 流程图 | Mermaid 图表支持 |
| Todo | 任务列表 `- [x]` `- [ ]` |

### 🔧 写作工具

| 功能 | 说明 |
|------|------|
| 字数统计 | 实时显示字符数、字数、行数、阅读时间 |
| 导出功能 | 导出 PDF、HTML、DOCX、PNG |
| 剪贴板粘贴 | 自动识别并格式化粘贴内容 |
| 快捷键 | 丰富的 Vim/Emacs 风格快捷键 |

## 🛠️ 技术栈

| 类别 | 技术 |
|------|------|
| 桌面框架 | Electron |
| 前端框架 | Vue.js |
| 编辑器核心 | CodeMirror / Monaco |
| Markdown | marked / markdown-it |
| 语法高亮 | highlight.js / Prism.js |
| 数学公式 | KaTeX / MathJax |

## 📁 项目结构

```
Markly/
├── build/                        # 构建资源
│   └── icons/                    # 应用图标
├── electron/                     # Electron 主进程
│   ├── main.js                  # 主进程入口
│   ├── preload.js               # 预加载脚本
│   ├── window.js               # 窗口管理
│   ├── menu.js                 # 菜单配置
│   └── ipc.js                  # 进程通信
├── public/                      # 静态资源
├── src/                         # 渲染进程源代码
│   ├── components/              # Vue 组件
│   │   ├── editor/              # 编辑器组件
│   │   ├── sidebar/             # 侧边栏组件
│   │   └── common/              # 公共组件
│   ├── views/                   # 页面视图
│   ├── store/                   # 状态管理
│   ├── utils/                   # 工具函数
│   └── assets/                 # 资源文件
├── testFiles/                  # 测试文件
└── package.json
```

## 🚀 快速开始

### 环境要求

- Node.js 14+
- npm 6+

### 安装依赖

```bash
npm install
```

### 启动开发服务器

```bash
npm run serve
```

### 打包桌面应用

```bash
npm run build
```

## ⌨️ 快捷键

### 编辑快捷键

| 快捷键 | 功能 |
|--------|------|
| `Ctrl + B` | 加粗 |
| `Ctrl + I` | 斜体 |
| `Ctrl + K` | 插入链接 |
| `Ctrl + Shift + K` | 插入代码块 |
| `Ctrl + Shift + I` | 插入图片 |
| `Ctrl + U` | 下划线 |
| `Ctrl + Shift + X` | 删除线 |

### 视图快捷键

| 快捷键 | 功能 |
|--------|------|
| `Ctrl + /` | 切换侧边栏 |
| `Ctrl + Shift + F` | 全屏编辑 |
| `Ctrl + 1` | 仅编辑视图 |
| `Ctrl + 2` | 仅预览视图 |
| `Ctrl + 3` | 双栏视图 |
| `F11` | 全屏 |

### 文件快捷键

| 快捷键 | 功能 |
|--------|------|
| `Ctrl + N` | 新建文件 |
| `Ctrl + O` | 打开文件 |
| `Ctrl + S` | 保存文件 |
| `Ctrl + Shift + S` | 另存为 |
| `Ctrl + W` | 关闭文件 |

## 🎨 主题预览

| 主题 | 说明 |
|------|------|
| 🌙 Dark | 深色主题，适合夜间写作 |
| ☀️ Light | 浅色主题，适合白天使用 |
| 🌿 Sepia | 护眼模式，减少眼睛疲劳 |
| 🌊 Ocean | 海洋蓝，清新护眼 |
| 🌲 Forest | 森林绿，自然舒适 |
| ⚫ Charcoal | 石墨黑，专业深邃 |

## 📤 导出格式

| 格式 | 说明 |
|------|------|
| `--format pdf` | PDF 文档 |
| `--format html` | HTML 网页 |
| `--format docx` | Word 文档 |
| `--format png` | 图片 |
| `--format json` | JSON 数据 |

## ❓ 常见问题

### Q: 支持 Vim 模式吗？

> 支持！在设置中开启 Vim 模式，即可使用 Vim 风格的快捷键和编辑方式。

### Q: 如何自定义快捷键？

> 进入设置 → 快捷键，可以查看和自定义所有快捷键绑定。

### Q: 同步功能如何使用？

> Markly 支持连接云存储服务（正在支持），可以在设置中添加云盘路径实现文件同步。

## 🔮 未来功能

- [ ] 云同步 (OneDrive, iCloud, Dropbox)
- [ ] 插件系统
- [ ] 对外开放 API
- [ ] 协作编辑
- [ ] 多语言界面
- [ ] 大纲视图

## 📄 License

MIT License
