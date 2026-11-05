# Toran 作品集

托兰（Toran）的一页作品集。版式参考 [leerob.com](https://leerob.com)：白底、正文为主、细分割线，五个栏目用同一种卡片，互不突出。

页面地址：<https://shuaixiangwang5-collab.github.io/toran-portfolio/>

发布文件在仓库根目录。[`.github/workflows/pages.yml`](.github/workflows/pages.yml) 会在推送到 `main`（以及当前功能分支）时把站点交到 GitHub Pages。GitHub 不允许工作流自己打开 Pages，所以需要仓库管理员做一次：

1. 打开 [Settings → Pages](https://github.com/shuaixiangwang5-collab/toran-portfolio/settings/pages)。
2. Build and deployment 的 Source 选 **GitHub Actions**。
3. 回到 Actions，重新运行失败的 “Deploy site”，或再推一次代码。

做完这一次之后，改 `index.html` 并推送到 `main` 就会更新页面。

## 怎么改内容

只改 [`index.html`](index.html)。用浏览器或 GitHub 网页编辑器都可以。

1. 搜索 `占位`。
2. 页首那句「占位简介」换成你想让读者先看到的话。请继续使用 **Toran / 托兰**，不要写入真实姓名。
3. 每张卡片改三处：标题、一句说明、日期。换成真实内容后，删掉标题里的 `<span class="mark">占位</span>`。
4. 要多加一条，复制一整块 `<article class="card">…</article>`，贴到同一栏里。
5. 提交并推送到 `main`。GitHub Actions 通常一分钟内更新页面。刷新时如果还是旧页面，再等一会儿。

五个栏目都在同一页，权重相同：

- AI 落地项目和案例
- 公众号文章
- 读书和思考笔记
- 抖音视频
- 关于我

现在的卡片都是占位，没有填写成果或数字。换成真实条目时，只写已经发生、可以公开的事。

## 文件

| 文件 | 作用 |
| --- | --- |
| `index.html` | 全部文字。平时只改这个。 |
| `styles.css` | 版式。不改内容就不用动。 |
| `favicon.svg` | 浏览器标签上的小图标。 |
| `.nojekyll` | 让 GitHub Pages 按原样发布静态文件。 |

深色只是页脚的「切换深色」。默认是浅色。选择会记在这台浏览器里。
