> **注意：** 本仓库包含 Anthropic 为 Claude 实现的技能。有关 Agent Skills 标准的信息，请参阅 [agentskills.io](http://agentskills.io)。

[![skills.sh](https://skills.sh/b/anthropics/skills)](https://skills.sh/anthropics/skills)

# 技能

技能是由指令、脚本和资源组成的文件夹，Claude 会动态加载它们，以提升在专门任务上的表现。技能会教 Claude 如何以可重复的方式完成特定任务，无论是按照你公司的品牌指南创建文档、使用你所在组织的特定工作流程分析数据，还是自动化个人任务。

如需更多信息，请查看：
- [什么是技能？](https://support.claude.com/en/articles/12512176-what-are-skills)
- [在 Claude 中使用技能](https://support.claude.com/en/articles/12512180-using-skills-in-claude)
- [如何创建自定义技能](https://support.claude.com/en/articles/12512198-creating-custom-skills)
- [使用 Agent Skills 为真实世界装备智能体](https://anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills)

# 关于本仓库

本仓库包含一些技能，用于展示 Claude 技能系统可以实现的能力。这些技能覆盖从创意应用（艺术、音乐、设计）到技术任务（测试 Web 应用、生成 MCP 服务器），再到企业工作流（沟通、品牌等）的多种场景。

每个技能都在自己的文件夹中自成一体，并包含一个 `SKILL.md` 文件，其中写有 Claude 使用的指令和元数据。你可以浏览这些技能，为自己的技能获得灵感，或了解不同的模式和实现方法。

本仓库中的许多技能都是开源的（Apache 2.0）。我们还收录了支撑 [Claude 文档能力](https://www.anthropic.com/news/create-files) 的文档创建与编辑技能，它们位于 [`skills/docx`](./skills/docx)、[`skills/pdf`](./skills/pdf)、[`skills/pptx`](./skills/pptx) 和 [`skills/xlsx`](./skills/xlsx) 子文件夹中。这些技能是源码可见的，但不是开源项目；我们希望把它们作为参考分享给开发者，用于了解更复杂的技能，这些技能正在生产级 AI 应用中被实际使用。

## 免责声明

**这些技能仅用于演示和教育目的。** 虽然 Claude 中可能提供其中一些能力，但你从 Claude 获得的实现和行为可能不同于这些技能中展示的内容。这些技能旨在说明模式和可能性。在将技能用于关键任务之前，请务必在你自己的环境中充分测试。

# 技能集合

- [./skills](./skills)：面向创意与设计、开发与技术、企业与沟通以及文档技能的技能示例
- [./spec](./spec)：Agent Skills 规范
- [./template](./template)：技能模板

# 在 Claude Code、Claude.ai 和 API 中试用

## Claude Code

你可以在 Claude Code 中运行以下命令，将本仓库注册为 Claude Code 插件市场：

```
/plugin marketplace add anthropics/skills
```

然后，如需安装特定的一组技能：

1. 选择 `Browse and install plugins`
2. 选择 `anthropic-agent-skills`
3. 选择 `document-skills` 或 `example-skills`
4. 选择 `Install now`

也可以通过以下命令直接安装任一插件：

```
/plugin install document-skills@anthropic-agent-skills
/plugin install example-skills@anthropic-agent-skills
```

安装插件后，只需提及相应技能即可使用。例如，如果你从市场安装了 `document-skills` 插件，可以让 Claude Code 执行类似这样的任务：“使用 PDF 技能从 `path/to/some-file.pdf` 中提取表单字段。”

## Claude.ai

这些示例技能已经面向 Claude.ai 的付费套餐开放。

如需使用本仓库中的任意技能或上传自定义技能，请按照 [在 Claude 中使用技能](https://support.claude.com/en/articles/12512180-using-skills-in-claude#h_a4222fa77b) 中的说明操作。

## Claude API

你可以通过 Claude API 使用 Anthropic 预构建的技能，也可以上传自定义技能。更多信息请参阅 [Skills API 快速入门](https://docs.claude.com/en/api/skills-guide#creating-a-skill)。

# 创建基础技能

技能很容易创建，只需要一个文件夹，其中包含一个带 YAML frontmatter 和指令的 `SKILL.md` 文件。你可以使用本仓库中的 **template-skill** 作为起点：

```markdown
---
name: my-skill-name
description: 清晰描述这个技能做什么，以及何时应该使用它
---

# 我的技能名称

[在这里添加 Claude 会在此技能激活时遵循的指令]

## 示例
- 示例用法 1
- 示例用法 2

## 指南
- 指南 1
- 指南 2
```

frontmatter 只需要两个字段：
- `name`：技能的唯一标识符（小写，使用连字符代替空格）
- `description`：完整描述这个技能做什么以及何时使用它

下面的 Markdown 内容包含 Claude 将遵循的指令、示例和指南。更多细节请参阅 [如何创建自定义技能](https://support.claude.com/en/articles/12512198-creating-custom-skills)。

# 合作伙伴技能

技能是一种很好的方式，可以教 Claude 更好地使用特定软件。当我们看到合作伙伴提供的优秀示例技能时，可能会在这里重点展示其中一些：

- **Notion** - [Claude 的 Notion Skills](https://www.notion.so/notiondevs/Notion-Skills-for-Claude-28da4445d27180c7af1df7d8615723d0)
