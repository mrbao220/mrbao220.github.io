# 个人简历网站（源码）

> 这是鲍俊一的个人简历主页源码，已提取到本地用于修改。

## 文件说明
- `index.html` —— 完整单文件站点。HTML / CSS（内联 `<style>`）/ JS（内联 `<script>`）全部在这一个文件里。
- 外部依赖走 CDN，无需本地资源：
  - Tailwind CSS：`https://cdn.tailwindcss.com`
  - 图标 Lucide：`https://unpkg.com/lucide@latest`
  - 字体 Google Fonts：Plus Jakarta Sans / Noto Serif SC / Zhi Mang Xing

## 如何修改
1. 直接用浏览器打开 `index.html` 即可预览。
2. 用任意编辑器（VS Code / Trae）修改 `index.html`，保存后刷新浏览器即可看到变化。
3. 常见修改点：正文文案直接在 HTML 里搜中文改；配色在 `<style>` 内的 CSS 变量 / Tailwind 类；动态效果在底部 `<script>`。

## 如何发布回 GitHub Pages
本机环境对 `github.com` 的 git 协议被网络代理拦截，无法在此直接 `git clone / push`。
请在能正常访问 GitHub 的环境下执行：

```bash
cd "个人网站trae版"
git init
git add index.html
git commit -m "update resume"
git branch -M main
git remote add origin https://github.com/mrbao220/mrbao220.github.io.git
git push -u origin main
```

推送后等待 GitHub Pages 自动部署（通常 1 分钟内），访问 https://mrbao220.github.io/ 查看更新。
