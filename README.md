# PaperSwipe 产品宣传页

> 别再搜论文了，开始刷论文。

PaperSwipe —— 从一个研究问题，到下一篇值得读的论文。围绕研究主题探索论文、查看结构化解读、整理文献库、再安排自己的阅读日程。

本仓库是 PaperSwipe 的静态产品宣传页，可部署到 Cloudflare Pages、Vercel 或任意静态托管平台。

## 目录结构

```
.
├── index.html            # 宣传页入口
├── paperswipe-assets/    # 图片、样式、脚本、演示视频等静态资源
│   ├── site.css
│   ├── site.js
│   ├── *.png / *.jpg
│   └── product-demo-20261015.mp4
└── README.md
```

## 本地预览

直接双击 `index.html` 即可在浏览器打开（保持 `paperswipe-assets/` 与 `index.html` 同级即可）。

## 部署到 Cloudflare Pages（Git 集成）

1. 登录 Cloudflare Dashboard → **Workers & Pages** → **Create application** → **Pages** → **Connect to Git**
2. 选择 GitHub 中的本仓库
3. 构建设置：
   - 框架预设：`None`（纯静态）
   - 构建命令：留空
   - 输出目录：`/`（或 `.`）
4. 点 **Save and Deploy**，等待完成后打开 `https://<项目名>.pages.dev`

> 提示：默认 `*.pages.dev` 域名在中国大陆可能无法稳定访问。面向大陆用户，建议绑定自定义域名并配合国内 CDN（如腾讯云 EdgeOne）回源，或改用国内对象存储（腾讯云 COS / 阿里云 OSS）托管。

## 相关链接

- 产品入口：https://paperswipe.site/login （邀请制内测）
