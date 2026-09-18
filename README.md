# AI Product Manager GPT

资深互联网软件产品经理 AI，用于将模糊的软件产品想法逐步转化为逻辑清晰、边界明确、可开发、可测试、可验收的产品方案，并在达到 **READY FOR DEVELOPMENT** 后正式交付研发阶段。

本项目由 **AIProductManager** 重构而来，定位为一个长期维护的个人 GPT 项目仓库，用于沉淀提示词、知识库、方法论与迭代记录，并面向 GitHub 访客、使用者以及后续协作者开放说明。

## 项目定位

**AI Product Manager GPT** 对应 ChatGPT 上的一个 GPT，扮演一名资深互联网软件产品经理，覆盖从需求澄清到研发交付前评审的完整产品工作流。

它不是一个只会“写 PRD”的文档生成器，而是一个以问题分析、边界收敛和开发可落地性为核心的 AI PM：

- 从想法出发，而不是直接输出方案
- 优先识别真实需求、业务目标、用户问题与风险
- 强调范围控制、MVP 拆解与研发可交付性
- 输出面向设计、开发、测试、验收都可使用的产品结果

## 核心能力

该 GPT 具备以下产品工作能力：

- 需求调研
- 业务分析
- 产品规划
- 需求分析
- 用户研究
- 用户故事地图
- MVP 规划
- 业务流程设计
- 功能架构设计
- 交互原型设计
- PRD 撰写
- 需求评审
- 研发交付支持

## 工作目标

该 GPT 的目标不是尽快“产出文档”，而是通过多阶段推进，把需求从模糊状态收敛到可执行状态，最终形成：

- 逻辑清晰
- 范围明确
- 假设透明
- 依赖可识别
- 可开发
- 可测试
- 可验收

当产品方案满足开发准备条件后，GPT 会进入 **Requirement Review / Development Readiness** 检查，并给出：

- `READY FOR DEVELOPMENT`
- `NOT READY FOR DEVELOPMENT`

## 适用场景

以下是该 GPT 的典型开场方式与适用场景：

| 开场白 | 使用场景 | 项目状态 | AI PM 应该做什么 |
| --- | --- | --- | --- |
| **① 我有一个新的产品想法，帮我从 Idea Intake 开始梳理，不要急着写 PRD。** | 从 0 到 1 有了一个新产品 Idea | 什么都还没确定 | 从 Phase 0 开始，先搞清楚 Why、目标用户、核心问题、关键假设与主要风险 |
| **② 帮我评审这个产品需求，重点找真实需求、逻辑漏洞、Scope 和过度设计问题。** | 已经有人提出需求或功能方案，想判断做不做、怎么做 | 有需求，但未必正确 | 进入 Requirement Analysis / Reviewer 模式，挑战需求本身，而不是默认需求成立 |
| **③ 这是我目前的产品资料，先判断项目处于哪个 Phase、还缺什么，再建议下一步。** | 接手一个已经进行一段时间的项目 | 中途加入 | 先读取已有资料，识别当前阶段、缺口和风险，再给出下一步推进建议 |
| **④ 这个产品准备交给研发了，请做 Requirement Review 和 Development Readiness 检查。** | 产品已经基本设计完成，准备开发 | 产品末期 | 进入交付前检查，判断 READY / NOT READY，并输出研发交接建议 |

## GPT 基本信息

**名称**：AI Product Manager GPT

**描述**：  
资深互联网软件产品经理 AI。通过需求调研、问题分析、产品定义、用户故事、MVP、功能架构、业务流程、交互设计、PRD 和需求评审，把模糊的软件产品想法逐步转化为逻辑清晰、边界明确、可开发、可测试、可验收的产品方案，并在达到 READY FOR DEVELOPMENT 后向研发阶段正式交付。

## 工作方式

该 GPT 按阶段推进，不鼓励一上来直接写方案或写 PRD，而是优先完成以下过程：

1. 明确业务目标、用户对象与问题定义
2. 拆解需求，识别伪需求、隐含假设和核心约束
3. 完成产品定义、范围控制与 MVP 规划
4. 形成用户故事、功能架构、业务流程和详细设计
5. 补齐交互说明、PRD、评审意见与研发交付材料
6. 在交付前完成 Development Readiness 检查

这意味着它既适合从零开始梳理产品，也适合中途接手需求、补齐文档、做需求评审或进行研发交付前把关。

## 知识库结构

本项目当前知识库由以下文档组成：

| 文件 | 作用 |
| --- | --- |
| `01-AI产品经理工作流.md` | 定义 AI 产品经理整体工作流与阶段推进方式 |
| `02-需求调研与需求分析.md` | 沉淀需求调研、问题分析与真实需求识别方法 |
| `03-产品定义与MVP规划.md` | 规范产品定义、范围控制与 MVP 规划方式 |
| `04-用户故事与产品功能架构.md` | 支持用户故事拆解、故事地图与功能架构设计 |
| `05-业务流程与详细功能设计.md` | 规范业务流程梳理与详细功能设计 |
| `06-交互设计与低保真原型.md` | 支持交互方案表达与低保真原型设计 |
| `07-PRD撰写规范与模板.md` | 统一 PRD 的结构、表达与模板规范 |
| `08-需求评审与研发交付.md` | 覆盖需求评审、交付物检查与研发交接 |
| `09-阶段产物与文件命名规范.md` | 统一各阶段产物与命名方式 |
| `10-Engineering-Design-Prompt.md` | 用于衔接工程设计阶段的提示词或输入规范 |
| `11-docs-engineering文档规范.md` | 规范面向工程阶段的文档结构与输出方式 |

这些知识文档共同构成该 GPT 的方法论基础，决定其输出质量、一致性与可维护性。

## 可用能力与工具

当前 GPT 支持的能力包括：

- ✅ 网页搜索
- ✅ 图片生成
- ✅ 代码解译器和数据分析

当前 **操作（Actions）**：暂未定义

## AI Product Manager GPT 整体结构

```
AI Product Manager GPT
│
├── 描述
│
├── Instructions
│   ├── Role / Mission
│   ├── Core Principles
│   ├── Workflow Controller
│   ├── Task Routing
│   ├── Phase Gate
│   ├── Artifact-aware
│   ├── Context / Decision Management
│   ├── Review / Readiness
│   └── Engineering Boundary
│
├── Knowledge
│   ├── 01～08  产品经理方法论
│   ├── 09      Artifact Governance
│   ├── 10      Engineering Design Handoff
│   └── 11      docs/engineering Contract
│
├── 对话开场白
│
└── Capabilities
    ├── Web Search
    ├── Data Analysis
    └── Image Generation（可选）
```

> Instructions = 怎么行动、哪些规则必须遵守  
> Knowledge = 做到某一步时，具体应该怎么做

## AI Product Manager GPT 的完整链路

```
                      AI Product Manager GPT
                               │
                ┌──────────────┴──────────────┐
                │                             │
          Instructions                    Knowledge
                │                             │
          Role / Workflow                01～08 方法论
          Gate / Boundary                09 Artifact
                │                        10 Handoff Prompt
                │                        11 Engineering Contract
                │
                ↓
                    Product Project
                          │
                    docs/product/
                          │
                Requirement Review
                          │
                READY FOR DEVELOPMENT
                          │
                     Phase 12
                          │
                 Development Handoff
                          │
                          ↓
                        Codex
                          │
                  Engineering Design
                          │
                docs/engineering/
                          │
                READY FOR IMPLEMENTATION
                          │
                          ↓
                    Implementation
```

## 仓库用途

该仓库用于长期维护 **AI Product Manager GPT** 的以下核心资产：

- GPT 定位与说明
- 指令与提示词迭代
- 产品方法论知识库
- 工程衔接文档
- 版本演进与维护记录

它既是一个 GPT 配置与知识资产仓库，也应逐步演变为一个可持续维护、可复用、可协作的 AI 产品经理项目模板。

## 维护原则

为保证该 GPT 长期可用，后续维护建议遵循以下原则：

- 知识库优先服务“可落地的产品交付”，避免空泛理论堆积
- 所有新增内容尽量围绕阶段推进、产物质量和研发可交付性展开
- 提示词迭代应关注稳定性、一致性与边界控制能力
- 若新增知识文档，优先保持编号化、模块化与可追踪
- 在功能增强时，优先补强评审、决策、约束识别和交付能力

## 适合谁使用

这个项目适合以下角色参考或使用：

- 独立开发者 / Solo Builder
- AI 产品经理工作流设计者
- 需要 AI 协助产出产品方案的 PM
- 希望将 Idea 系统化推进到研发阶段的创业者
- 希望沉淀产品方法论知识库的个人维护者

## 项目愿景

希望将 **AI Product Manager GPT** 持续打磨为一个真正具备产品经理思维、结构化分析能力和研发交付意识的 GPT，而不是一个只会生成表面化文档的助手。

长期目标是让它能够稳定承担从 **Idea Intake** 到 **Development Handoff** 的完整产品协作过程，成为个人或小团队的软件产品定义中枢。
