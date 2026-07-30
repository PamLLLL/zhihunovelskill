---
description: 知乎盐选故事生成器 — 一键生成签约级短篇故事
allowed-tools: Read, Write, Bash, AskUserQuestion
---

# 知乎盐选故事生成器

用户触发了知乎故事生成流程。

首先读取工作流主文件：
1. `/home/liuy405/.claude/plugins/local/zhihu-story-generator/skills/zhihu-story/SKILL.md` — 完整工作流指令（Phase 1-4 + Phase 3.5 + Phase 3.8）

**重要：不要一次性读取所有参考文件。** 参考文件在各 Phase 按需读取（SKILL.md 中有明确标注），避免撑满 context 导致生成卡住。

然后严格按照 SKILL.md 中的 Phase 1-4（含 Phase 3.5 反检测改写 + Phase 3.8 质量自检）执行。

用户的额外参数：$ARGUMENTS
