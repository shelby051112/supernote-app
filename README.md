# SuperNote

**笔记 · 浏览 · AI** — 一站式知识整理工具

> 单文件 Web 应用，打开即用，无需安装。支持本地笔记编辑、网页浏览、AI 对话、文本高亮标注，所有数据保存在浏览器 LocalStorage 中。

---

## ✨ 功能特性

### 📓 笔记编辑
- 富文本编辑器（加粗、斜体、下划线、标题、列表、引用）
- 多笔记管理，LocalStorage 自动保存
- 笔记导入 / 导出（JSON 格式）
- 划词高亮标注（4 种颜色：重点 / 疑问 / 要点 / 例证）
- 批注功能，标注汇总折叠栏
- 点击标注卡片自动定位到文中位置

### 🌐 内置浏览器
- URL 导航 + iframe 网页浏览
- 前进 / 后退 / 刷新

### 🤖 AI 助手
- OpenAI 兼容 API 流式对话（默认 DeepSeek）
- 网页划词自动优化 Prompt（问 AI / 解释 / 翻译 / 存笔记）
- 快捷操作：总结网页、解释、翻译、存为笔记
- API 设置持久化

### 🎨 界面体验
- 三栏布局，左右面板可拖拽调整宽度
- 3 种主题：浅色 / 深色 / 护眼
- 工具栏自适应换行
- 全部笔记 Overlay 抽屉面板

---

## 🚀 使用方式

### 在线访问
👉 [GitHub Pages 演示](https://shelby051112.github.io/supernote-app/)

### 本地使用
1. 下载 `index.html`
2. 用浏览器直接打开即可

就是这么简单——零依赖，零构建，零服务器。

---

## 🛠️ 技术栈

| 层面 | 技术 |
|------|------|
| UI 框架 | Tailwind CSS (CDN) |
| 图标 | Lucide Icons (CDN) |
| 富文本 | contentEditable + document.execCommand |
| 高亮标注 | Selection API + Range API + `<mark>` 元素 |
| AI 对话 | OpenAI 兼容 API (SSE Streaming) |
| 数据持久化 | LocalStorage |
| 托管 | GitHub Pages (静态) |

---

## ⚙️ AI 配置

1. 打开右侧 AI 面板
2. 点击「⚙️ API 设置」
3. 填入 API 地址、密钥、模型名
4. 默认配置为 DeepSeek（`https://api.deepseek.com/v1`，模型 `deepseek-chat`）

支持任何 OpenAI 兼容 API（OpenAI、DeepSeek、Ollama 等）。

---

## 📁 项目结构

```
supernote-app/
├── index.html    # 完整应用（单文件）
├── README.md     # 本文件
└── LICENSE       # MIT 协议
```

---

## 📜 开源协议

[MIT License](LICENSE) — 自由使用、修改、分发，只需保留版权声明。
