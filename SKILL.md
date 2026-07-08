---
name: xhs-postpublish-review
description: "Open Skill for reviewing Xiaohongshu / RedNote post-publish data using note link, backend screenshots, title, cover, script, caption, and 24h/48h/7d checkpoints. Use when the user asks for Xiaohongshu post-publish review, RedNote data review, XHS analytics review, social media content review, 小红书发布后复盘, 小红书数据复盘, 后台截图分析, 24小时复盘. This Skill uses user-provided material and public-safe reasoning only; it does not publish automatically, scrape private data, copy creators, or promise growth."
---

# Xiaohongshu Post-Publish Review

## Purpose

根据小红书 / RedNote 发布后的链接、截图、标题封面和 24h/48h/7d 数据，判断下一条该怎么改。

This is a lightweight standalone open Skill. It turns a repeated creator task
into a clear Agent workflow with inputs, checks, output shape, and boundaries.

## Use This For

- what the data most likely means
- where the note is leaking users
- what to change next time
- whether to remake title, cover, opening, body, or topic
- one next publishing experiment

## Do Not Use This For

- automatic publishing
- private account login
- private data extraction
- guaranteed traffic, growth, sales, or viral outcomes
- copying another creator's exact wording, identity, images, or claims
- making claims that the user's material does not support

## Inputs

- note link or identifier
- title and cover
- script, caption, or page text
- backend screenshot or manually typed metrics
- publish time and checkpoint: 24h, 48h, or 7d
- content goal

If the input is incomplete, proceed with a first-pass version and mark
assumptions. Ask only the smallest necessary follow-up when the missing detail
would materially change the result.

## Workflow

Read `references/workflow-rules.md` when the task needs the full rule set.

- Match data to the exact note.
- Judge exposure and click issues.
- Judge read, completion, or retention issues.
- Judge save, comment, share, and follow conversion.
- Connect the data back to title, cover, opening, body, and audience promise.
- Choose one next test.

## Output Contract

```markdown
## 1. Scope And Assumptions

## 2. Input Reading

## 3. Main Judgment

## 4. Working Table Or Checklist

## 5. Recommended Next Action

## 6. Boundaries
```

## Quality Bar

- Be specific and operational.
- Prefer a small usable output over a broad lecture.
- Explain why each recommendation fits the user's material.
- Mark weak evidence instead of pretending certainty.
- Do not promise results.
- Do not copy another creator's protected expression or personal story.

## Tone

Write in the user's language. For Chinese creator tasks, default to clear,
practical Chinese.

## Public Boundary

Keep examples generic. Do not include internal thread IDs, private file paths,
unpublished customer material, private account data, or internal product notes.
