# Mathematica 物理可视化交互平台

基于 Mathematica 的交互式物理教学与实验演示平台，涵盖**力学（19 个模块）、光学（9 个模块）、电磁学（4 个模块）**共 32 个交互实验。

> 本仓库是从妙搭（Miaoda）平台导出的**永久静态版本**，部署于 GitHub Pages，**无 60 天期限、无会员限制、永不过期**。

## 访问地址

- 在线访问：<https://yunli-physics.github.io/physics-platform/>
- Mathematica 笔记本仓库：[yunli-physics/-mathematica-](https://github.com/yunli-physics/-mathematica-)

## 站点说明

- 所有页面、样式、字体、图片均已**完整内联打包**为纯静态文件，不依赖任何外部平台接口
- 全部 32 个实验卡片链接到 GitHub 上对应的 Mathematica 笔记本（.nb 文件），点击即可跳转下载，使用 Wolfram Mathematica / Wolfram Player 打开运行
- 其中「粒子模拟（在线交互）」为 Wolfram Cloud 在线交互版，可直接在浏览器中运行

## 目录结构

```
physics-platform/
├── index.html            # 主页（物理可视化平台入口）
├── 404.html              # SPA 路由回退（与 index.html 相同）
├── assets/
│   ├── index-BKs8Alnb.js # 应用逻辑（已内联全部图片）
│   ├── toolkit-C6NFR-Qs.js
│   ├── radix-C4hRZIqI.js
│   ├── rolldown-runtime-CNC7AqOf.js
│   ├── polyfills.js
│   ├── index-B_rf05PM.css
│   └── fonts/fonts.css   # 字体（已内联为 base64）
└── .github/workflows/pages.yml  # GitHub Pages 自动部署
```

## 如何更新内容

1. 修改 `index-BKs8Alnb.js` 中的模块数据（名称、描述、GitHub 链接等）
2. 推送到 `main` 分支，GitHub Actions 会自动部署
3. 若在 Mathematica 中更新了笔记本，直接推送到 `-mathematica-` 仓库即可，网页中的链接自动指向最新文件

## 部署方式

本仓库通过 GitHub Actions 自动部署到 GitHub Pages（无需手动开启 Pages 设置）。首次推送后，Actions 运行完成即可访问。
