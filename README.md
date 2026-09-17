# ✦ Markdown 预览器

> 把 AI 聊天里的乱码，一键变成漂亮的文档。

**在线使用**：https://yejingaaa.github.io/ai-previewer/
**源码**：https://github.com/yejingaaa/ai-previewer

一个纯前端的 Markdown 实时预览工具，支持 **LaTeX 公式**、**Mermaid 图表**、**代码高亮**，可以导出为独立 HTML 文件离线查看。

只需要一个浏览器，不需要安装任何东西。

---

## 为什么做这个

每次跟 AI 聊天，遇到写得好的内容想复制下来保存成文档，结果贴到记事本或 Word 里全是乱码——表格乱了、公式变成一堆符号、代码缩进没了、列表挤成一团。

又不想为了存个文档去装一堆复杂的软件。

所以就做了这个工具：一个纯前端页面，把 AI 生成的 Markdown 内容重新排版成干净、美观的 HTML 文档。

**典型场景**

| 场景 | 怎么做 |
|------|--------|
| 保存 AI 对话记录 | 复制 AI 回复 → 粘贴到左侧 → 右侧自动排版 |
| 整理技术笔记 | 贴入 Markdown 源码 → 实时预览效果 |
| 分享带公式的内容 | 数学、物理公式自动渲染，不用截图 |
| 保存带流程图的内容 | Mermaid 图表自动变成图形 |
| 导出离线文档 | 一键导出独立 HTML 文件，发给谁都能打开 |

---

## 功能

| 功能 | 说明 |
|------|------|
| 📝 **实时预览** | 左边写，右边看，即时渲染 |
| 📐 **LaTeX 公式** | 行内 `$E=mc^2$` 和块级公式 `$$...$$` 都支持 |
| 📊 **Mermaid 图表** | 流程图、时序图、甘特图……直接写在 Markdown 里 |
| 🎨 **代码高亮** | Prism.js 驱动，支持 Python、JS 等多种语言 |
| 🌗 **亮色 / 暗色** | 手动切换，也会自动跟随系统设置 |
| 📦 **导出 HTML** | 一键导出独立的离线 HTML 文件，所有样式内嵌 |
| 📋 **任务列表** | GFM 任务列表 `- [x]` 支持 |
| 🦶 **脚注** | 支持 Markdown 脚注 |

---

## 使用方式

**方式一：在线使用（最简单）**

打开 https://yejingaaa.github.io/ai-previewer/ 即可，不需要下载任何东西。

**方式二：本地使用**

下载仓库里的 `index.html`，双击用浏览器打开即可。单个文件，零依赖，不需要安装。

**方式三：部署自己的副本**

fork 本仓库，在 Settings → Pages 里把 Source 设为 `main` / `/(root)`，就能得到一个属于你的在线地址。

---

## 技术栈

- [markdown-it](https://github.com/markdown-it/markdown-it) — Markdown 解析
- [KaTeX](https://katex.org/) — LaTeX 公式渲染
- [Mermaid](https://mermaid.js.org/) — 图表渲染
- [Prism.js](https://prismjs.com/) — 代码高亮
- [github-markdown-css](https://github.com/sindresorhus/github-markdown-css) — GitHub 风格样式

全部通过 CDN 加载，不需要安装任何东西。

---

## 它是怎么做出来的

非技术背景，通过 AI 编程工具独立完成整个项目：需求怎么拆、什么算「好用」、下一步做什么，这些判断由人来做；代码由 AI 生成。

开发过程就是不断对话：

- *「帮我做个 Markdown 预览器，左右分栏的」*
- *「加一个暗色模式吧」*
- *「表格太长了能不能左右滑动？」*
- *「导出的时候能不能把样式打包进去，离线也能看」*

生成代码 → 打开浏览器验证 → 把不好用的地方描述清楚 → 继续迭代。

---

## License

MIT — 随你用，随便改，随便发。
