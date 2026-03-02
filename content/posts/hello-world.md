+++
date = '2026-03-02T19:38:29+08:00'
draft = false
title = 'Hello World'
description = '我的第一篇博客文章，记录建站过程'
tags = ['Hugo', 'Blog', 'GitHub Pages']
categories = ['技术']
ShowToc = true
+++

## 你好，世界！

这是我的第一篇博客文章，使用 [Hugo](https://gohugo.io/) 构建，部署在 GitHub Pages 上。

## 技术栈

| 工具 | 用途 |
|------|------|
| Hugo | 静态网站生成器 |
| PaperMod | 简洁主题 |
| GitHub Pages | 免费托管 |
| GitHub Actions | 自动部署 |

## 为什么选择 Hugo？

**极快的构建速度** — Hugo 是目前最快的静态网站生成器之一，构建数百篇文章只需不到一秒。

**Markdown 写作** — 专注于内容本身，用 Markdown 写文章，Hugo 自动生成漂亮的页面。

**丰富的主题** — 社区提供了大量高质量主题，比如我正在使用的 PaperMod。

**零成本部署** — 配合 GitHub Pages，完全免费，还自带 HTTPS。

## 建站流程

```bash
# 安装 Hugo
wget https://github.com/gohugoio/hugo/releases/download/v0.146.0/hugo_extended_0.146.0_linux-amd64.deb
sudo dpkg -i hugo_extended_0.146.0_linux-amd64.deb

# 创建站点
hugo new site my-blog && cd my-blog && git init

# 添加主题
git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod

# 写文章
hugo new posts/hello-world.md

# 本地预览
hugo server -D
```

## 下一步

- 持续更新技术文章
- 探索更多 Hugo 功能
- 优化网站体验

期待在这里记录更多！
