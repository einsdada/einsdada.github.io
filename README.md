# einsdada.github.io

einsdada 的个人博客，托管于 GitHub Pages。

## 结构

- `index.html` — 博客页面框架（纯静态，运行时加载文章，无需构建）
- `posts/` — 文章目录，每篇一个 Markdown 文件
- `posts/README.md` — 文章清单，新增文章在此添加一行链接

## 添加文章

1. 在 `posts/` 新建 `xxx.md`，开头写 front matter（`title` / `date` / `tag` / `summary`）
2. 在 `posts/README.md` 列表中添加一行 `- [标题](xxx.md)`
3. 推送后页面自动发现并展示

## 本地预览

```bash
python -m http.server 8000
```

然后访问 <http://localhost:8000>。注意页面需通过 http 访问（file:// 下浏览器禁止读取数据文件）。
