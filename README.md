# management_writing

**让研究问题更清楚，让理论推导更连贯，让每一个结论都有证据支撑。**

management_writing 是面向中英文管理学实证论文的 AI 写作 Skill。它将论文精读中总结的写作方法整理为一套可复用的指引，帮助 AI 在起草、润色和修订时，把研究问题、理论解释与实证证据连接起来。

从引言如何引出问题，到假设如何逐步推导，再到结果如何准确呈现，它关注论文各部分的论证任务，也关注句子之间的信息衔接。你提供研究材料与写作目标，Skill 为写作过程提供一致的表达原则和修改边界。

[查看写作指引](skills/management-writing/SKILL.md) · [详细使用说明](skills/management-writing/README.zh-CN.md) · [修改权限](skills/management-writing/references/07-editing-permissions.md)

## 它可以帮你做什么

| 写作场景 | 关注重点 |
|---|---|
| 标题与摘要 | 准确概括问题、核心发现与适用边界，让读者快速理解研究 |
| 引言与文献综述 | 从具体情境进入研究问题，说明已有认识与本文的解释空间 |
| 理论与假设 | 写清构念之间为什么存在联系，让机制推导有必要的解释步骤 |
| 研究与方法 | 交代各项研究的分工、设计、程序与测量，使描述便于理解和核对 |
| 结果呈现 | 按研究问题组织统计证据，保留数值、比较方向和真实支持程度 |
| 讨论与贡献 | 回答研究问题，说明新增认识、管理含义及仍未解决的局限 |
| 中英文修订与转写 | 用两种语言自然表达相同的构念、命题、条件与证据 |

适合正在起草论文、修改已有段落，或希望统一全文叙事与表达方式的研究者。使用时，可以从一段理论、一段结果或一小节引言开始。

## 写得更清楚，也尊重你的研究

**围绕论证任务修改。** 每个段落要解决什么问题、句子如何接续、例子怎样回到理论关系，都有对应的写作指引。无需把所有论文写成同一种模板。

**中文与英文同样重要。** 两种语言共享叙事和论证原则，各自采用自然的学术表达。按你指定的语言交付；需要中英对照时，再核对两个版本的语义一致性。

**段落结构由你决定。** 原段落内可以调整措辞、句法、句序和衔接。移动、拆分、合并、增删段落或跨段转移内容，必须先提出具体方案，得到你的明确同意后再执行。

**事实与证据保持准确。** 研究问题、构念、引用、数据和结论强度不能为了文风而擅自改变。材料存在缺项或冲突时，应明确指出，不能补造数字、文献或研究发现。

## 从一个具体请求开始

向支持 Skill 的客户端提供你的稿件或研究材料，并说明希望处理的部分。例如：

**润色已有段落**

> 请使用 $management-writing 润色以下中文理论段落。保留研究事实、构念和引用；段落内可以调整句式与句序，段落结构变动先提出方案，等我同意后再执行。

**依据材料起草**

> 请使用 $management-writing，根据我提供的研究背景和文献笔记起草引言。把研究问题与理论解释连接起来，材料未支持的事实和引用请标注待补充。

**进行中英转写**

> 请使用 $management-writing，将以下内容改写为自然的学术英文。保持原段落边界、构念、引用和证据强度，不要求逐句直译。

## 安装与使用

将仓库中的整个 `skills/management-writing/` 文件夹复制到本地技能目录，保留全部子目录。已有同名版本时先备份。

Codex 用户级安装后的预期位置为：

```text
~/.agents/skills/management-writing/SKILL.md
```

在支持该调用方式的 Codex CLI／IDE 中，可用 `$management-writing` 显式提及。安装后需在当前客户端确认技能已被识别；下载仓库或在聊天中输入名称不等于已经加载。

仓库与界面显示名称为 `management_writing`，内部 Skill 标识和目录名称为 `management-writing`。完整说明见[使用文档](skills/management-writing/README.zh-CN.md)。

## 仓库内容

```text
management_writing/
├── README.md
├── .gitignore
├── .gitattributes
├── CHANGELOG.md
├── PUBLICATION.md
├── checksums.sha256
└── skills/
    └── management-writing/
        ├── SKILL.md
        ├── README.zh-CN.md
        ├── agents/openai.yaml
        ├── references/               # 八份写作、权限与检查指引
        ├── assets/source-index.json  # 公开书目信息与来源边界
        └── tests/scenarios.md        # 12个待行为验证的场景
```

## 来源与当前版本

写作方法由三篇参考材料的精读形成，主要涉及消费者行为与人机互动实证研究，覆盖标题、摘要、引言、理论、方法、结果、讨论及图表附录。它们提供写法参考，不构成所有管理学体裁或统计方法的通用规范。

中文表达是依据共同叙事原则作出的语言适配。当前版本仍需通过实际稿件持续校准；行为测试与用户新稿验收尚未完成，也不保证任何客户端都会自动调用。Skill 用于写作与表达，不替代文献核查、研究设计或统计判断。

公开仓库保留自行总结的写作方法、公开文献引用与 DOI，不附三篇原始 PDF／Word、论文页面截图、大段原文摘录或未确认可公开的稿件内容。使用规则不依赖私人原件。详情见[来源说明](skills/management-writing/references/06-exemplars-and-provenance.md)和[公开整理记录](PUBLICATION.md)。

私人材料应放入 `.gitignore` 已排除的 `private-references/` 等目录，避免误提交。本仓库未添加开放许可证，公开可访问不代表获得第三方材料的再分发授权。

可在仓库根目录运行 `shasum -a 256 -c checksums.sha256` 检查文件完整性。

技术格式参考：[Agent Skills Specification](https://agentskills.io/specification) · [OpenAI — Build skills](https://developers.openai.com/codex/skills)。这些资料用于说明技能格式与使用方式，不是管理学写作方法的来源。
