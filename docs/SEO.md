---
published: false
---

# Portal SEO 与流量提升策略

> 收录只是"能被找到"，涨流量要主动出击。本文汇总 DoodleLanguage 等应用的 Portal（https://sidneywang.github.io/portal/）可落地的流量策略。
> 最后更新：2026-07-16

## 0. 已完成的收录基础（前提）

- `sitemap.xml`：32 个 URL（中英文全部页面），部署于 `https://sidneywang.github.io/portal/sitemap.xml`
- `robots.txt`：允许全部抓取，指向 sitemap
- Google Search Console：已用 **HTML 文件验证**（`google43d99698ef665407.html` 已部署并验证通过）
- Bing Webmaster Tools：经 **Google Search Console 导入**完成验证
- Baidu（百度搜索资源平台）：被 `github.io` 主域配额限制，暂未完成（见第 5 节）

待办：在 GSC / Bing 后台**提交 sitemap URL**；对重点页（如 `/portal/DoodleLanguage/`）点"请求编入索引"。

## 1. 应用商店本身（最大流量源）

Portal 只是落地页，真实流量在 App Store。

- **ASO**：标题 / 关键词 / 截图 / 描述持续打磨；DoodleLanguage 支持 7 种语言，每个 locale 的关键词需分别优化。
- **评分**：App 内引导评分；Portal 的隐私/支持页放"去评分"链接。
- **推荐**：新功能 / 大版本可申 App Store Today 推荐，或做限时免费。

## 2. 站外引流（效果最直接）

- **Product Hunt** 首发 / 重启，配 Portal 链接。
- **社区**：Hacker News、Reddit（r/SideProject、r/iOSProgramming）、开发者论坛、GitHub README 链回 Portal。
- **中文阵地**：DoodleLanguage 有中文受众，**小红书 / 抖音 / 微博** 种草比搜索引擎更管用。
- **外链**：alternativeto.net 等目录提交；写 dev.to / Medium 教程文（如"用画画学英语"）反向链 Portal。外链是 SEO 排名核心因子。

## 3. 内容

- 给 Portal 加**博客 / 教程**（Jekyll 原生支持），持续产出来自搜索的长尾流量，也天然产生外链。
- 每个 App 页面补 FAQ / 使用场景，覆盖更多搜索词。

## 4. 技术增强（仓库内可改项）

| 项 | 说明 | 状态 |
|----|------|------|
| JSON-LD `SoftwareApplication` | 每产品页加 name/操作系统/价格/评分 schema → Google 富媒体摘要，提升 CTR | 待做 |
| IndexNow | 内容更新主动通知 Bing，秒级收录 | 待做 |
| 分析工具 | 接 GA4 或隐私友好 Plausible（head.html 已预留 `site.google_analytics` 开关） | 待做 |
| `og:image` | 每页设 App 图标 / 首图为分享预览图（微信 / X） | 待做 |
| 显式 `hreflang` | 中英文互链，Google 按地区分发，避免重复内容 | 待做 |

## 5. 百度（主域配额问题）

百度把 `sidneywang.github.io` 归到共享主域 `github.io`，账号下 `*.github.io` 站点数超限，无法再加 `/portal/`。

可选方案：

1. **自定义域名（正解）**：用自有域名（如 `apps.sidneywang.com`）CNAME 到 GitHub Pages，仓库加 `CNAME` + 改 `_config.yml` 的 `url`。百度主域变为自有域名，配额独立。
2. **腾配额**：百度后台删掉几个不要的 `github.io` 站点再试。
3. **跳过**：Google + Bing 已覆盖绝大多数流量；百度对 `github.io` 抓取慢、收录弱，ROI 不高。

## 6. 优先级建议

1. 接**分析工具**（先看清流量来源）
2. 加 **JSON-LD**（零风险提升 CTR）
3. 做一波 **Product Hunt + 小红书** 站外
4. 再补 IndexNow / 博客

## 7. 核对清单

- [ ] GSC 提交 sitemap
- [ ] Bing 提交 sitemap
- [ ] GSC 对 DoodleLanguage 页请求编入索引
- [ ] 加 JSON-LD
- [ ] 接分析工具
- [ ] 设 `og:image`
- [ ] 百度：决定跳过 / 自定义域名 / 腾配额
- [ ] Product Hunt / 小红书 推广
