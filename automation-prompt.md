# Daily Automation Prompt

This repository is updated by a daily Codex automation.

## Schedule

- Run every day at 06:00 Asia/Shanghai.
- Target date is yesterday in Asia/Shanghai.

## Required behavior

1. Pull the latest `main` branch before editing.
2. Determine the target date as yesterday in Asia/Shanghai.
3. Collect only AI technology items published or materially updated during the target date, from 00:00 to 23:59 Asia/Shanghai.
4. Do not backfill with older news. If fewer than 20 qualified items exist, publish fewer than 20.
5. Prioritize models, APIs, open source projects, papers, developer tools, AI agents, image/video/multimodal generation, compute infrastructure, and safety evaluations.
6. Include image/video/multimodal technology items when there are qualified items on the target date.
7. Use discovery channels from `sources.md`, but every final `来源` must point to a concrete article, official blog post, paper page, technical report, system card, or GitHub project page.
8. Do not use home pages, channel pages, rankings, trending pages, search results, or daily aggregation pages as final sources.
9. Write the daily issue to `docs/YYYY/YYYY-MM-DD.md`.
10. Update `README.md` so the latest issue and archive point to the new file.
11. Commit and push to `main`.

## Daily issue format

```md
# AI 技术热点日报｜YYYY-MM-DD

筛选口径：只收录北京时间 YYYY-MM-DD 00:00-23:59 发布或实质更新的 AI 技术新闻。技术新闻优先，关注模型、API、开源项目、论文进展、AI agent、图像/视频/多模态生成、算力基础设施、开发者工具和安全评估。每条 `来源` 都指向具体页面。

## 1. 标题

2-4 句中文总结：发生了什么、技术重点是什么、为什么值得关注。

来源：https://example.com/concrete-page
```
