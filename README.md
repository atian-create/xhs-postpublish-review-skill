# 小红书发布后复盘 Skill

这是一个给小红书 / RedNote 创作者用的开源轻量 Skill：当一条内容已经发布，你拿到了链接、后台截图、标题封面、正文和 24h / 48h / 7d 数据后，它帮你判断问题到底出在哪里，以及下一条内容该测试什么。

很多人复盘数据时只会看“好不好”，但不知道“为什么”：

- 曝光低，是选题问题还是账号阶段问题？
- 点击低，是标题问题还是封面第一眼不清楚？
- 阅读/完播一般，是开头慢了还是结构太散？
- 收藏不错但关注少，是内容有用但主页承接弱？
- 评论少，是没有讨论点，还是用户需求没有被打开？

这个 Skill 会把数据重新接回内容本身：标题、封面、前三行/前三秒、正文结构、用户承诺和账号目标，最后给出一个下一条最小实验。

## 你下载后可以用它做什么

- 根据 24h、48h、7d 数据做发布后复盘。
- 判断问题更可能发生在曝光、点击、阅读/完播、收藏、评论、分享还是关注转化。
- 把数据和标题、封面、开头、正文、受众承诺连接起来。
- 判断下一条应该改标题、封面、开头、正文，还是重新定选题。
- 保留有效信号，避免一条数据不好就全部推翻。
- 输出一个下一条内容可以验证的小实验。

## 适合谁

- 已经发了内容，但看不懂后台数据的人。
- 想做 24 小时、48 小时、7 天复盘的创作者。
- 经常觉得“数据不好但不知道改哪里”的运营者。
- 给客户做小红书复盘报告的人。
- 想让 Agent 帮自己形成持续复盘习惯的人。

## 为什么这个 Skill 值得单独装

普通数据分析容易停在“点击低、收藏高、互动一般”这种描述。真正有用的复盘，必须回答下一条怎么改。

这个 Skill 会按链路判断：

1. 曝光：平台有没有给到初始展示。
2. 点击：标题和封面有没有第一眼理由。
3. 阅读/完播：开头和结构有没有留住用户。
4. 收藏：内容是否解决了实际问题。
5. 评论：是否激发了提问、共鸣或补充。
6. 关注：主页和账号承诺是否接得住这条内容。

最后它会帮你选择一个最小实验，而不是让你同时改十件事。

## 3 分钟上手

把这个仓库里的 `SKILL.md` 放到你的 Agent Skill 目录，然后这样问：

```text
用 xhs-postpublish-review 帮我复盘这条小红书。
检查点：24 小时
标题：收藏了 20 个 AI 工具，为什么还是发不出来？
封面：你缺的不是工具，是内容流程
正文概要：讲从选题、写稿到复盘的三步流程
数据：曝光一般，点击偏低，读完率中等，收藏率高，关注少
目标：希望下一条提高点击和关注
```

## 你会拿到什么结果

默认输出会包括：

- 这组数据最可能说明什么。
- 用户在哪一步流失。
- 哪个环节最该先改。
- 下一条内容应该保留什么。
- 下一条内容只测试一个什么变量。
- 24h / 48h / 7d 后继续看什么。

## 公开版边界

这个开源版只基于你提供的数据截图、文字指标和内容材料做判断。它不登录后台，不自动拉取数据，不承诺下一条一定变好。它的作用是把一次发布变成下一次更清楚的实验。

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
