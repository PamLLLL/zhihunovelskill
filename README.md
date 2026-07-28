# 知乎盐选故事生成器

Claude Code Skill，一键生成知乎盐选签约级短篇故事。

## 功能

输入 `/zhihu-story`，自动走完完整流程：

1. 选择类型（古言/现言/悬疑/脑洞）和子类型
2. AI 头脑风暴 5 个故事概念，你选一个
3. 一气呵成生成 8000-15000 字完整故事
4. 自动生成发布素材（书名、标签、简介、金句）
5. 保存到桌面

## 安装

```bash
# 将插件路径添加到 Claude Code 全局设置
claude mcp add-plugin /path/to/zhihu-story-generator
```

或手动编辑 `~/.claude/settings.json`：

```json
{
  "plugins": ["/absolute/path/to/zhihu-story-generator"]
}
```

## 使用

在任意 Claude Code 会话中：

```
/zhihu-story
```

或直接说：

```
帮我写个知乎古言甜宠故事
```

## 写作标准

内置知乎盐选编辑审稿标准：
- 第一人称叙事
- 高潮切入开篇
- 每千字至少一个看点
- 全套去 AI 味规则（禁词表 + 替代方案 + Show don't tell）
- 四条过稿防拒指南
- 类型专属写作规则
