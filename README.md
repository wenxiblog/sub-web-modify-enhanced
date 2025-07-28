# Sub-Web Modify（增强版）

> 🚀 优化 UI + 支持 Vercel/Cloudflare 部署的订阅转换 Web 工具

基于 [sub-web](https://github.com/CareyWang/sub-web) 修改增强，适合自部署、美观易用、支持订阅解析、暗黑模式、Cloudflare/Vercel 部署等。

---

## ✨ 功能特色

- 🎨 UI 美化（圆角、卡片、输入框、按钮、动画）
- 🌙 暗黑模式（自动/手动切换）
- 🌐 支持 Cloudflare Pages / Vercel 无服务器部署
- 🛠 支持 Docker 本地部署

---

## 📦 本地运行

```bash
yarn install
yarn serve
```

访问：http://localhost:8080

---

## 🚀 一键部署

### ✅ Vercel 部署

1. Fork 本项目
2. 进入 [Vercel](https://vercel.com/) 绑定 GitHub
3. 新建项目，设置构建命令：
   ```
   yarn build
   ```
   输出目录：
   ```
   dist
   ```

### ✅ Cloudflare Pages 部署

- 构建命令：`yarn build`
- 输出目录：`dist`
- Node 版本建议：`18`
- 可启用 Git 自动部署

---

## 🐳 Docker 运行

```bash
docker build -t sub-web-modify .
docker run -d -p 8080:80 sub-web-modify
```

---

## 🧾 目录结构简述

```
├── public/               # 静态资源（favicon、html）
├── src/                  # Vue 源码
│   ├── assets/css        # 样式（已优化 UI）
│   ├── components        # 公共组件
│   └── App.vue           # 根组件
├── vue.config.js         # 构建配置
├── package.json          # 项目元信息
├── vercel.json           # Vercel 部署配置 ✅
```

---

## 📄 License

MIT @ 本项目修改维护者