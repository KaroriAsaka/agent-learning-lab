# LLM Gateway

练习目标：把 LLM 调用封装成一个后端服务，而不是散落在业务代码里。

## First Version

接口：

- `POST /chat`
- `POST /summarize`
- `POST /extract`

能力：

- timeout
- retry
- request_id
- structured output validation
- token and latency logging

## Suggested Stack

- Python
- FastAPI
- Pydantic
- pytest

## Notes

先实现最小版本，再考虑多 provider、streaming、auth、rate limit。

