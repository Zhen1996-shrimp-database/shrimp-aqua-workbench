# 对虾养殖产业数据库工作台（永久只读公网版）

本站是对虾养殖产业数据库工作台的**只读公网快照**，用于向他人分享查看。

## 入口

| 页面 | 用途 |
|---|---|
| `index.html` | 工作台首页（导航到全部子页） |
| `benefit.html` | **效益评估**（参数编辑 · 一键应用修改 · 9 类分析图） |
| `benefit-offline.html` | 同上单文件版（内联 ECharts/Chart.js，断网可用 / 可邮件转发） |
| `database.html` | 主数据库浏览 |
| `newlit.html` | 新增文献 |
| `etl.html` | ETL 流水线 |
| `dedup.html` | 文献去重 |
| `review.html` | 复审 |
| `quality.html` | 质量评估 |
| `summary.html` | 摘要 |
| `schema.html` | 数据模式 |
| `search.html` | 检索 |

`lib/` 子目录存放 ECharts / Chart.js（站点自包含，不依赖 jsdelivr，国内外均可访问）。

> 公网版仅支持浏览/查看。搜索与「加入待确认」等写操作建议在本机实时工作台
> （`http://127.0.0.1:8787`）使用，避免互相覆盖。
