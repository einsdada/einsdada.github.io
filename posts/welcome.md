---
title: 欢迎来到我的博客
date: 2026-09-27
tag: 站点
summary: 这个站点从占位页变成了一块可以写字的地方，介绍博客的用途与写作的意义。
---

# 欢迎来到我的博客

这里是我的个人博客。以前这个站点只是一个占位页，现在它变成了一块可以写字的地方。

我会在这里整理：

- 学习过程中踩过的坑与解法
- 自己动手做的小项目
- 一些值得记录的想法

> 站点刚刚起步，内容会陆续补充。如果你是从 GitHub 主页过来的，感谢停留。

## 为什么写博客

写作是整理思路的最好方式。很多问题在写下来之前，其实并没有想清楚。把过程记录下来，既是给未来的自己，也可能帮到遇到同样问题的人。

## 技术栈

这个站点本身非常简单——单个 HTML 文件作为页面框架，文章以独立的 Markdown 文件存放在 `posts/` 目录中，页面运行时按需加载，用 [marked](https://github.com/markedjs/marked) 渲染，代码高亮使用 highlight.js，托管在 GitHub Pages 上。

```js
// 渲染一篇文章的 Markdown
const html = marked.parse(markdownText);
document.getElementById("post-body").innerHTML = html;
```

> 注：本文为示例文章，用于展示博客的文章排版效果，内容可随时替换。
