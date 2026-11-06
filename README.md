# LedgerCrew · 账清社

**一个人经营，一支 MiMo AI 财务团队交付。**

Junction China 2026 人工智能赛道参赛项目：为小型工作室提供票据整理、流水核对和异常说明服务，由一位老板统筹多个 AI Agent 完成接单、处理、审批和报告交付。

## 团队从这里开始

**[查看三人任务清单与 40 小时排期](docs/PLAN.md)**

| 成员 | 职责 | 领取任务 |
| --- | --- | --- |
| A：taiyi747 | 产品、前端、部署、用户体验与路演 | [前端任务 FE-01～FE-06](docs/PLAN.md#前端任务清单a) |
| B：后端队友 | API、数据库、对账规则、Worker、审批与恢复 | [后端任务 BE-01～BE-07](docs/PLAN.md#后端任务清单b) |
| C：AI 队友 | MiMo 接入、Microsoft Agent Framework、Agent 与工作流 | [AI 任务 AI-01～AI-07](docs/PLAN.md#ai-任务清单c) |

## 技术方案

- 前端：Next.js App Router、TypeScript、Tailwind CSS。
- 后端：Python 3.11、FastAPI、Pydantic 2、SQLite、SQLAlchemy 2、Alembic。
- AI：MiMo API、Microsoft Agent Framework Python SDK、WorkflowBuilder、FileCheckpointStorage。
- 部署：本地服务，通过公网隧道暴露 Next.js；Next.js 代理后端 API。

核心流程：**模拟下单 → 上传材料 → 识别票据 → 核对流水 → 人工处理异常 → 审核报告 → 客户领取。**

## 当前状态

当前仓库提供团队任务清单和协作约定，应用代码由三位成员按分工实现。请从各自的功能分支提交 PR，按照计划中的阶段验收完成联调。

首版交付账目核对报告和异常清单；体验交易明确标注为模拟交易。
