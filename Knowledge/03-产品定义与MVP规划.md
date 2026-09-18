# 产品定义与 MVP 规划

> Product Definition & MVP Planning  
> Version: 1.0

---

# 1. 文档目的

本文档定义 AI 产品经理在完成需求调研与需求分析后，如何进一步完成：

* 产品定位
* 产品愿景
* 目标用户定义
* 核心场景定义
* 核心价值主张
* 产品边界
* 成功指标
* MVP 范围
* 需求优先级
* 版本规划
* Roadmap

本文档主要解决两个核心问题：

1. **我们到底要做一个什么产品？**
2. **第一版到底做到什么程度？**

产品定义解决的是“方向”。

MVP 规划解决的是“范围”。

两者共同决定：

> 产品团队接下来应该聚焦什么，以及明确不做什么。

---

# 2. 前置条件

进入产品定义与 MVP 规划阶段前，应至少具备以下信息：

* 核心用户基本明确
* 核心场景基本明确
* 核心 Pain Point 基本明确
* Root Cause 已有合理判断
* 用户价值基本成立
* 业务价值基本成立
* 主要产品假设已经被识别
* 核心需求和非核心需求已有初步区分

如果上述信息仍非常模糊，应返回：

> 需求调研 / Requirement Research

或：

> 需求分析 / Requirement Analysis

不要在问题尚未理解时仓促定义产品。

---

# 3. 产品定义的核心逻辑

产品定义应沿着以下链路形成：

```text
Target User
↓
Core Scenario
↓
Core Problem
↓
Desired Outcome
↓
Value Proposition
↓
Product Capability
↓
Product Boundary
↓
Success Metric
```

不能反过来：

```text
已有技术
↓
想到功能
↓
拼成产品
```

除非项目本身属于明确的技术驱动型创新，并且已经验证存在真实需求。

---

# 4. Product Vision

## 4.1 产品愿景是什么

Product Vision 用于回答：

> 我们希望长期创造什么价值？

它不是详细功能描述。

也不是一句营销口号。

一个好的 Product Vision 应体现：

* 给谁创造价值
* 解决什么核心问题
* 希望形成什么长期价值

---

## 4.2 推荐表达方式

推荐格式：

> 为【目标用户】，在【核心场景】下，通过【核心能力】，解决【核心问题】，帮助用户获得【核心价值】。

例如：

> 为需要频繁处理客户咨询的中小商家，通过 AI 辅助理解客户意图、生成高质量回复和沉淀客户信息，减少重复沟通成本，提高服务效率与客户转化。

---

## 4.3 Vision 不应包含过多实现细节

不推荐：

> 做一个 React + Node.js + GPT-5 的客服系统。

这是技术方案，不是产品愿景。

---

# 5. Product Positioning

## 5.1 产品定位

产品定位回答：

> 这个产品在用户心智里到底是什么？

通常包含：

* 产品类别
* 目标用户
* 核心问题
* 核心价值
* 主要差异化

---

## 5.2 Positioning Template

可以使用：

> For [目标用户]
> Who [存在某类问题]
> The [产品名称]
> Is a [产品类别]
> That [核心价值]
> Unlike [当前替代方案]
> Our product [核心差异]

---

## 5.3 示例

```text
For:
经常需要处理大量客户消息的中小商家

Who:
回复耗时、质量不稳定、客户信息容易遗漏

The:
AI Customer Assistant

Is a:
AI 客户沟通辅助工具

That:
帮助用户快速理解客户问题并生成高质量回复

Unlike:
纯人工回复或普通模板回复工具

Our Product:
能够结合上下文和客户历史信息进行智能辅助
```

---

# 6. Target User

## 6.1 核心用户必须具体

不要定义：

> “所有互联网用户。”

也不要定义：

> “所有需要提高效率的人。”

这样的目标用户几乎没有产品指导价值。

---

## 6.2 用户分层

建议至少区分：

### Primary User

核心用户。

产品首先为其优化。

### Secondary User

次要用户。

会使用产品，但不是最主要服务对象。

### Stakeholder

可能不直接使用产品，但受到产品影响。

例如：

* 管理员
* 老板
* 财务
* 审计
* IT

---

## 6.3 用户选择标准

判断某类用户是否应该作为核心用户，可以考虑：

* 问题是否高频
* Pain Point 是否严重
* 当前替代方案是否差
* 是否愿意尝试新方案
* 是否具有商业价值
* 是否适合 MVP 快速验证

---

# 7. Core Scenario

## 7.1 场景比用户画像更重要

产品设计中，不能只知道：

> 用户是谁。

还必须知道：

> 用户在什么情况下需要产品。

---

## 7.2 场景描述模板

```text
Actor:
谁

Context:
处于什么环境

Trigger:
什么事情发生

Goal:
想完成什么

Pain Point:
哪里困难

Desired Outcome:
希望得到什么结果
```

---

## 7.3 核心场景标准

核心场景通常应该满足：

* 高频
* 高价值
* 高痛点
* 与产品长期定位一致

不是所有用户场景都应该进入 MVP。

---

# 8. Core Problem

产品必须明确：

> 最核心的问题到底是什么？

推荐写成：

> [目标用户] 在 [核心场景] 中，因为 [Root Cause]，导致 [问题/损失]。

例如：

> 运营人员在每周制作经营周报时，因为系统缺乏面向分析场景的数据聚合能力，导致需要大量手工整理数据，耗时且容易出错。

---

# 9. Desired Outcome

产品最终不是为了“提供功能”。

而是为了让用户获得某种结果。

例如：

不是：

> 提供自动报表。

而是：

> 将周报制作时间从 2 小时降低到 15 分钟。

Desired Outcome 应尽可能：

* 明确
* 可观察
* 可衡量

---

# 10. Value Proposition

## 10.1 用户价值

回答：

> 为什么用户愿意使用这个产品？

常见用户价值：

* 更快
* 更简单
* 更准确
* 更安全
* 更便宜
* 更智能
* 更可控
* 更省心
* 更容易协作
* 获得此前无法获得的能力

---

## 10.2 业务价值

回答：

> 为什么公司值得做这个产品？

常见业务价值：

* 收入增长
* 转化提升
* 留存提升
* 客单价提升
* 成本下降
* 人效提升
* 风险降低
* 战略布局
* 数据沉淀
* 用户增长

---

# 11. Product Principles

为产品定义少量长期设计原则。

例如：

```text
1. 用户始终拥有最终控制权
2. 默认减少操作步骤
3. 不为了智能化牺牲可解释性
4. 核心任务优先于扩展能力
5. 重要操作必须可恢复
```

Product Principles 用于后续出现方案冲突时辅助判断。

不要写十几条空泛口号。

建议：

> 3～7 条。

---

# 12. Product Boundary

## 12.1 产品边界必须明确

产品定义不仅要回答：

> 我们做什么？

还要回答：

> 我们不做什么？

---

## 12.2 建议定义

### In Product

属于产品核心职责。

### Adjacent

与产品有关，但不是当前核心。

### Out of Product

明确不承担。

---

## 12.3 示例

```text
产品负责：
- 理解聊天上下文
- 辅助生成回复
- 帮助用户组织表达

产品暂不负责：
- 自动发送消息
- 社交关系 CRM
- 长期自动运营联系人

产品明确不负责：
- 冒充用户自主对外沟通
```

边界能够有效防止：

> 产品做着做着变成一个什么都做的平台。

---

# 13. Product Anti-Goals

建议为复杂产品明确：

> Anti-Goals / 非目标。

例如：

```text
本产品当前不追求：
- 覆盖所有 IM 平台
- 自动替用户作出关系决策
- 完全取代人工沟通
```

Anti-Goals 可以有效减少后续需求争议。

---

# 14. Product Capability

产品能力是：

> 为解决核心问题，产品必须具备的稳定能力。

它不同于页面，也不同于具体功能。

例如：

```text
需求：
帮助用户快速回复客户

能力可能包括：

Context Understanding
Reply Generation
Knowledge Retrieval
Tone Control
Customer Context
```

再往下才是具体 Feature。

---

# 15. Product Hypothesis

早期产品本质上是一组假设。

例如：

```text
H1:
用户确实因为回复客户耗时而痛苦

H2:
AI 生成回复能显著降低回复时间

H3:
用户愿意把聊天上下文提供给 AI

H4:
用户认为 AI 建议的质量足够可信
```

产品经理应主动把隐含假设显性化。

---

# 16. 核心假设优先级

可以按照：

```text
Risk =
Importance × Uncertainty
```

判断。

最危险的不是：

> 小问题但不确定。

而是：

> 对产品生死极其重要，同时又高度不确定的假设。

这些假设应该优先验证。

---

# 17. Success Metrics

## 17.1 为什么需要成功指标

如果无法回答：

> 上线后怎样知道产品做对了？

那么产品目标很可能仍然模糊。

---

## 17.2 指标层级

### Business Metrics

例如：

* 收入
* GMV
* 毛利
* CAC
* LTV

### Product Metrics

例如：

* Activation
* Retention
* Conversion
* Task Success Rate

### User Outcome Metrics

例如：

* 完成任务时间下降
* 错误率下降
* 回复效率提高

---

# 18. North Star Metric

North Star Metric 应尽量反映：

> 用户持续获得核心价值。

例如：

不是简单：

> DAU。

而可能是：

> 每周通过 AI 成功完成的有效客户回复数量。

北极星指标不是每个项目都必须定义。

小型内部工具可能只需要明确关键 Outcome Metrics。

---

# 19. Guardrail Metrics

产品优化某个指标时，可能伤害其他指标。

因此必要时定义 Guardrail Metrics。

例如：

目标：

> 提高 AI 自动回复采纳率。

Guardrail：

* 用户投诉率
* 错误回复率
* 编辑修改比例
* 撤回率

避免：

> 一个指标变漂亮，产品反而变差。

---

# 20. MVP 的真正定义

MVP：

> Minimum Viable Product

不是：

> 最少功能产品。

而是：

> 能够验证核心价值假设的最小可行产品闭环。

---

# 21. MVP 必须验证什么

至少应该验证以下一个或多个关键问题：

* 用户是否真的有这个问题？
* 用户是否愿意尝试新方案？
* 产品是否能够解决问题？
* 用户是否愿意持续使用？
* 用户是否愿意付费？
* 产品是否具备商业可行性？

---

# 22. MVP 的最小闭环

一个合格 MVP 应满足：

```text
用户进入
↓
完成核心行为
↓
获得核心价值
↓
产生可观察结果
```

而不是：

```text
做了很多基础模块
但用户还无法完成核心任务
```

---

# 23. MVP 不是 Demo

Demo 可以证明：

> 技术能做出来。

MVP 应该验证：

> 用户愿不愿意用，以及有没有价值。

---

# 24. MVP 不是 Prototype

Prototype 主要验证：

* 交互
* 理解
* 用户路径
* 方案反馈

MVP 则需要让真实用户：

> 真正完成核心任务。

---

# 25. MVP 不是 V1.0 的缩水版

错误思路：

```text
完整产品有 100 个功能
↓
砍掉 70 个
↓
剩下 30 个 = MVP
```

正确思路：

```text
核心问题是什么
↓
最小价值闭环是什么
↓
验证需要什么能力
↓
只做这些
```

---

# 26. MVP 规划流程

建议按照：

```text
Core User
↓
Core Problem
↓
Core Value
↓
Core Journey
↓
Critical User Stories
↓
Minimum Capabilities
↓
MVP Scope
```

---

# 27. Story Mapping 切 MVP

如果已经建立用户故事地图，可以使用：

```text
Backbone
用户核心活动

↓

Stories
具体用户故事

↓

Release Slice
MVP / Next / Later
```

MVP 应优先覆盖：

> 主干路径的最小完整纵向切片。

而不是先把某个模块横向做得特别完整。

---

# 28. Walking Skeleton

对于复杂软件，可以使用 Walking Skeleton 思路。

即：

> 先建立一条从前到后的最小业务链路。

例如电商：

```text
注册
↓
浏览商品
↓
下单
↓
支付
↓
订单完成
```

每个环节功能都可以很简单，但核心链路要通。

之后再逐步增强：

* 搜索
* 优惠券
* 推荐
* 售后
* 积分

---

# 29. MVP 功能判断问题

每个候选 Feature 都问：

1. 不做它，核心用户还能获得核心价值吗？
2. 不做它，核心业务闭环还能成立吗？
3. 它是在验证核心假设吗？
4. 它是解决当前问题，还是为了未来扩展？
5. 是否已有低成本替代方案？
6. 它是否只是“看起来应该有”？

如果大量答案指向：

> 不影响核心价值。

通常不应该进入 MVP。

---

# 30. Must / Should / Could / Won't

推荐使用 MoSCoW。

## Must

如果没有：

* 核心价值无法成立
* 核心流程无法闭环
* 存在不可接受风险

才能算 Must。

---

## Should

价值较高，但没有它 MVP 仍可运行。

---

## Could

体验增强或边缘场景。

---

## Won't

当前版本明确不做。

Won't 非常重要。

必须把：

> “以后可能做”

和：

> “现在必须做”

分开。

---

# 31. P0 / P1 / P2 / P3

可与 MoSCoW 配合。

## P0

核心闭环、法律安全、严重风险。

## P1

近期高价值核心需求。

## P2

次级价值或体验完善。

## P3

边缘需求、长期增强。

---

# 32. RICE

需求较多时可使用：

```text
RICE =
Reach × Impact × Confidence
─────────────────────────
Effort
```

用于辅助排序。

不要机械相信计算结果。

例如：

* 法规要求
* 安全问题
* 战略项目
* 关键客户承诺

可能需要人工 override。

---

# 33. Value / Effort Matrix

快速决策时可以使用：

```text
             High Value

       Quick Win | Strategic
                 |
Low Effort ------+------ High Effort
                 |
       Fill-in   | Avoid
                 
             Low Value
```

优先：

> High Value + Low Effort

谨慎：

> Low Value + High Effort

---

# 34. Kano

体验型产品可辅助区分：

## Basic

没有会强烈不满。

## Performance

越多越满意。

## Delight

没有不会抱怨，但有会惊喜。

MVP 一般优先：

> Basic + 最关键 Performance。

不要在核心问题未解决时大量投入 Delight。

---

# 35. Scope 定义

## 35.1 In Scope

当前版本明确实现。

每条建议尽可能说明：

* User Story
* Value
* Priority
* Reason

---

## 35.2 Out of Scope

当前版本明确不实现。

同时说明：

> Why Not Now

例如：

```text
功能：
自动发送 AI 回复

Out of Scope Reason：
当前阶段需要优先验证用户是否信任 AI 建议，自动发送会增加风险并掩盖真正价值验证。
```

---

# 36. MVP Scope Template

```markdown
# MVP Scope

## Core User

## Core Scenario

## Core Problem

## Core Value

## Core Hypothesis

## MVP Goal

## In Scope

| Feature | User Story | Value | Priority | Reason |
|---|---|---|---|---|

## Out of Scope

| Feature | Reason | Revisit Condition |
|---|---|---|

## Critical Dependencies

## Risks

## Success Metrics
```

---

# 37. Release Planning

推荐结构：

```text
MVP
↓
V1.1
↓
V1.5
↓
V2.0
```

不要提前规划过细。

未来越远：

> 规划越应该保持模糊。

---

# 38. MVP

目标：

> 验证核心价值。

特点：

* 极度聚焦
* 核心闭环
* 最少必要能力
* 快速获得真实反馈

---

# 39. V1.1

通常处理：

* 核心体验优化
* 高频反馈
* 明显 Bug
* 必要运营能力
* 数据完善

---

# 40. V1.5

通常可能加入：

* 次级场景
* 效率增强
* 用户增长能力
* 管理能力
* 商业化探索

---

# 41. V2.0

适合：

* 产品能力扩展
* 新用户群体
* 新商业模式
* 重大架构升级
* 平台化

---

# 42. Roadmap 不是承诺表

Roadmap 应表达：

> 当前战略判断。

不是：

> 一年后的绝对合同。

建议区分：

```text
Now
Next
Later
```

比硬写：

```text
2027 年 7 月 18 日上线功能 X
```

更适合早期产品。

---

# 43. Now / Next / Later

## Now

已经确认并正在执行。

## Next

较高置信度的下一阶段方向。

## Later

探索方向，不代表承诺。

---

# 44. Roadmap Template

```markdown
# Product Roadmap

## Now

### Goal

### Scope

### Key Metrics

---

## Next

### Goal

### Candidate Capabilities

### Conditions

---

## Later

### Opportunities

### Assumptions
```

---

# 45. Product Definition Template

```markdown
# Product Definition

## 1. Product Name

## 2. Background

## 3. Target User

### Primary User

### Secondary User

### Stakeholders

## 4. Core Scenario

## 5. Core Problem

## 6. Desired Outcome

## 7. Product Vision

## 8. Product Positioning

## 9. Value Proposition

### User Value

### Business Value

## 10. Product Principles

## 11. Product Boundary

### In Product

### Adjacent

### Out of Product

## 12. Anti-Goals

## 13. Core Product Capabilities

## 14. Key Hypotheses

## 15. Success Metrics

### North Star Metric

### Supporting Metrics

### Guardrail Metrics

## 16. Risks

## 17. Open Questions
```

---

# 46. MVP Planning Template

```markdown
# MVP Planning

## 1. MVP Objective

## 2. Core User

## 3. Core Scenario

## 4. Core Problem

## 5. Core Value

## 6. Critical Hypotheses

## 7. Core Journey

## 8. MVP Scope

### Must

### Should

### Could

### Won't

## 9. In Scope

## 10. Out of Scope

## 11. Dependencies

## 12. Risks

## 13. Success Metrics

## 14. Validation Plan

## 15. Release Recommendation
```

---

# 47. 常见产品定义错误

## 47.1 用户太泛

例如：

> 所有人。

导致产品无法聚焦。

---

## 47.2 场景太泛

例如：

> 提高工作效率。

需要继续具体化。

---

## 47.3 把功能当价值

例如：

> 核心价值是拥有 AI Chatbot。

AI Chatbot 是能力或方案。

价值应该是：

> 更快解决问题。

---

## 47.4 产品边界缺失

最后变成：

> 什么需求都能加。

---

## 47.5 目标和指标脱节

产品目标：

> 提高效率。

指标却只有：

> DAU。

需要建立合理因果关系。

---

# 48. 常见 MVP 错误

## 48.1 MVP 大而全

因为团队担心：

> “没有这个用户体验不好。”

结果第一版半年都出不来。

---

## 48.2 MVP 不闭环

做了一堆模块，但核心任务无法完成。

---

## 48.3 把后台管理做得比用户价值还完整

早期产品经常出现：

> 用户端核心能力还没验证，后台已经有 12 个菜单。

---

## 48.4 为未来扩展提前设计太多

例如：

> “以后可能国际化，所以第一版就做 14 种语言。”

属于典型 premature optimization。

---

## 48.5 MVP 只验证技术

技术跑通不等于产品成立。

---

# 49. Scope Creep 控制

新增需求进入当前版本前必须回答：

```text
这个需求：

1. 是否解决当前核心问题？
2. 是否属于核心用户？
3. 是否属于 MVP 核心路径？
4. 是否影响当前 Success Metric？
5. 不做是否影响闭环？
6. 为什么一定要现在做？
```

如果无法给出充分理由：

> 默认不进入当前 Scope。

---

# 50. Change Control

当项目进行中提出新需求时，记录：

```text
Change Request

Reason

Impact

Scope Impact

Schedule Impact

Risk

Decision
```

产品经理不能每周换一次 MVP。

除非新证据证明原假设错误。

---

# 51. 产品假设验证

对关键假设明确：

```text
Hypothesis

Evidence Needed

Validation Method

Success Criteria

Failure Criteria

Decision
```

例如：

```text
Hypothesis:
用户愿意使用 AI 回复建议。

Validation:
真实用户试用。

Success:
≥40% AI 建议被直接采用或少量编辑后采用。

Failure:
大量用户查看后放弃使用。
```

---

# 52. Kill Criteria

成熟的 MVP 规划应该允许：

> 项目验证失败。

必要时提前定义：

```text
如果出现以下情况，则重新评估或停止：

- 核心用户问题不成立
- 使用频率远低于预期
- 用户不愿采用新方案
- 核心技术成本无法接受
- 商业价值无法成立
```

MVP 的目的不是：

> 证明我们一定是对的。

而是：

> 尽快知道我们到底对不对。

---

# 53. Pivot Criteria

如果核心假设部分成立，但产品方向不对，可以考虑 Pivot。

常见 Pivot：

* 用户群体变化
* 核心场景变化
* 产品形态变化
* 商业模式变化
* 渠道变化

Pivot 必须基于新证据，不应只是团队情绪变化。

---

# 54. 产品定义阶段的 AI 提问策略

当信息不充分时，应优先追问：

1. 谁是最核心用户？
2. 哪个场景最值得优先解决？
3. 用户最痛的一个问题是什么？
4. 如果只能解决一个问题，会选哪个？
5. 用户当前为什么会选择现有方案？
6. 产品成功后，用户行为会发生什么变化？
7. 什么指标可以证明我们真正创造了价值？

---

# 55. MVP 阶段的 AI 质疑策略

面对候选功能，主动问：

> 这个功能为什么必须第一版做？

> 不做它，核心闭环真的无法成立吗？

> 是用户价值需要它，还是团队觉得产品“应该有”？

> 是否存在人工或低成本替代方案？

> 它是在验证核心假设，还是在提前建设未来能力？

---

# 56. Product Definition Gate

进入用户故事地图或 MVP 深化前检查：

## User

* [ ] Primary User 明确
* [ ] Secondary User 已区分

## Problem

* [ ] Core Problem 清晰
* [ ] Root Cause 基本明确

## Scenario

* [ ] Core Scenario 明确

## Value

* [ ] User Value 明确
* [ ] Business Value 明确

## Product

* [ ] Product Vision 明确
* [ ] Product Positioning 明确
* [ ] Product Boundary 明确
* [ ] Anti-Goals 明确

## Metrics

* [ ] Success Metrics 基本明确

## Risk

* [ ] Key Hypotheses 已识别
* [ ] 重大风险已记录

满足：

> READY FOR MVP PLANNING

---

# 57. MVP Gate

进入产品功能架构前检查：

## Core Loop

* [ ] MVP 能完成核心业务闭环
* [ ] 用户能实际获得核心价值

## Scope

* [ ] In Scope 明确
* [ ] Out of Scope 明确
* [ ] Must 与 Should 已区分

## Validation

* [ ] MVP 明确要验证什么
* [ ] Success Criteria 明确

## Complexity

* [ ] 已删除非必要能力
* [ ] 没有明显过度设计

## Dependency

* [ ] 关键依赖明确

## Risk

* [ ] 关键风险可接受
* [ ] 高风险假设有验证方案

满足：

> READY FOR PRODUCT ARCHITECTURE

否则：

> CONTINUE MVP PLANNING

---

# 58. 阶段输出建议

完成本阶段后建议输出：

```text
Current Phase

Product Definition / MVP Planning

Product Vision

Target User

Core Scenario

Core Problem

Value Proposition

Product Boundary

MVP Goal

In Scope

Out of Scope

Key Hypotheses

Success Metrics

Risks

Open Questions

Gate Result

Next
```

---

# 59. 最终工作原则

产品定义的核心不是：

> 给产品写一句漂亮的宣传语。

而是：

> **明确为谁解决什么问题，以及这个产品到底应该承担什么职责。**

MVP 规划的核心不是：

> 尽可能少做功能。

而是：

> **用最小成本构建完整价值闭环，并验证最关键的产品假设。**

始终牢记：

> 不明确目标用户，就无法真正定义产品。

> 不明确产品边界，功能一定会持续膨胀。

> 不明确 MVP 要验证什么，就无法判断第一版是否成功。

> 不写 Out of Scope，Scope Creep 几乎一定发生。

> MVP 的价值不是让团队更快“上线一个东西”，而是让团队更快获得真实世界的答案。
