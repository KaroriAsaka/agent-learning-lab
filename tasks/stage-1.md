# Stage 1 Tasks

## 任务 1：搭建项目骨架

- [ ] 选择 Python 版本
- [ ] 初始化包管理工具
- [ ] 配置 `.env.example`
- [ ] 配置测试命令
- [ ] 写最小 README

验收标准：

- 能本地安装依赖
- 能运行测试命令
- 不提交真实 API key

## 任务 2：封装 LLM Client

- [ ] 创建统一 `LLMClient`
- [ ] 支持 model、temperature、timeout
- [ ] 支持 retry
- [ ] 返回统一响应对象
- [ ] 记录 token 和 latency

验收标准：

- 业务代码不直接调用厂商 SDK
- 调用失败时能返回统一错误

## 任务 3：实现 LLM Gateway

- [ ] 实现 `/chat`
- [ ] 实现 `/summarize`
- [ ] 实现 `/extract`
- [ ] 增加 request_id
- [ ] 增加错误格式

验收标准：

- 三个接口能本地调用
- 输出结构清晰
- 错误格式统一

## 任务 4：结构化输出练习

- [ ] 定义摘要 schema
- [ ] 定义分类 schema
- [ ] 定义 action item schema
- [ ] 校验模型输出
- [ ] 处理 JSON parse 失败

验收标准：

- 至少 3 个 schema
- 至少 5 条样例输入
- 失败样例可被识别

## 任务 5：Markdown 笔记摘要脚本

- [ ] 扫描 Markdown 文件
- [ ] 跳过 `.obsidian/`
- [ ] 读取正文
- [ ] 调用模型生成摘要
- [ ] 保存 JSON 结果

验收标准：

- 能处理当前 Obsidian Vault
- 每篇摘要包含 title、summary、key_points、tags
- 空文件不会中断任务

## 任务 6：阶段复盘

- [ ] 写清楚学到了什么
- [ ] 记录踩坑
- [ ] 记录下一阶段要补什么
- [ ] 更新 README

验收标准：

- `docs/stage-1-retrospective.md` 存在
- 有至少 5 条具体复盘

