<h1 align="center">林宇祥 / Oliver</h1>

<p align="center">
  211 · 双一流 · 网络工程本科生
</p>

<p align="center">
  <a href="mailto:2865598015@qq.com">Email</a>
  ·
  <a href="https://github.com/Oliver1205/12306-pressure-test-lab">12306 Pressure Test Lab</a>
</p>

---

## About

计算机学院网络工程本科生，来自 211、双一流高校。

关注 Java 后端工程、数据库、缓存、中间件与高并发业务场景，重视从业务链路出发理解系统设计：  
不仅看接口是否能跑通，也关注数据是否正确落库、状态是否闭环、异常是否可定位、结果是否可复盘。

目前主要沉淀方向包括：

| Area | Focus |
|---|---|
| Java Backend | Java、Spring Boot、Spring Cloud、Gateway |
| Database | MySQL 索引、事务、锁、MVCC、SQL 优化 |
| Cache | Redis、缓存一致性、分布式锁、Lua |
| Middleware | RocketMQ、Nacos、Docker |
| Engineering | 接口压测、链路验证、异常排查、数据对账 |
| Interview | 项目表达、技术复盘、场景化问题拆解 |

---

## Stack

<p>
  <img src="https://img.shields.io/badge/Java-111111?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring_Boot-111111?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring_Cloud-111111?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/MySQL-111111?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-111111?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/RocketMQ-111111?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Nacos-111111?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-111111?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/JMeter-111111?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Git-111111?style=flat-square&logoColor=white" />
</p>

| Category | Technologies |
|---|---|
| Language | Java |
| Framework | Spring Boot、Spring Cloud、Gateway |
| Database | MySQL、索引优化、事务、锁、MVCC |
| Cache | Redis、Lua、分布式锁、缓存一致性 |
| Middleware | RocketMQ、Nacos |
| Tooling | Docker、Git、Maven、JMeter |
| Engineering | 压测验证、链路排障、数据状态对账 |

---

## Project

### 12306 Pressure Test Lab

基于开源 12306 铁路购票项目，完成本地部署、核心链路验证、JMeter 压测、订单状态对账与工程问题排查。

Repository:  
[github.com/Oliver1205/12306-pressure-test-lab](https://github.com/Oliver1205/12306-pressure-test-lab)

### Highlights

| Module | Result |
|---|---|
| 本地部署 | SpringBoot 聚合版启动成功 |
| 中间件 | MySQL、Redis、Nacos、RocketMQ、Docker |
| 核心链路 | 登录、查询车票、乘车人、购票、订单落库、取消订单 |
| 查询接口压测 | 50 / 100 / 200 并发均 0 错误 |
| 查询接口峰值 | 200 并发 / 5000 请求，QPS ≈ 1000 req/s，P95 ≈ 5ms |
| 单用户购票 | 单用户单次购票成功，订单正常生成 |
| 幂等验证 | 单用户 5 并发重复购票，仅 1 个请求成功，其余被流程锁拦截 |
| 多用户购票 | 5 / 10 / 20 用户并发购票压测通过 |
| 20 用户压测 | HTTP 20/20 成功，Avg 250.75ms，P95/P99 274ms |
| 订单状态闭环 | 订单主表与订单明细均完成 `status = 0` 到 `status = 30` 流转 |
| 分库分表排障 | 定位并修复取消订单缺少 `user_id` 导致的分片路由不一致问题 |
| Redis Lua 排障 | 定位并修复 ticket-service 取消链路令牌桶回滚 nil 比较异常 |

### Engineering Value

这个项目重点不只是保存 JMeter 报告，而是围绕完整业务链路进行验证：

- 从 HTTP success 进一步追踪到数据库订单主表、订单明细表状态；
- 从单接口压测扩展到购票、取消、状态闭环验证；
- 从表面错误码继续定位到分库分表路由、Redis Lua 脚本和后置资源回滚；
- 将压测数据、问题定位、修复方案和截图证据沉淀到 README 和文档中。

---

## Project Snapshot

| Scenario | Result |
|---|---|
| Q-001 查询接口压测 | 50 并发 / 1000 请求 / 成功率 100% |
| Q-002 查询接口压测 | 100 并发 / 3000 请求 / 成功率 100% |
| Q-003 查询接口压测 | 200 并发 / 5000 请求 / QPS ≈ 1000 req/s |
| P-001 单用户购票 | 单次购票成功，订单生成 |
| P-002 幂等验证 | 5 并发重复提交，仅 1 个成功 |
| P-003 5 用户购票 | 5/5 购票成功，取消后状态闭环 |
| P-004 10 用户购票 | 10/10 HTTP 成功，Avg 350ms |
| P-005 20 用户购票 | 20/20 HTTP 成功，Avg 250.75ms |
| P-006 异常修复 | Redis Lua 令牌桶回滚异常修复，取消链路回归通过 |

---

## GitHub

<p align="center">
  <img height="160" src="https://github-readme-stats.vercel.app/api?username=Oliver1205&show_icons=true&hide_border=true&title_color=111111&text_color=222222&icon_color=111111&bg_color=ffffff" />
  <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Oliver1205&layout=compact&hide_border=true&title_color=111111&text_color=222222&bg_color=ffffff" />
</p>

---

<p align="center">
  把项目做实，把问题查清，把技术讲透。
</p>
