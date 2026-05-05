# Obsidian Note Summarizer

练习目标：读取本地 Obsidian Markdown 笔记，生成结构化摘要。

## Input

Markdown files from an Obsidian Vault.

## Output

JSON summary:

```json
{
  "title": "string",
  "summary": "string",
  "key_points": ["string"],
  "tags": ["string"],
  "related_notes": ["string"]
}
```

## First Version

- [ ] Scan `.md` files
- [ ] Skip `.obsidian/`
- [ ] Skip empty files
- [ ] Generate summary JSON
- [ ] Save results to `.summaries/`

## Later

- Recommend backlinks
- Write summaries back into notes
- Feed summaries into RAG pipeline

