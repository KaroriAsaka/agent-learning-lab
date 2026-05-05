# Agent Learning Lab

这是一个用于系统学习 Agent 开发的个人练习仓库。

目标不是收藏一堆 demo，而是把每个阶段的学习任务都落实成可运行、可测试、可复盘的小项目。

## 学习主线

1. LLM API 工程化
2. 结构化输出
3. Tool Calling
4. RAG 与知识库工程
5. Agent 状态管理
6. MCP 与外部工具
7. Evals、Tracing 与生产化

## 当前阶段

当前聚焦：`Stage 1 - LLM 应用基础`

阶段目标：

- 封装稳定的 LLM client
- 处理 timeout、retry、rate limit
- 让模型稳定返回结构化 JSON
- 设计并执行简单工具调用
- 做出两个可运行练习项目

## 目录结构

```text
.
├── docs/                         # 学习笔记与设计记录
├── tasks/                        # 阶段任务清单
├── projects/                     # 每阶段练习项目
│   ├── llm-gateway/              # 练习 1：LLM 网关服务
│   └── obsidian-note-summarizer/ # 练习 2：Markdown 笔记结构化摘要
├── src/                          # 可复用代码
├── tests/                        # 测试
└── .github/ISSUE_TEMPLATE/       # GitHub issue 模板
```

## 推荐工作方式

- 每个任务开一个 issue
- 每个练习项目开一个分支
- 每次完成一个小目标就提交一次
- README 记录最终使用方式
- `docs/` 记录踩坑和设计取舍

## 第一批推荐 issues

这些任务可以在 GitHub 上创建为 issues：

- Stage 1: 搭建 Python 项目骨架
- Stage 1: 封装 LLM client
- Stage 1: 实现 `/chat` 接口
- Stage 1: 实现结构化摘要 schema
- Stage 1: 实现 Markdown 笔记摘要脚本
- Stage 1: 给模型调用加日志和成本统计
- Stage 1: 写第一份复盘笔记

## 参考项目

- OpenAI Agents SDK: https://github.com/openai/openai-agents-python
- Pydantic AI: https://github.com/pydantic/pydantic-ai
- LangGraph: https://github.com/langchain-ai/langgraph
- LlamaIndex: https://github.com/run-llama/llama_index
- MCP Python SDK: https://github.com/modelcontextprotocol/python-sdk

