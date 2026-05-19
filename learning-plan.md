# Learning Plan / 学习计划

> 基于 AI/Web3 新手，每日 1-2 小时，中文输出为主
> Adapted from: AI × Web3 School Handbook

---

## 概览 / Overview

本计划基于 Handbook 四层地图设计：

| 阶段 | 内容 | 周数 |
|------|------|------|
| Phase 1 | AI 基础 | Weeks 1-4 |
| Phase 2 | Web3 基础 | Weeks 5-8 |
| Phase 3 | AI × Web3 Bridge | Weeks 9-10 |
| Phase 4 | 前沿探索 & 原型 | Weeks 11-12 |

---

## Phase 1: AI 基础（Weeks 1-4）

### Week 1 — LLM & Prompt / 大语言模型与提示词

**必读章节：**
- [ ] [LLM](https://aiweb3.school/zh/handbook/ai/llm/)：大模型能做什么，不能替代什么
- [ ] [Prompt](https://aiweb3.school/zh/handbook/ai/prompt/)：如何把任务目标、边界和输出格式写清楚

**练习：**
- [ ] 写 3 个不同场景的 prompt（任务目标 + 边界 + 输出格式）
- [ ] 对比不同 prompt 策略的效果差异

**产出：**
- 将练习的 prompt 记录到 `experiments/` 目录

---

### Week 2 — Context & RAG / 上下文与检索增强生成

**必读章节：**
- [ ] [Context](https://aiweb3.school/zh/handbook/ai/context/)：模型一次能看见什么，哪些信息可信，哪些会过期
- [ ] [RAG](https://aiweb3.school/zh/handbook/ai/rag/)：如何把外部知识、来源和引用接入模型

**练习：**
- [ ] 搭建一个简单的本地 RAG pipeline（可用 LangChain 或直接用向量数据库）
- [ ] 理解 context window 和信息可信度的区别

**产出：**
- 将 RAG 实验记录到 `experiments/` 目录

---

### Week 3 — Agent & Tool Use / 智能体与工具调用

**必读章节：**
- [ ] [Agent](https://aiweb3.school/zh/handbook/ai/agent/)：如何让模型进入工具调用和多步执行
- [ ] [Frameworks](https://aiweb3.school/zh/handbook/ai/frameworks/)：LangChain、LangGraph、Agents SDK 各解决哪一层问题

**练习：**
- [ ] 运行一个简单的 Agent loop（带工具调用）
- [ ] 理解 ReAct、Plan-and-Execute 等不同 Agent 模式的区别

---

### Week 4 — MCP & Evaluation & More / 模型上下文协议与评估

**必读章节：**
- [ ] [MCP](https://aiweb3.school/zh/handbook/ai/mcp/)：模型、工具和上下文如何通过协议连接
- [ ] [Evaluation](https://aiweb3.school/zh/handbook/ai/evaluation/)：如何测试、回放和持续改进 Agent 输出
- [ ] [Vibe Coding](https://aiweb3.school/zh/handbook/ai/vibe-coding/)（选读）：氛围编程的概念

**练习：**
- [ ] 理解 MCP 的核心概念（Host、Tools、Resources）
- [ ] 搭建一个简单的 Evaluation 流程（输入 → 输出 → 评分）

**产出：**
- [ ] 构建个人 AI 概念地图（可放在 `tasks/` 或直接放 README）

---

## Phase 2: Web3 基础（Weeks 5-8）

### Week 5 — Network & Cryptography & Wallet / 网络、密码学与钱包

**必读章节：**
- [ ] [Network](https://aiweb3.school/zh/handbook/web3/network/)：区块、共识、L2、RPC 和链上状态的基本环境
- [ ] [Cryptography](https://aiweb3.school/zh/handbook/web3/cryptography/)：哈希、公私钥、签名概念
- [ ] [Wallet](https://aiweb3.school/zh/handbook/web3/wallet/)：钱包作为身份和签名入口

**练习：**
- [ ] 设置 MetaMask 钱包，理解助记词安全
- [ ] 用钱包连接一个测试网 DApp

---

### Week 6 — Smart Contract & Dev Stack / 智能合约与开发栈

**必读章节：**
- [ ] [Smart Contract](https://aiweb3.school/zh/handbook/web3/smart-contract/)：链上规则如何部署、调用和更新状态
- [ ] [Dev Stack](https://aiweb3.school/zh/handbook/web3/dev-stack/)：开发栈总览

**练习：**
- [ ] 读懂一个简单的 Solidity 合约（如 ERC-20 或 Storage 合约）
- [ ] 了解 Hardhat/Foundry + ethers.js 的基本使用

---

### Week 7 — Account Abstraction & DeFi & Oracle / 账户抽象与 DeFi

**必读章节：**
- [ ] [Account Abstraction](https://aiweb3.school/zh/handbook/web3/account-abstraction/)：为什么 Smart Account 更适合表达 Agent 权限模型
- [ ] [DeFi](https://aiweb3.school/zh/handbook/web3/defi/)：开放金融协议里的资产、流动性、借贷和风险传播
- [ ] [Oracle](https://aiweb3.school/zh/handbook/web3/oracle/)：链外数据如何进入链上系统

**练习：**
- [ ] 理解 EOA vs Smart Account 的区别
- [ ] 在测试网体验一次 swap（如 Uniswap fork）

---

### Week 8 — Indexing & Security / 索引与安全

**必读章节：**
- [ ] [Indexing](https://aiweb3.school/zh/handbook/web3/indexing/)：把链上事件、交易和状态整理成 AI 与产品可用的数据层
- [ ] [Security](https://aiweb3.school/zh/handbook/web3/security/)：合约、权限、模拟和监控里的风险边界

**练习：**
- [ ] 用 The Graph 或 Dune 体验一次链上数据查询
- [ ] 理解权限最小化原则和模拟验证的重要性

**产出：**
- [ ] 画一张 Web3 概念关系图

---

## Phase 3: AI × Web3 Bridge（Weeks 9-10）

### Week 9 — Chain Context & Web3 Tool Use / 链上上下文与工具调用

**必读章节：**
- [ ] [Chain-aware Context](https://aiweb3.school/zh/handbook/bridge/chain-aware-context/)：链上状态如何进入 Agent 上下文
- [ ] [Web3 Tool Use](https://aiweb3.school/zh/handbook/bridge/web3-tool-use/)：RPC、钱包、合约工具如何被 Agent 调用
- [ ] [Agent Workflow](https://aiweb3.school/zh/handbook/bridge/agent-workflow/)：哪些步骤适合自动化，哪些必须 human-in-the-loop

**练习：**
- [ ] 让 Agent 读取链上状态（通过 RPC 或索引服务）
- [ ] 实现一个 Web3 工具调用 demo

---

### Week 10 — Agent Wallet & Machine Payment / 智能体钱包与机器支付

**必读章节：**
- [ ] [Agent Wallet](https://aiweb3.school/zh/handbook/bridge/agent-wallet/)：Agent 能拿什么权限，如何限制和撤销
- [ ] [Machine Payment](https://aiweb3.school/zh/handbook/bridge/machine-payment/)：机器之间如何完成小额支付
- [ ] [Agent Identity](https://aiweb3.school/zh/handbook/bridge/agent-identity/)：Agent 如何被识别、授权和追踪

**选读：**
- [ ] [Settlement & Escrow](https://aiweb3.school/zh/handbook/bridge/settlement-and-escrow/)
- [ ] [Agent Trust & Reputation](https://aiweb3.school/zh/handbook/bridge/agent-trust-and-reputation/)

---

## Phase 4: 前沿探索 & 原型开发（Weeks 11-12）

### Week 11 — Prototype Development / 原型开发

**选择一条赛道：**
- [ ] [Agentic Commerce](https://aiweb3.school/zh/handbook/tracks/agentic-commerce/)：Agent 如何发现服务、协商任务、完成支付
- [ ] [Wallet / Permission](https://aiweb3.school/zh/handbook/tracks/wallet-permission/)：钱包、权限、Session Key、Policy 原型
- [ ] [AI Security](https://aiweb3.school/zh/handbook/tracks/ai-security/)：攻击面、权限隔离、审计和告警
- [ ] [Governance](https://aiweb3.school/zh/handbook/tracks/governance/)：面向 DAO 和协议治理的 AI 协作
- [ ] [Dev Tooling](https://aiweb3.school/zh/handbook/tracks/dev-tooling/)：合约理解、测试、代码审查工具

**任务：**
- [ ] 搭建一个最小可行原型（MVP）
- [ ] 记录架构和关键决策

---

### Week 12 — Hackathon Prep / 黑客松准备

**任务：**
- [ ] 完善原型，准备演示
- [ ] 撰写项目文档（README + Architecture）
- [ ] 提交黑客松 / 公开分享

---

## 每日学习流程 / Daily Routine

1. **早上（09:00）**：收到提醒 → 查看今日任务 → 阅读 Handbook 章节
2. **学习与实践**：按周计划推进，完成练习和产出
3. **晚间（21:00）**：收到打卡提醒 → 写打卡内容 → 手动提交 WCB
4. **Git 记录**：每日学习后更新 `daily/YYYY-MM-DD.md`，并 push 到 GitHub

---

## 目录结构说明 / Repo Structure

```
ai-web3-school-cohort-0/
├── README.md              # 本文件
├── profile.md             # 个人学习档案
├── learning-plan.md       # 本学习计划
├── daily/                 # 每日学习笔记 (YYYY-MM-DD.md)
│   └── 2026-05-19.md     # 示例
├── tasks/                 # 任务笔记和进度
├── experiments/           # 实践实验和 demo
├── handbook-feedback/     # Handbook 反馈（问题、建议）
│   └── 2026-05-17-initial-setup.md  # 示例
├── hackathon/             # 黑客松项目
├── submissions/           # 提交记录和链接
└── templates/             # 笔记模板
    ├── daily-note.md
    └── task-note.md
```

---

*Last updated: 2026-05-19*
