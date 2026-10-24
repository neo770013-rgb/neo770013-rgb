# Web3 开发实践｜从 0 到 1 的系统开发与部署

专注 **Web3 / 数字资产交易系统开发**，围绕现货、永续合约与资金费率套利场景，积累交易所 API 接入、策略执行、仓位监控与风险控制的工程实践。

具备 **从需求拆解、方案设计、前后端开发、接口联调、测试验证到部署上线的完整交付能力**，能够独立推进项目落地，将业务想法转化为可运行、可体验、可维护的系统。

代表项目 **Papaya 资金费率套利系统**：基于开源基础持续迭代，完成交易接口接入、策略与状态管理、监控界面及部署交付，并提供公开脱敏演示与源码，便于直接体验和技术审阅。

**[体验 Papaya 在线演示 ↗](https://papaya-arbitrage-portfolio.alylwxy.chatgpt.site/) · [查看公开源码 ↗](https://github.com/neo770013-rgb/Papaya-Portfolio)**

## 核心能力 · Web3 交易场景 × 从 0 到 1 交付

- **数字资产交易业务实践：**围绕中心化交易所（CEX）的现货与永续合约场景，实现资金费率扫描、成本评估、候选池筛选与仓位监控，将策略判断落实为业务功能。
- **交易所接入与执行工程：**对接行情和交易接口，处理 HMAC 请求签名、双腿订单执行、订单终态确认、状态持久化与异常恢复，关注执行过程的可观察性与风险边界。
- **独立推进完整交付：**覆盖需求拆解、方案设计、前后端开发、接口联调、测试验证和部署交付；基于开源基础完成迭代，并独立上线公开演示，让项目可以被访问、体验和审阅。

**交付路径：**业务需求 → 策略与数据建模 → 前后端开发 → 交易所接入 → 测试与安全加固 → 部署与运行监控。

## 代表项目 · Papaya

### [在线体验 ↗](https://papaya-arbitrage-portfolio.alylwxy.chatgpt.site/) · [查看公开源码 ↗](https://github.com/neo770013-rgb/Papaya-Portfolio) · [阅读项目说明 ↗](https://papaya-arbitrage-portfolio.alylwxy.chatgpt.site/#/project)

[![Papaya 资金费率套利系统：点击进入在线演示](https://raw.githubusercontent.com/neo770013-rgb/Papaya-Portfolio/main/docs/images/overview.jpg)](https://papaya-arbitrage-portfolio.alylwxy.chatgpt.site/)

**项目目标：**在[开源套利项目](https://github.com/yansc153/fundingRate_Arb_Tool)基础上持续开发，通过现货与永续合约双腿对冲，将机会扫描、成本评估、策略执行、仓位监控及交易记录组织为完整业务流程。

| 方向 | 项目中的实践 |
| --- | --- |
| 业务到产品 | 将资金费率套利拆分为扫描、筛选、执行、监控和收益归因，形成可交互的业务流程 |
| 全栈开发 | 使用 React / TypeScript 构建交互界面，结合 Python / FastAPI 实现后端服务 |
| 交易所接入 | 行情与交易接口对接、HMAC 请求签名、双腿执行和订单终态确认 |
| 策略与状态管理 | 结合手续费、滑点、基差筛选候选，实现仓位约束、轮换逻辑及状态持久化与异常恢复 |
| 部署与交付 | 完成系统部署与账户接口认证，将公开展示与账户操作分离，交付可访问的演示网站、源码与中文文档 |

**建议用 1 分钟体验：**

1. [费率扫描](https://papaya-arbitrage-portfolio.alylwxy.chatgpt.site/#/scanner)：搜索交易对，筛选候选与已过滤标的，查看决策原因。
2. [项目首页](https://papaya-arbitrage-portfolio.alylwxy.chatgpt.site/)：切换收益窗口和策略场景，观察成本对净收益的影响。
3. [交易样本](https://papaya-arbitrage-portfolio.alylwxy.chatgpt.site/#/trade-history)：查看状态筛选、仓位信息及收益归因。

> 正式系统保留在私有仓库；公开仓库仅包含独立的演示前端。网站行情、交易样本及收益均为合成数据，不连接真实账户、不执行真实交易，也不代表实盘或回测业绩。

## 技术与代码阅读

**后端与接入：**Python · FastAPI · SQLite · HTTP / WebSocket  
**前端与交付：**React · TypeScript · Vite · Tailwind CSS · 静态网站部署

如果希望进一步了解实现，可以从以下代码开始：

- [合成数据与收益计算](https://github.com/neo770013-rgb/Papaya-Portfolio/blob/main/src/lib/demo.ts)：查看统一交易账本与指标口径。
- [收益展示组件](https://github.com/neo770013-rgb/Papaya-Portfolio/blob/main/src/components/PerformancePanel.tsx)：查看曲线交互与多周期指标展示。
- [费率扫描页面](https://github.com/neo770013-rgb/Papaya-Portfolio/blob/main/src/pages/Scanner.tsx)：查看搜索、排序及候选池筛选。
- [回归测试](https://github.com/neo770013-rgb/Papaya-Portfolio/tree/main/tests)：查看演示边界与数据一致性检查。

项目问题与技术交流欢迎通过 [Papaya Issues](https://github.com/neo770013-rgb/Papaya-Portfolio/issues) 留言。
