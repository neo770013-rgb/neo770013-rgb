# Web3 系统工程笔记

围绕公开演示项目涉及的数据接入、执行状态、可观测性和部署交付，整理设计原则、故障场景与验证方法。这里提供的是设计检查表，不声明公开仓库已实现相应生产能力。

整理说明：本组笔记于 2026-11-03 集中编写；提交作者日期沿用原有贡献日安排，提交者时间记录本次整理时间。这些日期不代表当时实际完成了开发。

阅读方式：每篇包含设计约束、三步落地检查、典型失效模式、验证场景和审阅问题。涉及产品规则时，应以目标接口当前官方协议为准。验证应使用固定样本或隔离测试环境。

## 目录

- [交易所适配器边界](api-boundary.md)
- [交易对与资产命名](symbol-map.md)
- [金额与数量精度](decimal-money.md)
- [数量步长校验](quantity-step.md)
- [价格刻度校验](price-tick.md)
- [名义金额与过滤器](notional-check.md)
- [事件时间与接收时间](time-model.md)
- [时钟偏移与请求窗口](clock-offset.md)
- [HTTP 超时预算](http-timeouts.md)
- [读取请求重试](read-retries.md)
- [请求限额预算](rate-budget.md)
- [错误分类与传播](error-model.md)
- [HMAC 请求载荷](hmac-payload.md)
- [凭证权限与生命周期](credential-scope.md)
- [日志脱敏](log-redaction.md)
- [WebSocket 连接生命周期](ws-lifecycle.md)
- [WebSocket 重连退避](ws-backoff.md)
- [快照与增量衔接](snapshot-delta.md)
- [数据新鲜度](stale-data.md)
- [盘口深度与执行估计](book-depth.md)
- [客户端订单标识](client-order-id.md)
- [订单状态机](order-states.md)
- [下单结果未知](ambiguous-submit.md)
- [部分成交记录](partial-fills.md)
- [撤单与成交竞态](cancel-race.md)
- [双腿执行编排](two-leg-flow.md)
- [净敞口表达](exposure-model.md)
- [执行前约束检查](limits-gate.md)
- [暂停开关语义](pause-switch.md)
- [本地与远端对账](state-reconcile.md)
- [SQLite 事务边界](sqlite-transaction.md)
- [数据结构迁移](schema-change.md)
- [去重键与唯一约束](unique-keys.md)
- [状态变更事件记录](event-history.md)
- [进程重启恢复](startup-recovery.md)
- [异步任务取消](async-cancel.md)
- [工作队列背压](worker-queue.md)
- [请求关联与链路](trace-context.md)
- [运行指标](health-metrics.md)
- [前后端 API 契约](api-contract.md)
- [分页与稳定排序](pagination-order.md)
- [界面异步状态](ui-async-states.md)
