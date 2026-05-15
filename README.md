<h1 align="center">Hi there, I'm 林宇祥 👋</h1>

<p align="center">
  Java 后端方向学习者 / 专注分布式系统、工程实践与面试沉淀
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Java_Backend-000000?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring_Cloud-000000?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/MySQL-000000?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-000000?style=for-the-badge&logoColor=white" />
</p>

---

## About Me

- 🎓 **华南师范大学**｜计算机学院 · 网络工程本科（2024 - 2028）
- 🎯 **目标方向**：Java 后端开发实习
- 📚 **当前重点**：MySQL、Redis、JVM、Spring Cloud、SQL 场景题、项目表达
- 🧠 **学习风格**：偏工程实践 + 高频母题 + 面试表达
- 📫 **Contact**：2865598015@qq.com

---

## Tech Stack

### 核心语言与基础
<p>
  <img src="https://img.shields.io/badge/Java-111111?style=for-the-badge" />
  <img src="https://img.shields.io/badge/JUC-111111?style=for-the-badge" />
  <img src="https://img.shields.io/badge/JVM-111111?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Design_Patterns-111111?style=for-the-badge" />
</p>

### 框架与微服务
<p>
  <img src="https://img.shields.io/badge/Spring-111111?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Spring_Boot-111111?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Spring_Cloud-111111?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Gateway-111111?style=for-the-badge" />
</p>

### 数据库与缓存
<p>
  <img src="https://img.shields.io/badge/MySQL-111111?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Redis-111111?style=for-the-badge" />
  <img src="https://img.shields.io/badge/SQL-111111?style=for-the-badge" />
</p>

### 中间件与工具
<p>
  <img src="https://img.shields.io/badge/RocketMQ-111111?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Nacos-111111?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Docker-111111?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Maven-111111?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Git-111111?style=for-the-badge" />
</p>

---

## Featured Project

### 12306 铁路购票系统｜本地部署与压测验证

基于开源 12306 铁路购票项目，完成了一轮从 **本地部署、核心链路验证到接口压测** 的工程实践，重点围绕 **库存安全、购票链路、幂等控制、异常排查** 展开。

#### 我做了什么
- 使用 Docker 拉起 **MySQL、Redis、Nacos、RocketMQ**
- 启动 **SpringBoot 聚合服务 + Gateway**
- 跑通 **登录、车票查询、乘车人新增、购票下单、订单落库、取消订单** 等核心链路
- 对查询接口进行本地压测，并验证购票接口的幂等控制能力
- 排查并解决服务调用中的真实问题，如：
  - **Nacos 注册 IP 不可达**
  - **乘车人手工造数与加密字段不兼容**
  - **订单状态与链路对账口径问题**

#### 第一版压测结果
| 场景 | 指标 |
|---|---|
| 车票查询接口 | 30 并发 / 300 请求 / 100% 成功 |
| 查询性能 | QPS ≈ **1103** / Avg RT ≈ **26.42 ms** / P95 ≈ **42.58 ms** / P99 ≈ **47.33 ms** |
| 购票幂等验证 | 同一用户 10 并发重复提交，**1 次成功下单，9 次被幂等拦截** |

#### 项目价值
- 更真实地理解了微服务项目的 **启动依赖顺序、服务注册发现、缓存与数据库协作**
- 对高频面试问题里的 **Redis、Lua、幂等、防重复下单、异常一致性** 有了更强的工程感
- 不只是“看过项目”，而是做了 **可验证、可复述、可继续迭代** 的本地实践

🔗 项目仓库：`12306-pressure-test-lab`  
🔗 压测记录：`docs/pressure-test/README.md`

---

## Current Focus

- **MySQL**：索引、锁、事务、MVCC、SQL 调优
- **Redis**：缓存、高并发、Lua、分布式锁
- **JVM**：内存结构、垃圾回收、类加载
- **Project**：12306 库存安全、异常一致性、压测与复盘
- **Interview**：项目表达、八股体系化、SQL 场景题

---

## GitHub Stats

<p>
  <img height="160" src="https://github-readme-stats.vercel.app/api?username=Oliver1205&show_icons=true&hide_border=true&title_color=000000&text_color=222222&icon_color=000000&bg_color=ffffff" />
  <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Oliver1205&layout=compact&hide_border=true&title_color=000000&text_color=222222&bg_color=ffffff" />
</p>

---

## Motto

> 持续把“会做”沉淀成“会讲”，把“会讲”落实成“能落地”。
