# XHS Post-Publish Review Skill

Open Skill for reviewing Xiaohongshu / RedNote post-publish data using note link, backend screenshots, title, cover, script, caption, and 24h/48h/7d checkpoints.

中文一句话：根据小红书 / RedNote 发布后的链接、截图、标题封面和 24h/48h/7d 数据，判断下一条该怎么改。

## Search Keywords

English keywords:

`Xiaohongshu post-publish review`, `RedNote data review`, `XHS analytics review`, `social media content review`, `24 hour content review`, `creator data review`, `post performance diagnosis`, `AI skill for creators`.

中文关键词：

`小红书发布后复盘`, `小红书数据复盘`, `后台截图分析`, `24小时复盘`, `48小时复盘`, `7天复盘`, `内容数据分析`, `创作者复盘工具`.

## Why This Exists


A data screenshot alone does not explain what to change. The review must connect exposure, click, read/completion, saves, comments, shares, and follows back to the exact content.
This Skill turns post-publish review into a next-test decision instead of a vague data summary.

## What It Can Do

- what the data most likely means
- where the note is leaking users
- what to change next time
- whether to remake title, cover, opening, body, or topic
- one next publishing experiment

## Best Inputs

- note link or identifier
- title and cover
- script, caption, or page text
- backend screenshot or manually typed metrics
- publish time and checkpoint: 24h, 48h, or 7d
- content goal

## Workflow

- Match data to the exact note.
- Judge exposure and click issues.
- Judge read, completion, or retention issues.
- Judge save, comment, share, and follow conversion.
- Connect the data back to title, cover, opening, body, and audience promise.
- Choose one next test.

## Output Contract

Default output:

1. Scope and assumptions
2. Input reading
3. Main judgment
4. Structured table or checklist
5. Recommended next action
6. Boundary notes

For detailed rules, see `references/workflow-rules.md`.

## Example Prompt

```text
Use $xhs-postpublish-review for this task:
Checkpoint: 24h
Title: 收藏了 20 个 AI 工具，为什么还是发不出来？
Cover: 你缺的不是工具，是内容流程
Data: low click, medium read, high save among readers
Goal: saves and follows
```

## Example Output Shape

See `examples/sample-output.md` for a short sample.

## Open-Source Boundary

This standalone open version includes:

- reusable creator workflow instructions
- input and output contracts
- workflow rules
- example output
- Agent metadata
- MIT license

This standalone open version does not include:

- private platform credentials
- automatic publishing
- private analytics connectors
- scraping or monitoring
- guaranteed traffic, growth, sales, or viral outcomes
- copying another creator's content
- internal operating notes or private project context

## Repository Map

- `SKILL.md`: Agent entrypoint and workflow rules
- `agents/openai.yaml`: Agent display metadata
- `references/workflow-rules.md`: detailed workflow and quality rules
- `examples/sample-output.md`: sample input and output shape
- `LICENSE`: MIT license

## Recommended GitHub Description

> Open Skill for reviewing Xiaohongshu / RedNote post-publish data using note link, backend screenshots, title, cover, script, caption, and 24h/48h/7d checkpoints.

## Suggested GitHub Topics

`postpublish-review`, `analytics-review`, `xiaohongshu`, `rednote`, `creator-tools`, `content-workflow`, `social-media`, `ai-skill`, `open-source`

## License

MIT
