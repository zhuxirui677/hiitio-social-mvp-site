# HIITIO Social MVP Site

这是 HIITIO 社媒运营工作台 MVP 的静态网站部署包。

## 目录内容

- `index.html`：网站主文件，可直接部署。
- `preview-desktop.png`：桌面预览图。
- `preview-mobile.png`：移动预览图。
- `vercel.json`：Vercel 静态部署配置。
- `netlify.toml` / `_headers`：Netlify、Cloudflare Pages 可用的基础配置。

## 最快上线方式

### Netlify Drop

1. 打开 https://app.netlify.com/drop
2. 把整个 `hiitio-social-mvp-site` 文件夹拖进去。
3. Netlify 会生成一个公开 URL，其他人即可访问。

### Vercel

1. 打开 https://vercel.com/new
2. 导入包含本文件夹的 Git 仓库，或使用 Vercel CLI。
3. Framework 选择 `Other`，Build Command 留空，Output Directory 选择当前文件夹。

### Cloudflare Pages

1. 打开 Cloudflare Pages。
2. 选择 Direct Upload 或连接 Git 仓库。
3. Build Command 留空，Output Directory 选择当前文件夹。

## 本地预览

在本目录运行：

```bash
python3 -m http.server 4173
```

然后打开：

```text
http://127.0.0.1:4173
```

## 正式产品化下一步

- 接入真实登录和权限。
- 把 mock 数据迁移到后端数据库。
- 接入平台 OAuth/API。
- 把素材压缩从浏览器模拟改成后端队列任务。
- 给发布任务加真实回执、重试和错误日志。
