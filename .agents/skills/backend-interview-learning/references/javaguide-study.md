# JavaGuide 学习适配

仅在用户正在阅读 JavaGuide/AIGuide、提供相关链接或摘录时使用。

## 内容地图

JavaGuide 的 Java 后端主线通常包括：

1. Java 基础、集合和新特性。
2. Java 并发：线程、锁、JMM、CAS、AQS、线程池、CompletableFuture、虚拟线程。
3. JVM：内存区域、GC、类加载、调优和故障排查。
4. Spring/Spring Boot、事务、MyBatis/JPA。
5. MySQL、Redis、消息队列。
6. 网络、操作系统、Linux。
7. 分布式、微服务、高性能、高可用、系统设计和安全。

当前入口：

- JavaGuide GitHub：`https://github.com/Snailclimb/JavaGuide`
- JavaGuide 网站：`https://javaguide.cn/`
- 后端面试计划：`https://javaguide.cn/interview-preparation/backend-interview-plan.html`
- AI 应用知识体系：`https://javaguide.cn/ai/`
- AIGuide GitHub：`https://github.com/Snailclimb/AIGuide`

AIGuide 的推荐顺序是：大模型基础 → RAG → AI Agent → AI 系统设计。Agent 专题包括 Agent Loop、Memory、Prompt、Context、MCP、Skills、Harness、Workflow、Graph 和 Loop；面试还会追到失败定位、成本、稳定性、权限与评测。

## 用户最可能的提问形态

### 原文澄清

示例：“文章说 volatile 不保证原子性，具体是什么意思？”

处理：先把原句放回上下文，用最小例子解释。除非用户继续要求，不展开整个并发体系。

### 设计原因

示例：“为什么 MySQL 索引用 B+ 树？”“为什么工具描述会影响 Agent 选工具？”

处理：说明目标约束、机制、收益、代价和替代方案，避免只复述结论。

### 概念对比

示例：“synchronized 和 ReentrantLock 有什么区别？”“MCP 和 Function Calling 有什么区别？”

处理：先给共同问题，再按同一组维度比较，最后给场景化选择规则。

### 链路追踪

示例：“一条 SQL 是怎么执行的？”“Agent 从收到问题到调用工具经历什么？”

处理：按时间顺序解释状态和数据如何变化，指出关键分支、失败点和可观测信号。

### 面试表达

示例：“这题怎么回答比较完整？”

处理：提供 30 秒结论版、2～3 分钟展开版，并列出最可能的两三个追问。不要生成无法自然说出口的长文。

### 正确性检查

示例：“JavaGuide 这里是不是过时了？”“我的理解对吗？”

处理：区分核心思想和特定版本实现；检查当前官方文档或源码，不凭记忆裁决。

### 看完后的抽查

示例：“根据这一节考我。”“继续追问。”

处理：从定义题逐步过渡到机制、边界和场景题，一次一题。

## 使用来源的规则

- 用户给出页面链接时，先阅读对应页面的相关段落，不假设文章内容。
- JavaGuide/AIGuide 用于确定知识脉络、常见题和中文解释。
- JDK、Spring、MySQL、Redis、MCP 或框架行为以当前官方文档、规范和源码为最终依据。
- 对具有版本差异的内容明确写出版本，例如 JDK 8 与当前 LTS 中 AQS 内部实现的差异。
- 不整篇复制文章。围绕用户问题重组解释并链接来源。

## 深入学习的最小闭环

当用户明确要求深入学习某一节时：

1. 用一个问题快速判断现有理解。
2. 给出该节在整个专题中的位置。
3. 解释核心因果链或执行链路。
4. 处理一个易错点或反例。
5. 让用户闭卷解释、预测结果或回答一道场景题。
6. 根据回答决定继续、补前置知识或结束。
