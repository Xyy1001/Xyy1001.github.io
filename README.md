# 个人主页 (Xyy1001.github.io)

这是一个基于静态页面的个人网站源码，用于展示个人简介、教育与项目经历、联系方式和沟通指南等内容。

此站点不依赖服务器端框架，主要由 HTML、CSS 和少量 JavaScript 组成，方便在 GitHub Pages 或任意静态站点托管服务上发布。

## 主要目的

- 作为个人学术/工程主页，展示简历、项目和联系方式。
- 展示若干项目链接（如 GitHub 仓库）。
- 为访问者提供清晰的交流与协作方式（包含一份交流指南页面）。

## 仓库结构（重要文件）

```
e:\Xyy1001.github.io
├─ index.html                # 站点首页
├─ README.md                 # 本说明文档
├─ LICENSE                  # 许可证
├─ Usage.txt                # 使用说明（可选）
├─ contents/
│   └─ HowtoCommunicate.html # 交流指南页面
├─ static/
│   ├─ assets/
│   │   └─ img/              # 图片资源（头像、背景等）
│   ├─ css/
│   │   ├─ main.css
│   │   └─ styles.css        # 页面样式
│   └─ js/
│       ├─ bootstrap.bundle.min.js
│       ├─ js-yaml.min.js
│       ├─ marked.min.js
│       └─ scripts.js        # 页面交互脚本
└─ time/                     # 可能用于页面时间戳或构建记录
```

（以上为仓库中当前的关键文件与目录，具体图片与静态资源请在 `static/assets` 下查看）

## 本地查看（开发/预览）

因为这是纯静态网站，最简单的预览方式是直接用浏览器打开 `index.html`：

1. 使用文件管理器双击打开 `index.html`。
2. 或者在命令行中切换到仓库目录并使用一个轻量的静态服务器：

   - 推荐（Python 3 已安装）:

     ```powershell
     # 在仓库根目录运行
     python -m http.server 8000
     # 然后在浏览器打开 http://localhost:8000
     ```

   - 若使用其他静态服务器（例如 live-server、http-server 等），按各自文档运行即可。

注意：某些浏览器在直接通过 file:// 打开时可能限制跨域请求或某些脚本功能（例如 MathJax 的部分功能）；使用本地服务器可避免这些限制。

## 编辑说明

- 页面主要入口为 `index.html`。内容分为多个 section（例如 `#教育经历`、`#项目经历` 等），直接编辑 HTML 中的文本即可。
- 通用样式放在 `static/css/styles.css` 与 `static/css/main.css`。
- 交互与初始化脚本在 `static/js/scripts.js` 中（例如填充某些动态文本、处理 Markdown 等）。
- 若要新增页面，请将 HTML 文件放入 `contents/` 或根目录，并在导航中添加链接（修改 `index.html` 中的导航栏）。

建议编辑流程：

1. 创建新分支（可选）：

   ```powershell
   git checkout -b feat/update-readme
   ```

2. 修改文件并在本地预览。
3. 提交并推送更改：

   ```powershell
   git add .
   git commit -m "更新页面内容或样式"
   git push origin feat/update-readme
   ```

4. 发起 Pull Request（如果使用协作流程）。

## 部署（GitHub Pages）

1. 将仓库 push 到 GitHub（例如 `github.com/<your>/Xyy1001.github.io`）。
2. 在仓库设置中启用 GitHub Pages，选择 `main` 分支的根目录作为发布源。
3. 等待数分钟，站点将在 https://<用户名>.github.io/ 生效。

提示：若需要自定义域名，可以在仓库设置或添加 `CNAME` 文件来配置。

## 支持的功能与第三方库

- Bootstrap（用于样式与响应式布局）。
- MathJax（用于渲染数学公式）。
- marked.js（用于解析 Markdown 内容到 HTML，若 `scripts.js` 使用）。
- js-yaml（若需要解析 YAML 数据）。

具体实现细节请查看 `index.html` 中的 script 引入和 `static/js/scripts.js`。

## 许可与版权

项目根目录包含 `LICENSE` 文件，请参阅该文件以了解本项目的许可证条款。

## 联系方式

- 学生邮箱：202330841782@mail.scut.edu.cn
- QQ邮箱：3503269275@qq.com
- GitHub： https://github.com/Xyy1001

如需协作或有改进建议，欢迎通过上述联系方式联系我，或直接提交 issues / PR。