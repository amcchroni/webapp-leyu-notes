# webapp-leyu-notes

## 项目简介

`webapp-leyu-notes` 是一个用于归档和发布多个独立 HTML 页面的仓库。这些页面通常为单页应用或静态内容，不依赖特定的后端服务，主要用于个人记录、工具页面或轻量级演示。

本仓库不针对任何特定域名或网站，所有页面均为独立的 HTML 文件，可直接在浏览器中打开运行。

## 目录结构

```
webapp-leyu-notes/
├── README.md          # 本文件
├── index.html         # 主入口页面（可选）
├── pages/             # 存放各个独立 HTML 页面的目录
│   ├── page1.html
│   ├── page2.html
│   └── ...
└── assets/            # 公共资源（样式、脚本、图片等）
    ├── css/
    ├── js/
    └── images/
```

- `pages/`：每个 HTML 文件代表一个独立页面，可单独访问。
- `assets/`：存放页面共用的 CSS、JavaScript 或图片资源，减少重复。

## 页面归档说明

仓库中的 HTML 页面主要用于以下场景：

- 个人笔记或备忘的网页化展示
- 轻量级工具页面（如计算器、清单、时间线等）
- 静态演示或原型页面
- 其他无需后端支持的独立页面

每个页面均为自包含或仅引用 `assets/` 下的公共资源，便于直接部署到任何静态文件服务器（如 GitHub Pages、Netlify、本地服务器等）。

## 如何使用

1. **克隆仓库**
   ```bash
   git clone https://github.com/your-username/webapp-leyu-notes.git
   ```

2. **本地预览**
   直接在浏览器中打开 `pages/` 下的任意 HTML 文件，或通过本地服务器运行（推荐）：
   ```bash
   cd webapp-leyu-notes
   python -m http.server 8000
   ```
   然后访问 `http://localhost:8000/pages/` 查看页面列表。

3. **添加新页面**
   - 在 `pages/` 目录下创建新的 HTML 文件。
   - 如需引用公共资源，使用相对路径 `../assets/...`。
   - 提交并推送即可归档新页面。

## 维护说明

- 本仓库主要用于个人归档，不保证所有页面长期可用或兼容最新浏览器。
- 欢迎提交 Issue 或 Pull Request 来改进页面内容或修复问题。
- 请勿上传包含敏感信息、商业机密或违反法律法规的内容。
- 如使用本仓库中的代码或设计，请自行评估风险。

## 许可

本仓库中的内容仅供个人学习与参考，不附带任何明示或暗示的保证。如需引用或分发，请注明出处。
