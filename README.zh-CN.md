> [English](README.md) | 中文

# TradingAgent Reports

TradingAgent 生成的研究报告资料库，按股票 ticker 和研究日期归档。

## 目录结构

```text
<TICKER>/
└── <YYYY-MM-DD>/
    └── reports/
        ├── final_trade_decision.md
        ├── trader_investment_plan.md
        ├── investment_plan.md
        ├── fundamentals_report.md
        ├── market_report.md
        ├── news_report.md
        └── sentiment_report.md
```

报告来自 TradingAgents 的 `results/<TICKER>/<YYYY-MM-DD>/reports/`，原样保留文件名和正文，仅归档人读 Markdown 报告。运行日志和缓存留在源目录。

阅读时可先看 `final_trade_decision.md`（最终结论），再看 `trader_investment_plan.md`（交易方案）、`investment_plan.md`（研究结论），按需阅读其余分析。

日期使用研究日期；同日内容不同的版本使用 `<YYYY-MM-DD>_HHMMSS` 目录保留，时间采用归档时的本地时间。保留原始研究内容；如需更正，另加注明日期的勘误。

## 贡献方式

补充报告、勘误或文档时，请 fork 本仓库，并提交以本仓库 `main` 为目标的 Pull Request，由维护者 review 后合并。本仓库仅维护 `main` 分支。

PR 标题简要写明动作和范围，例如 `Add TSLA research — 2026-09-07`。填写中英双语 [PR 模板](.github/pull_request_template.md)：勾选目的，用 1–3 句话解释本次改动与原因，并列出涉及的 ticker／日期或文件路径。说明可使用中文或英文。

## 使用说明与许可

报告由 AI 生成，可能包含事实错误、过时数据或未经验证的判断，仅供研究与学习，不构成投资建议，也不代表实际交易记录。

本仓库采用 [MIT License](LICENSE)。报告中引用的第三方资料仍归原权利人所有，不因归档而改变其授权。
