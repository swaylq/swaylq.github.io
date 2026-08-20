# swaylq.github.io

`swaylq` 的 GitHub Pages 用户主页 —— 一个静态索引页，外加这台 host 的根级 `robots.txt`。

## 为什么需要这个仓库

GitHub Pages 上每个项目站点住在 `swaylq.github.io/<repo>/` 下，但**爬虫只读域名根目录的那一份 `robots.txt`**。在没有用户主页仓库之前 `https://swaylq.github.io/robots.txt` 返回 404，各项目 `docs/robots.txt` 里的 sitemap 声明爬虫根本读不到，域名根也是一个 GitHub 的「Site not found」页。

这个仓库补上两件事：

- 根级 `robots.txt`，把所有项目站点的 sitemap 一次声明齐；
- 一个真实的首页，给各项目站点一个内部链接入口，而不是彼此孤立。

## 内容

| 文件 | 用途 |
|------|------|
| `index.html` | 索引页 |
| `robots.txt` | 根级，声明本 host 上全部 sitemap |
| `sitemap.xml` | 本页自己的 sitemap |
| `assets/` | 样式与 favicon |
| `google*.html` | Google Search Console 所有权验证，**别删** |

MIT。
