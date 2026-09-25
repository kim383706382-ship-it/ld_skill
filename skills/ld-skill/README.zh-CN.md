# ld_skill 使用说明

`ld` 来自作者一位名叫 LD 的老师。这个 Skill 把从其写作指导中学到的判断，与管理学实证论文的写法整理为可调用的工作方法：读懂研究材料，找出论证断点，在证据允许的范围内写得更清楚。项目介绍、示例与版本验证见[仓库 README](../../README.md)。

## 从一句话开始

在已经安装本 Skill 的项目中，直接说出需求即可；需要明确指定时，用 `$ld-skill`：

> 请使用 $ld-skill，结合这部分批注、引言和结果，修改假设推导。说明文献为哪一步提供前提，写清相邻变量为什么有关联，核对比较方向。保留构念与证据强度，跨段调整先给出具体方案。

请尽量提供待处理原文、相关上下文、批注、文献及结果。没有的资料不会被当作已有证据。可指定只要中文或英文、直接替换稿、修改理由、篇幅或原文档格式；没有额外要求时只交付任务所需的内容。

## 适用内容

- **引言、文献综述和假设：**从研究问题进入理论解释，检查前提、相邻关系、机制与条件比较。[论证指南](references/01-narrative-and-argument.md)与[理论专项指南](references/09-literature-and-hypothesis-development.md)
- **研究设计与方法：**交代研究分工、样本、程序和测量，保持准确与简洁。[方法指南](references/03-studies-and-methods.md)
- **结果与讨论：**按研究问题呈现证据，再说明新增认识和局限。[结果指南](references/04-results-and-statistics.md)、[讨论指南](references/05-discussion-and-presentation.md)
- **中英文写作：**保留相同命题和证据强度，分别写出自然表达。[双语指南](references/02-bilingual-prose.md)

理论专项指南只在相应任务中读取，不会要求所有段落套用固定假设结构。

## 修改边界

原段落内可以优化措辞、句序和衔接。移动、拆分、合并、增删段落或跨段转移内容，必须先提出“原位置—拟调整—理由—影响”，取得对具体方案的同意后执行。已有明确授权继续有效，不重复索要。构念、机制、假设、事实、数据、引用对应关系与证据强度不能作为文风调整擅自改变。[完整权限规则](references/07-editing-permissions.md)

示例只是帮助读者理解推理，不能冒充实证结果；所需前提缺失时应指出具体缺口，不能替作者编造文献或研究发现。[来源边界](references/06-exemplars-and-provenance.md)、[交付检查](references/08-review-and-coverage.md)

## 安装与更新

将**整个** `ld-skill` 目录放入项目的 `.agents/skills/`。`SKILL.md` 是入口，`references/`、`assets/`、`tests/` 和 `agents/` 是随附资源，不能只复制入口文件。显示名为 `ld_skill`；内部名称和目录为 `ld-skill`。项目级安装不自动更新其他项目、全局目录或网页版。

更新时先备份现有目录，再放入新版，并在项目新会话中实际调用一次，核对读取路径。当前公开版本见[GitHub main](https://github.com/kim383706382-ship-it/ld_skill/tree/main/skills/ld-skill)；从 GitHub 下载不等于客户端已加载。旧版备份和恢复位置以你的安装记录为准。

## 来源与验证

公开包不包含原始论文、私人精读或真实稿件。原创例子解释写法，不是可引用的研究证据。具体评测见[本轮验证记录](https://github.com/kim383706382-ship-it/ld_skill/blob/main/docs/updates/completion-validation-20260925.md)：当前版本已经安装并完成一次实际调用，但既有新旧对照**没有证明它稳定优于旧版**，完整留出测试未运行。文件齐全、引用链接可打开及一次调用成功，都不替代写作质量验证。
