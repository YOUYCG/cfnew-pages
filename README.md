这是自动升级

> **⚠️ 重要：部署后请将兼容日期设置为 `2026-01-20`**
>
> **Pages 部署：**
> 1. 登录 [Cloudflare 控制台](https://dash.cloudflare.com/)
> 2. 进入 **Workers 和 Pages** → 选择你的 Pages 项目
> 3. 点击 **设置** → **运行时**
> 4. 找到 **兼容性日期**，选择 `2026-01-20`，点击 **保存**
> 5. 返回 **部署** → 对最新一次部署点 **重试部署**，让新日期生效
>
> **Worker 部署：**
> 1. 登录 [Cloudflare 控制台](https://dash.cloudflare.com/)
> 2. 进入 **Workers 和 Pages** → 选择你的 Worker
> 3. 点击 **设置** → **运行时**
> 4. 找到 **兼容性日期**，选择 `2026-01-20`，点击 **保存**
>
> 这个设置只用改一次，之后每 6 小时的自动同步不会动它。

## 此 Fork 的部署

- Cloudflare Pages 项目：`cfnew-pages`
- 生产分支：`main`
- 面板地址：`https://cfnew-pages-ab1.pages.dev/<UUID>`（UUID 保存在 Cloudflare 的 `u` 环境变量中，不要提交到仓库）
- KV 绑定名：`c`；命名空间：`cfnew-pages-config`
- GitHub Actions 每 6 小时检查一次上游 Release，也可手动运行。
