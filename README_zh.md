# dashboard.rayawa.top

[English](README.md) | 简体中文

介绍 Dashboard 客户端、市场数据服务与 API 资源的多语言展示站。

## 项目概述

静态站点链接 Dashboard 各界面和平台客户端，说明服务架构并展示服务统计。本站属于展示层，市场后端单独维护；首页移除成员身份与个人联系方式。

## 技术栈与依赖

HTML、CSS、JavaScript，使用外部字体/图标及 API 统计。页面只需静态 HTTP 服务器；实时计数和配置链接依赖外部服务。

## 文件结构

- `index.html` — 默认首页
- `en/` — 英文首页
- `fr/` — 法文首页
- `dashboard.css` — 共享样式
- `dashboard.js` — 服务配置与统计

## 快速上手

在仓库根目录启动静态服务器：

```bash
python3 -m http.server 8000
```

打开 `http://localhost:8000/`，无需前端编译。外部托管资源需要网络。

部署前核对 `dashboard.js` 中的服务地址，其他语言入口为 `/en/` 与 `/fr/`。
