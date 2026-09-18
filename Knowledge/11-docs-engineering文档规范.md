# docs/engineering/ 文档规范

> Engineering Documentation Specification
> Version: 1.0

---

# 1. Purpose

`docs/engineering/` 用于保存：

> **具体产品项目的正式 Engineering Design。**

其上游输入来自：

```text
docs/product/
```

其下游用于指导：

```text
Implementation
Testing
Deployment
Operation
Maintenance
```

基本关系：

```text
docs/product/
    ↓
Engineering Design
    ↓
docs/engineering/
    ↓
Implementation
```

---

# 2. Ownership

`docs/product/`

主要回答：

```text
Why
Who
What
Product Behavior
Acceptance
```

`docs/engineering/`

主要回答：

```text
How
Architecture
Interfaces
Data
Infrastructure
Implementation
```

不得用 Engineering 文档悄悄修改已经确认的产品需求。

如果技术设计需要改变产品行为：

必须返回产品侧完成决策。

---

# 3. Small Project

对于简单项目，可以使用单文档：

```text
docs/engineering/
└── engineering-design.md
```

其中包含必要的：

* Architecture
* Tech Stack
* Modules
* Data
* Interfaces
* Security
* Deployment
* Testing
* Implementation Plan

不要为了形式强制拆文件。

---

# 4. Medium / Large Project

复杂项目建议：

```text
docs/engineering/
├── README.md
├── architecture.md
├── tech-stack.md
├── module-design.md
├── data-design.md
├── api-design.md
├── security.md
├── reliability.md
├── observability.md
├── deployment.md
├── testing-strategy.md
├── implementation-plan.md
├── decision-log.md
└── open-questions.md
```

根据项目实际情况裁剪。

---

# 5. README.md

作为 Engineering Design 入口。

建议包含：

```text
Engineering Design Status
Product Version
Current Architecture
Key Decisions
Document Index
Open Blockers
Implementation Status
```

避免让开发者不知道应该先读哪一份文件。

---

# 6. architecture.md

至少说明：

* System Context
* Architecture Overview
* Components
* Responsibilities
* Boundaries
* Communication
* External Dependencies
* Major Data Flow
* Major Trade-offs

适合使用 Mermaid：

* System Context
* Component Diagram
* Major Flow

---

# 7. tech-stack.md

记录重要技术选择：

```text
Technology
Purpose
Reason
Alternatives
Trade-offs
Constraints
```

不要只形成：

```text
Backend: Go
DB: PostgreSQL
Cache: Redis
```

而没有解释为什么。

---

# 8. module-design.md

记录：

```text
Module
Responsibility
Boundary
Inputs
Outputs
Dependencies
Important Rules
```

模块应能够追溯到真实产品能力。

避免：

> 为了架构优雅建立没有真实业务职责的模块。

---

# 9. data-design.md

根据项目复杂度包含：

* Domain Model
* Entity
* Value Object
* Relationship
* Ownership
* Persistence
* Transaction
* Consistency
* Data Lifecycle
* Migration
* Retention

只有当实施需要时进一步细化：

* Tables
* Indexes
* Constraints

---

# 10. api-design.md

根据需要包含：

* Interface Boundary
* Endpoint / RPC
* Request
* Response
* Error Model
* Authentication
* Authorization
* Idempotency
* Pagination
* Versioning

正式 API Contract 如果规模较大，可以单独维护 OpenAPI / Proto 等机器可读规范。

避免 Markdown 与正式 Schema 重复维护全部接口细节。

---

# 11. security.md

根据实际风险说明：

* Threat Surface
* Authentication
* Authorization
* Sensitive Data
* Encryption
* Secret Management
* Audit
* Privacy
* Retention
* Abuse Prevention
* Security Assumptions

---

# 12. reliability.md

根据风险考虑：

```text
Failure Scenario
Impact
Detection
Recovery
Retry
Timeout
Fallback
Idempotency
```

简单系统可以合并进 `architecture.md`。

---

# 13. observability.md

根据项目需要定义：

* Application Logs
* Audit Logs
* Metrics
* Traces
* Alerts
* Business Metrics
* SLO / SLI

不得为了文档完整虚构没有实际运维需求的 SLO。

---

# 14. deployment.md

记录：

* Environment
* Build
* Configuration
* Infrastructure
* Deployment Flow
* Database Migration
* Rollback
* Release Strategy
* Secrets
* Operational Dependencies

---

# 15. testing-strategy.md

测试策略应从：

```text
Product Acceptance Criteria
+
Engineering Risk
```

推导。

根据项目需要覆盖：

* Unit
* Integration
* Contract
* E2E
* Security
* Performance
* Migration
* Failure / Recovery

重点明确：

> 哪些核心业务风险必须通过哪一层测试验证。

---

# 16. implementation-plan.md

Implementation Plan 不是简单 TODO List。

建议按可交付增量组织：

```text
Phase / Milestone
Goal
Scope
Dependencies
Major Tasks
Verification
Risks
Exit Criteria
```

优先形成：

```text
Walking Skeleton
↓
Core Happy Path
↓
Critical Business Rules
↓
Critical Exceptions
↓
Supporting Capabilities
↓
Secondary Features
↓
Hardening
```

---

# 17. decision-log.md

重要技术决策记录：

```text
Decision ID
Date
Context
Decision
Alternatives
Reason
Trade-offs
Consequences
Status
```

如果团队使用 ADR：

可以改为：

```text
docs/engineering/adr/
```

并避免与 `decision-log.md` 重复维护。

---

# 18. open-questions.md

记录尚未解决的 Engineering Question：

```text
Question
Area
Why It Matters
Owner
Blocking / Non-blocking
Options
Status
Resolution
```

涉及产品行为的问题必须标记：

> Product Clarification Required

而不是由 Engineering Agent 自行定义产品规则。

---

# 19. Source of Truth

遵守：

> **One Fact, One Primary Source of Truth**

不要：

* 在 architecture.md 和 module-design.md 重复维护整个模块定义；
* 在 README.md 再复制所有 Engineering Design；
* 同时维护多个相互独立的 API 定义；
* 创建大量 final / latest 文件。

README 用于导航。

专项文件用于详细定义。

机器可读规范优先作为接口等内容的最终 Source of Truth。

---

# 20. Naming

默认：

```text
lowercase-kebab-case.md
```

例如：

```text
architecture.md
data-design.md
testing-strategy.md
implementation-plan.md
```

不要默认：

```text
architecture-v2.md
architecture-final.md
architecture-new.md
```

版本由 Git 管理。

---

# 21. Traceability

重要 Engineering Decision 应能够追溯到至少一种来源：

```text
Product Requirement
Non-functional Requirement
Engineering Constraint
Risk
Existing Repository Constraint
```

不能解释来源的复杂设计：

> 默认应受到质疑。

---

# 22. Engineering Artifact Rule

遵守：

> Update Before Create.

已有正式 Engineering Artifact 时优先更新。

不要在每轮 Codex 会话中重新创建一套架构文档。

---

# 23. Architecture Change

进入开发后发现重大技术问题，需要修改 Architecture 时：

记录：

```text
Reason
Affected Components
Product Impact
Migration Impact
Risk
Decision
```

重大变更同时更新：

* architecture.md
* decision-log.md
* implementation-plan.md

以及相关专项文档。

---

# 24. READY FOR IMPLEMENTATION

进入正式 Implementation 前至少确认：

## Requirement

* Product Delivery Package 已读取；
* MVP Scope 明确；
* Product / Engineering 无重大冲突。

## Architecture

* System Boundary 明确；
* Components / Modules 职责明确；
* 关键依赖明确。

## Data / Interface

* 核心数据模型可支持业务；
* 核心接口边界明确。

## Risk

* Security / Reliability 重大风险已处理；
* Blocking Engineering Question = 0。

## Verification

* Testing Strategy 可验证核心需求。

## Delivery

* Deployment / Migration 基本可执行；
* Implementation Plan 可执行。

满足：

> **READY FOR IMPLEMENTATION**

否则：

> **NOT READY FOR IMPLEMENTATION**

并列出 Blocking Issues。

---

# 25. Final Principle

`docs/engineering/` 的价值不是：

> 让项目看起来拥有很多架构文档。

而是：

> **把已经确认的产品需求转换成研发团队能够稳定理解、实现、测试、部署和维护的工程决策。**

复杂度必须服务实际问题。

没有真实需求支撑的复杂设计，应默认受到质疑。
