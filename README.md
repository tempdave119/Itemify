---
name: "Itemify README"
description: "项目介绍：目标、使用方式与快速上手"
---

# Itemify

## 项目简介

一个纯前端的开发者工具箱：格式化、编码、加密、生成器、网络计算与图片处理共 24 个功能收在一个页面里，双击即可打开，全部在本机浏览器内完成，数据不出本机。

## 目标

- 常见小工具不再散落在各种在线网站上，一个本地页面解决。
- 零安装、零后端、零账号：下载就能用，不联网也能用（个别功能除外）。
- 能打包成单个 HTML 带走：U 盘、内网机器、临时环境。

## 快速上手

```bash
# 直接用：双击 src/index.html，或在浏览器里打开
open src/index.html

# 打包成单文件（产物在 dist/）
node scripts/build-single-file.mjs

# 跑测试（需要本机有 Google Chrome）
node --test tests/nav-default.test.mjs
node --test tests/ssh-keygen.test.mjs
```

无 `npm install`，无依赖树。

## 使用方式

- **格式化**：XML / JSON / CSS / HTML / Java 与 XML⇄JSON 互转全部本地计算；JS 与 SQL 通过 CDN 加载 Prettier / sql-formatter，首次使用需要联网。
- **工具**：密码、Base64、URL、UUID/ULID、随机串、二维码（生成与本地解析）、Hash、RSA、签名验签、Bcrypt、SSH 密钥、时间日期、IP 网络计算器、IP 归属查询、`docker run` → `docker-compose.yml`、图片水印。
- **导航自定义**：点左下「⚙ 自定义」后，可把右侧功能拖到左侧任意归类、拖分类调整顺序、新建归类；「设为默认」记住当前布局，「恢复默认」回到它，「恢复出厂」清掉自定义默认。配置存在 localStorage。
- **联网项**：仅「IP 地址查询」与 JS / SQL 格式化的 CDN 引擎。
