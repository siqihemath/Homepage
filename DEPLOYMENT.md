# Siqi He 的个人主页

这是一套可直接用于 GitHub Pages 的静态网页，无需安装依赖或执行构建。目标仓库：[fatlao0627/Homepage](https://github.com/fatlao0627/Homepage)。

## 发布到 GitHub Pages

1. 打开已有仓库 [fatlao0627/Homepage](https://github.com/fatlao0627/Homepage)。仓库目前为私有；GitHub Free 的 Pages 需要公开仓库，支持私有 Pages 的付费方案可保留私有仓库。
2. 将本文件夹**里面的全部内容**上传到仓库根目录，不要把外层 `siqi-he-homepage` 文件夹一并套进去。确认根目录能直接看到 `index.html`，并保留隐藏文件 `.nojekyll`。
3. 打开仓库的 **Settings → Pages**，在 **Build and deployment → Source** 选择 **Deploy from a branch**。
4. 选择 **main** 分支、**/(root)** 文件夹，点击 **Save**。无需另外编写 GitHub Actions 工作流。
5. 等待 GitHub Pages 完成发布，再从该页面提供的地址打开网站。本仓库的预期网址为 `https://fatlao0627.github.io/Homepage/`；以 Pages 设置页显示的发布结果为准。

页面使用相对路径，支持该项目仓库的 `/Homepage/` 地址。若文件已经上传，可直接从第 3 步开始。

官方说明：[创建 GitHub Pages 网站](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)、[配置发布来源](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)。

## 本地查看

在此文件夹打开终端，运行：

```sh
python3 -m http.server 8000
```

然后在浏览器打开 [本地预览](http://localhost:8000)。结束时在终端按 `Ctrl+C`。

## 日常修改

| 内容 | 文件 |
| --- | --- |
| 首页简介、照片说明、常用链接 | `index.html` |
| 论文及研究信息 | `research.html` |
| 学术活动 | `activities.html` |
| 联系方式 | `contact.html` |
| 历史教学记录 | `teaching.html` |
| MA303 课程存档 | `ma303.html` |
| 字体、颜色、间距及手机布局 | `styles.css` |
| 个人照片 | `assets/siqi-he.jpg` |
| 简历 PDF | `assets/cv.pdf` |

保留文件名替换照片或简历，即可继续使用原有链接。导航栏出现在各个 HTML 页面中；修改导航时请同步更新。将修改后的文件提交到发布分支，GitHub Pages 会重新发布。

## 内容与迁移说明

- 内容来源：[原 Google Sites 主页](https://sites.google.com/scgp.stonybrook.edu/siqi-he-math-homepage)。
- 版式参考：[Ciprian Manolescu 的主页](https://web.stanford.edu/~cm5/)，采用简洁的文字、链接和留白布局。
- 照片署名：Sun Song，2020 年，Hyde Park。
- 原研究页面第 [14] 项显示的 arXiv 编号 `2310.18198` 与其实际链接不一致；这里将显示编号修正为 [2310.18934](https://arxiv.org/abs/2310.18934)，保留原有标题与发表信息。

- 历史教学记录保留在页脚的 Teaching archive；MA 303 保留 38 个原 Google Drive 讲义链接与原作业加粗标记，过时的 Zoom 会议号未迁入。
- 论文的 submitted / to appear 等状态沿用原主页，未在此次迁移中逐篇更新。
