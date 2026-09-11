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

`echarts.min.js` / `chart.umd.min.js` 与页面同级存放（站点自包含，不依赖 jsdelivr，国内外均可访问）。

## 效益评估口径

社会效益含 **4 个组分**（v5 起）：

```
S_t = V_protein + V_subsidy + V_carbon + V_women
V_protein = Y_t × α × ρ    蛋白产出
V_subsidy = δ × t          社会岗位收入
V_carbon  = Y_t × β        碳汇价值（β 正=碳汇 / 负=碳源）
V_women   = γ × t          女性占比收入价值   ← v5 新增
```

γ 即参数表中的「女性占比收入价值 γ gender（USD/(m²·d)）」。
如需与 R 原脚本输出严格对齐，把 γ 设为 0 即可还原旧口径。

> 公网版仅支持浏览/查看。搜索与「加入待确认」等写操作建议在本机实时工作台
> （`http://127.0.0.1:8787`）使用，避免互相覆盖。
