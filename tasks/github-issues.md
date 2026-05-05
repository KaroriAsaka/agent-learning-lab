# GitHub Issue Seeds

这些 issue 等仓库推到 GitHub 后创建。

## Issue 1: Stage 1 - 搭建 Python 项目骨架

Labels: `learning`, `stage-1`, `setup`

### Goal

初始化一个适合 Agent 学习项目的 Python 工程。

### Scope

- [ ] 选择 Python 版本
- [ ] 配置包管理工具
- [ ] 配置 `.env.example`
- [ ] 配置测试目录
- [ ] 配置 README 的运行说明

### Acceptance Criteria

- [ ] 能本地安装依赖
- [ ] 能运行测试命令
- [ ] 不提交真实 API key

## Issue 2: Stage 1 - 封装 LLM Client

Labels: `learning`, `stage-1`, `llm`

### Goal

实现统一的模型调用入口，避免业务代码直接依赖厂商 SDK。

### Scope

- [ ] 创建 `LLMClient`
- [ ] 支持 model、temperature、timeout
- [ ] 支持 retry
- [ ] 统一错误类型
- [ ] 记录 token 和 latency

### Acceptance Criteria

- [ ] 成功调用模型
- [ ] 失败时返回统一错误
- [ ] 日志中包含 request_id、model、latency

## Issue 3: Stage 1 - 实现 LLM Gateway

Labels: `project`, `stage-1`, `backend`

### Goal

实现一个最小 LLM 网关服务。

### Scope

- [ ] `POST /chat`
- [ ] `POST /summarize`
- [ ] `POST /extract`
- [ ] request_id
- [ ] 统一错误格式

### Acceptance Criteria

- [ ] 三个接口可以本地调用
- [ ] 错误格式稳定
- [ ] README 写清楚运行方式

## Issue 4: Stage 1 - 结构化输出练习

Labels: `learning`, `stage-1`, `structured-output`

### Goal

练习让模型稳定返回 JSON，并用 schema 校验。

### Scope

- [ ] 摘要 schema
- [ ] 分类 schema
- [ ] action item schema
- [ ] JSON parse error 处理
- [ ] schema validation error 处理

### Acceptance Criteria

- [ ] 至少 3 个 schema
- [ ] 至少 5 条测试样例
- [ ] 错误输出可被识别

## Issue 5: Stage 1 - Markdown 笔记结构化摘要脚本

Labels: `project`, `stage-1`, `obsidian`

### Goal

读取 Obsidian Markdown 笔记，生成结构化摘要。

### Scope

- [ ] 扫描 Markdown 文件
- [ ] 跳过 `.obsidian/`
- [ ] 跳过空文件
- [ ] 生成 JSON 摘要
- [ ] 保存到 `.summaries/`

### Acceptance Criteria

- [ ] 能处理当前 Obsidian Vault
- [ ] 每篇摘要包含 title、summary、key_points、tags
- [ ] 单个文件失败不影响整体批处理

## Issue 6: Stage 1 - 日志与成本统计

Labels: `learning`, `stage-1`, `observability`

### Goal

给模型调用增加最小可观测性。

### Scope

- [ ] request_id
- [ ] model
- [ ] input_tokens
- [ ] output_tokens
- [ ] latency_ms
- [ ] error_type

### Acceptance Criteria

- [ ] 每次模型调用都有日志
- [ ] 日志不包含 API key
- [ ] 日志不包含未脱敏敏感数据

## Issue 7: Stage 1 - 阶段复盘

Labels: `learning`, `stage-1`, `retrospective`

### Goal

复盘第一阶段学到的东西和踩过的坑。

### Scope

- [ ] 学到的概念
- [ ] 实现时踩坑
- [ ] 代码设计取舍
- [ ] 下一阶段问题清单

### Acceptance Criteria

- [ ] `docs/stage-1-retrospective.md` 存在
- [ ] 至少 5 条具体复盘

