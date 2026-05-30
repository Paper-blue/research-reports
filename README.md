# Research Reports

公开的深度调研报告集合。纯静态 HTML,托管于 Cloudflare Pages,`git push` 自动部署。

## 发布一篇新报告(由 skill `内容-调研报告发布` 自动执行)

1. 把新 HTML 放进 `reports/`,用英文/拼音文件名
2. 在 `index.html` 列表区加一张卡片
3. **过脱敏检查**(`scripts/desensitize-scan.sh`,无命中才能发)
4. `git add . && git commit -m "add: 标题" && git push` → ~30s 上线

## ⚠️ 隐私红线

**这是公开仓库。** 只放确定要公开的报告。不要放任何个人/理财/持仓/账户/密钥等敏感内容——上公网即可能被搜索引擎与缓存永久收录。
