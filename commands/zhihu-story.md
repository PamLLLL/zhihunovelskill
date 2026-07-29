---
description: 知乎盐选故事生成器 — 一键生成签约级短篇故事
allowed-tools: Read, Write, Bash, AskUserQuestion
---

# 知乎盐选故事生成器

用户触发了知乎故事生成流程。

首先读取以下文件获取完整工作流和写作规则：
1. `/home/liuy405/.claude/plugins/local/zhihu-story-generator/skills/zhihu-story/SKILL.md` — 完整工作流指令（Phase 1-4 + Phase 3.5 + Phase 3.8）
2. `/home/liuy405/.claude/plugins/local/zhihu-story-generator/skills/zhihu-story/references/anti-detection.md` — 反AI检测策略（最高优先级）
3. `/home/liuy405/.claude/plugins/local/zhihu-story-generator/skills/zhihu-story/references/quality-checklist.md` — 生成后质量自检清单
4. `/home/liuy405/.claude/plugins/local/zhihu-story-generator/skills/zhihu-story/references/zhihu-editorial.md` — 知乎编辑标准
5. `/home/liuy405/.claude/plugins/local/zhihu-story-generator/skills/zhihu-story/references/writing-style.md` — 写作风格规则
6. `/home/liuy405/.claude/plugins/local/zhihu-story-generator/skills/zhihu-story/references/zhihu-baokuan-style.md` — 爆款风格模式
7. `/home/liuy405/.claude/plugins/local/zhihu-story-generator/skills/zhihu-story/references/genre-guides.md` — 类型指南

然后严格按照 SKILL.md 中的 Phase 1-4（含 Phase 3.5 反检测改写 + Phase 3.8 质量自检）执行。

用户的额外参数：$ARGUMENTS
