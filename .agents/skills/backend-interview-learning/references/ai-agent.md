# AI Agent 八股范围

仅在问题涉及 AI Agent、LLM 应用、RAG、MCP、Skills、工作流或 AI 系统设计时读取。

## 主知识链

按下面的依赖关系组织解释，不围绕单一框架背 API：

1. **一次模型调用**：Token、上下文、消息、采样、流式输出、结构化输出。
2. **外部知识**：Embedding、Chunk、检索、Rerank、引用与 RAG 评测。
3. **外部动作**：Function/Tool Calling、Schema、执行权、结果回传和错误处理。
4. **Agent Loop**：读取状态、决定动作、调用工具、观察结果、继续/结束/交给人工。
5. **状态与记忆**：会话历史、工作状态、Checkpoint、短期与长期 Memory。
6. **编排方式**：Workflow、Graph、Loop、ReAct、Plan-and-Execute、Reflection、多 Agent。
7. **能力交付**：MCP、Agent Skills、工具注册、权限与能力发现。
8. **工程外壳**：Context/Harness Engineering、评测、Trace、安全、成本、限流、降级和恢复。

## 高频追问方向

- 它解决什么问题？普通模型调用或固定 Workflow 为什么不够？
- 完整请求链路是什么？状态在哪里保存？
- 模型负责决策，应用负责什么？
- 失败可能发生在哪一层？如何观察和复现？
- 为什么选择当前方案？替代方案和代价是什么？
- 怎样限制工具权限、避免提示注入和危险写操作？
- 如何证明 Prompt、检索、模型或工具修改真的改善了效果？
- 如何控制 Token、延迟、并发和供应商故障？

## 必须分清的概念

- Chatbot、Workflow、Agent、Agentic Workflow。
- RAG、长上下文、搜索和微调。
- Chat History、当前任务状态、短期 Memory、长期 Memory。
- Function Calling、工具执行、MCP。
- Prompt、Context、Skill、Tool。
- 单 Agent、多 Agent、Supervisor、Router 和 Handoff。
- 离线评测、在线指标、Trace 与业务结果。

## 时效性

AI Agent 术语和框架变化快。回答框架能力、协议字段、模型限制或 API 行为时必须查当前官方资料。将稳定原理与某一版本实现分开表达，并标注核对日期或版本。

JavaGuide/AIGuide 可作为中文知识入口；协议和框架事实优先使用对应官方规范与文档。
