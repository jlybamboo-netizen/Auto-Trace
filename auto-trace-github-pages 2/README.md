# AUTO TRACE · GitHub Pages 部署包

这是可直接部署到 GitHub Pages 的静态版本，无需 Node.js、数据库或服务器。

## 首次部署

1. 在 GitHub 新建一个仓库，建议命名为 `auto-trace`。
2. 解压本部署包，把包内全部文件上传到仓库的 `main` 分支。
3. 打开仓库的 **Settings → Pages**。
4. 在 **Build and deployment → Source** 中选择 **GitHub Actions**。
5. 打开仓库的 **Actions** 页面；`Deploy AUTO TRACE to GitHub Pages` 完成后即可获得公开网址。

后续只要更新 `site/index.html` 并推送到 `main`，GitHub Pages 会自动重新发布。

## 数据说明

- 当前快照日期：2026-09-14。
- Apple App Store 版本记录作为更新锚点。
- 品牌官方信息可作为单一确认来源。
- 新闻媒体需要至少两个独立来源交叉核验。
- 高热自媒体只作为待核验线索，不参与热度或节点颜色计算。
- 无可靠来源时保留“暂无符合门槛的补充来源”，不推测或编写更新内容。
- 车辆 OTA 只有在直接改变 App 或 Web 任务流程时才纳入。

## 每周更新

Codex 周期任务会在每周一 09:00（北京时间）检查新版本与来源，并重新生成此部署包。要让更新自动推送到你的 GitHub Pages，请在仓库创建完成后，把仓库地址发给 Codex；在此之前，新包需要手动上传。

## 文件结构

- `site/index.html`：站点主页面和数据快照。
- `site/favicon.svg`：站点图标。
- `site/social-preview.png`：分享预览图。
- `.github/workflows/deploy-pages.yml`：GitHub Pages 自动部署流程。
