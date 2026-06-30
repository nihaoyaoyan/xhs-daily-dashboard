# 小红书每日增长看板

这个仓库用于通过 GitHub Pages 发布每日生成的静态 HTML 看板。

## 发布方式

在 `xhs-qianfan-codex-mcp` 项目中生成日报：

```powershell
uv run xhs-qianfan-daily-report --stores config/stores.json --out reports
```

把生成的 `reports/YYYY-MM-DD-dashboard.html` 复制为本仓库根目录的 `index.html`，然后提交推送到 `main` 分支。GitHub Actions 会自动发布到 GitHub Pages。

## 注意

当前仓库是公开仓库。上传真实看板前，请确认页面中包含的计划 ID、搜索词、笔记和经营数据可以公开访问。
