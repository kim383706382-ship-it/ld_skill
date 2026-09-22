# management_writing｜管理学论文写作 Skill v0.1

**中英文统一风格；段落结构变动须事先批准。**

这是一份依据你认可的三篇范文整理的个人写作Skill初版。它不是模型微调，也不是论文模板填空：主文件决定何时使用、读哪些规则、哪些修改需先询问；参考文件保存从标题到附录的写作方式、公开来源说明与语言适配示例；不附原文长段摘录。

## 已纳入的约定
中文和英文采用相同的研究叙事与论证原则，分别以自然的学术语言实现。中英都包含在第一版，不要求每次同时输出两个版本。

段落内可以调整措辞、句法、句序和衔接。移动、拆分、合并、增删段落以及跨段转移内容，必须先说明“改哪里、如何改、为什么”，得到你对具体方案的明确同意后才执行。新理论、构念、假设或实质结论的变化另行确认。

普通写作细节由助手依据范文判断；不再要求你填写覆盖所有细节的长问卷。

## 文件怎么分工
| 文件 | 内容 |
|---|---|
| SKILL.md | 核心入口、使用步骤与修改权限 |
| references/01-narrative-and-argument.md | 标题、摘要、引言、综述、理论、假设 |
| references/02-bilingual-prose.md | 中英表达、段落与句法、语言适配示例 |
| references/03-studies-and-methods.md | 研究概览、预实验、样本、程序、测量 |
| references/04-results-and-statistics.md | 结果组织、统计外观、主效应、交互及中介报告 |
| references/05-discussion-and-presentation.md | 讨论、贡献、启示、局限、图表、附录与声明 |
| references/06-exemplars-and-provenance.md | 42项写法索引、公开来源定位、精读方法与不可照搬的问题；私人来源细节已省略 |
| references/07-editing-permissions.md | 段落与内容变动的事前审批规则 |
| references/08-review-and-coverage.md | 全文覆盖与交付核对，不是用户问卷 |
| assets/source-index.json | 公开文献书目信息及来源边界，不含原件路径或私人原件哈希 |
| agents/openai.yaml | 可选界面名称与调用配置 |
| tests/scenarios.md | 12个待实测场景，明确区分检查与真正验收 |

## 使用与安装状态
本仓库提供可独立使用的公开文件，不代表已安装到任何客户端；既有论文原件未修改。

本包使用“一个目录＋SKILL.md＋参考材料”的结构。OpenAI官方文档列出的本地Codex个人技能位置为：

```text
~/.agents/skills/management-writing/SKILL.md
```

后续在本地安装时，将仓库内 skills/management-writing 文件夹放入个人技能目录，保留references、assets等子目录，不能只复制SKILL.md。同名旧版本先留存再替换，避免两个副本造成重复。该步骤需你在本机执行，或明确授权可访问本机的工具完成。

官方文档区分调用方式：ChatGPT界面用@选择已可用技能；Codex CLI／IDE使用/skills或$提及技能。是否已被你的界面识别，需要在那里实际检查；下载ZIP或在聊天里提到名字都不等于已经安装。本包没有附加自动发布或上传原始论文的操作。

技术结构与本地路径参考（核对日期：2026-09-22；该来源仅用于技能格式，不参与管理学文风提炼）：

```text
OpenAI — Build skills
https://learn.chatgpt.com/docs/build-skills
原入口：https://developers.openai.com/codex/skills/
```

## 实际使用时的简短请求
已有稿件：

> 按管理学论文写作Skill修改以下内容。段落内可以调整句式与句序，段落结构变动先提出方案。保留研究事实、构念、引用与结果。

从零起草：

> 按管理学论文写作Skill，用我提供的研究材料起草中文／英文的这一部分。材料未支持的事实、文献和数据不要补造。

## 目前完成到哪里
已整理核心指令、分部分写作规则、公开来源说明和双语适配示例。公开文件结构、相对引用和校验值可独立核对；原件不随仓库提供，也不是使用规则的必读依赖。

仍需用你的新稿确认实际写作效果；尚未完成独立代理的重复行为测试，也没有证据保证每次自动调用。三篇原件均为英文，因此中文实现是已明确标注的语言适配，而不是谎称另有中文范文验证。

公开版已移除原件、长段原文以及未确认可公开稿件的具体内容。私人参考材料仅在本地保留，放入被忽略的 private-references/ 目录；不得因分享 Skill 而一并提交。

## GitHub 仓库命名
仓库名称及界面显示名称为 `management_writing`；为符合 Agent Skills 的标识规则，内部名称和技能目录使用 `management-writing`。仓库内安装入口为 `skills/management-writing/`。公开整理仅调整受限制的来源内容及分发说明，核心写作要求和段落审批规则保留。
