> [English](README.md) | 中文

# TradingAgent Reports

基于 **TradingAgent 生成的研究报告**建立的开放资料维护库，按股票 ticker 和研究日期持续归档，方便阅读、检索和比较不同时期的研究。GitHub 保存公开版本，本地文件夹作为同步副本；仓库仅使用 `main` 分支。

## 目录结构

```text
<TICKER>/
└── <TICKER>_<YYYYMMDD>/
    ├── complete_report.md    # 完整报告
    ├── 1_analysts/           # 分析师报告
    ├── 2_research/           # 多空研究与结论
    ├── 3_trading/            # 交易方案
    ├── 4_risk/               # 风险讨论
    └── 5_portfolio/          # 最终决策
```

日期使用报告自身的研究日期。保留 TradingAgent 的原始输出结构；新增研究放入对应日期目录，历史报告保留。同一天有多次研究时，在目录名后追加 `_HHMMSS` 区分。

## 已归档研究

| Ticker | 研究日期 | 完整报告 |
| --- | --- | --- |
| TSLA | 2026-09-07 | [查看报告](TSLA/TSLA_20260907/complete_report.md) |
| TTWO | 2026-09-07 | [查看报告](TTWO/TTWO_20260907/complete_report.md) |

## 维护与使用

新增报告后更新上方索引。维护时保留原始研究内容；如需更正，另加注明日期的勘误，便于追溯。

## 贡献方式

欢迎补充研究、提交勘误或改善资料索引。外部贡献者请 fork 本仓库，在自己的 fork 中修改，并提交 **以本仓库 `main` 为目标的 Pull Request**，由维护者 review 后合并。本仓库仅维护 `main` 分支。

PR 标题简要写明动作和范围，例如 `Add TSLA research — 2026-09-07`。填写自动加载的 [PR 模板](.github/pull_request_template.md)：勾选目的，用 1–3 句话解释本次改动与原因，并列出涉及的 ticker／日期或文件路径。说明可使用中文或英文。

## 使用说明与许可

报告由 AI 生成，可能包含事实错误、过时数据或未经验证的判断，仅供研究与学习，不构成投资建议，也不代表实际交易记录。

本仓库采用 [MIT License](LICENSE)。报告中引用的第三方资料仍归原权利人所有，不因归档而改变其授权。
