# Research Reports

公开的深度调研报告集合。纯静态 HTML,托管于 Cloudflare Pages。

**线上地址**:https://paperblue-research.pages.dev/
**Cloudflare 项目名**:`paperblue-research`(账号 zayenwang.dev)
**GitHub**:https://github.com/Paper-blue/research-reports

## 发布一篇新报告(由 skill `内容-调研报告发布` 执行)

1. 把新 HTML 放进 `reports/`,用英文/拼音文件名
2. 在 `index.html` 列表区加一张卡片
3. **过脱敏检查**(脚本在 skill 里,无命中才能发)
4. 存档:`git add . && git commit -m "add: 标题" && git push`
5. 部署(这步才上线):
   ```
   wrangler pages deploy . --project-name=paperblue-research --branch=main --commit-dirty=true
   ```

> 当前是 wrangler 直传,非 git 自动部署。想改自动:Cloudflare 后台把项目连上本仓库。

## ⚠️ 隐私红线

**这是公开仓库。** 只放确定要公开的报告。不要放任何个人/理财/持仓/账户/密钥等敏感内容——上公网即可能被搜索引擎与缓存永久收录。
