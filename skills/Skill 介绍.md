# Skill 介绍

本文根据各目录下的 `SKILL.md` 整理，用于快速了解这些 Skill 的用途、触发场景和主要能力。

## 总览

| Skill | 主要用途 | 适合场景 |
| --- | --- | --- |
| `algorithmic-art` | 使用 p5.js、随机种子和可调参数创建算法艺术。 | 生成艺术、代码艺术、流场、粒子系统、交互式视觉探索。 |
| `brand-guidelines` | 将 Anthropic 官方品牌颜色、字体和视觉规范应用到产物中。 | 品牌化文档、演示稿、网页、视觉素材或任何需要统一公司风格的内容。 |
| `canvas-design` | 基于设计哲学创建静态视觉作品，并输出 `.png` 或 `.pdf`。 | 海报、艺术图、静态设计稿、视觉排版作品。 |
| `claude-api` | 构建、调试和优化 Claude API / Anthropic SDK 应用。 | Claude API、Anthropic SDK、Managed Agents、提示缓存、工具调用、批处理、文件 API、模型迁移。 |
| `doc-coauthoring` | 引导用户共同撰写结构化文档。 | 技术方案、提案、决策文档、产品说明、长文档协作。 |
| `docx` | 创建、读取、编辑和分析 Word `.docx` 文件。 | Word 报告、备忘录、信函、模板、批注、修订、图片替换、格式化文档。 |
| `frontend-design` | 创建具有高设计质量的生产级前端界面。 | 网站、落地页、仪表盘、React 组件、HTML/CSS 布局、Web UI 美化。 |
| `internal-comms` | 按公司偏好的格式撰写内部沟通内容。 | 状态报告、领导层更新、3P 更新、公司通讯、FAQ、事故报告、项目更新。 |
| `mcp-builder` | 指导创建高质量 MCP 服务器。 | 为 LLM 集成外部 API 或服务，使用 Python FastMCP 或 Node/TypeScript MCP SDK。 |
| `pdf` | 处理 PDF 文件的读取、创建、编辑和转换。 | 提取文本/表格、合并拆分、旋转、水印、表单填写、加密解密、OCR。 |
| `pptx` | 创建、读取、编辑和验证 PowerPoint `.pptx` 演示文稿。 | 幻灯片、deck、pitch deck、演示稿、模板、布局、讲者备注、评论。 |
| `skill-creator` | 创建、修改、优化和评估 Skill。 | 从零创建 Skill、改写 `SKILL.md`、运行评测、优化触发描述、打包 Skill。 |
| `slack-gif-creator` | 创建面向 Slack 优化的动画 GIF。 | Slack 表情、动图、简单角色动画、循环动画、尺寸和体积受限的 GIF。 |
| `theme-factory` | 为各类产物应用或生成主题。 | 幻灯片、文档、报告、HTML 页面等需要统一配色和字体的产物。 |
| `web-artifacts-builder` | 构建复杂的 claude.ai HTML artifacts。 | 多组件 Artifact、React、Tailwind CSS、shadcn/ui、状态管理或路由。 |
| `webapp-testing` | 使用 Playwright 与本地 Web 应用交互并测试。 | 前端功能验证、UI 调试、截图、浏览器日志、自动化点击和输入。 |
| `xlsx` | 创建、读取、编辑和分析电子表格文件。 | `.xlsx`、`.xlsm`、`.csv`、`.tsv` 文件处理，公式、格式、图表、数据清洗。 |

## 分组说明

### 创意与视觉设计

`algorithmic-art` 面向生成式视觉创作。它强调先形成算法哲学，再用 p5.js 实现可复现、可探索的视觉系统，适合需要随机性、参数调节和交互预览的艺术作品。

`canvas-design` 面向静态视觉设计。它关注画面构成、字体、色彩、层次和输出质量，适合生成海报、封面、艺术图或其他静态图形产物。

`frontend-design` 面向真实可用的前端界面。它要求界面具备清晰的信息结构、良好的视觉完成度和产品级交互体验，避免泛化模板感。

`theme-factory` 是主题应用工具。它提供预设主题，也支持按需生成新主题，用于统一文档、幻灯片、网页或报告的视觉风格。

`brand-guidelines` 专注 Anthropic 品牌规范。它适用于需要采用 Anthropic 官方颜色、字体和整体观感的产物。

### Web 与应用构建

`web-artifacts-builder` 用于创建复杂 HTML Artifact。相比简单单文件 HTML，它更适合需要 React、Tailwind、shadcn/ui、状态管理、路由或多组件结构的交互式产物。

`webapp-testing` 用于本地 Web 应用测试。它通过 Playwright 自动化浏览器操作，支持功能验证、界面检查、截图采集和日志排查。

`mcp-builder` 用于开发 MCP 服务器。它覆盖从需求研究、协议理解、项目结构、工具设计、实现、测试到评估问题设计的完整流程。

`claude-api` 用于 Claude API 和 Anthropic SDK 应用开发。它覆盖多语言 SDK、提示缓存、工具调用、流式输出、文件 API、批处理、Managed Agents 和模型迁移。

### 文档与办公文件

`doc-coauthoring` 是文档共创工作流。它通过上下文收集、结构梳理、迭代打磨和读者测试，帮助产出更适合目标读者的文档。

`docx` 负责 Word 文件处理。它适合创建专业 Word 文档、读取内容、编辑 XML、处理目录、页眉页脚、批注、修订和图片等。

`pdf` 负责 PDF 文件处理。它覆盖文本和表格提取、页面操作、表单处理、水印、OCR、加密解密、图片提取和新 PDF 生成。

`pptx` 负责 PowerPoint 文件处理。它覆盖幻灯片读取、创建、编辑、设计建议、图片预览、内容 QA 和视觉 QA。

`xlsx` 负责电子表格处理。它强调公式优先、避免硬编码计算结果，并支持数据清洗、格式化、图表、财务模型规范和公式校验。

### 沟通、协作与扩展

`internal-comms` 用于内部沟通写作。它提供常见内部沟通格式和示例，包括领导层更新、FAQ、公司通讯、项目更新和事故报告。

`skill-creator` 用于 Skill 的全生命周期管理。它不仅能创建和修改 Skill，还能设计测试用例、运行评测、对比基线、优化描述并生成报告。

`slack-gif-creator` 用于 Slack 动图制作。它包含 GIF 尺寸、帧数、优化、动画曲线、图形绘制和验证工具，适合制作轻量、循环、表达明确的 Slack GIF。

## 选择建议

如果任务涉及具体文件格式，优先选择对应文件 Skill：Word 用 `docx`，PDF 用 `pdf`，PowerPoint 用 `pptx`，电子表格用 `xlsx`。

如果任务是视觉产物，先区分输出类型：动态或生成式艺术用 `algorithmic-art`，静态海报或图形用 `canvas-design`，产品界面用 `frontend-design`，统一主题用 `theme-factory`，Anthropic 品牌风格用 `brand-guidelines`。

如果任务是系统或工程能力，Claude API 应用用 `claude-api`，MCP 服务器用 `mcp-builder`，本地 Web 应用测试用 `webapp-testing`，复杂 HTML Artifact 用 `web-artifacts-builder`。

如果任务是写作或组织内容，结构化文档共创用 `doc-coauthoring`，内部沟通内容用 `internal-comms`，创建或优化 Skill 用 `skill-creator`。
