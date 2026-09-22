# management_writing

中英文管理学实证论文写作 Skill。统一叙事与论证方式，而不是只做同义词替换。

## 核心约定

在现有段落内，可以调整措辞、句法、句序与衔接，但保留原主张和引用对应关系。移动、拆分、合并、增删段落或跨段转移内容，必须先提出具体方案，得到用户同意后再执行。研究事实、构念、理论、假设和统计结果不能为改善文风而擅自改变。

写作规范由三篇用户认可范文的精读形成，覆盖标题、摘要、引言、文献、理论与假设、方法、结果、讨论及图表附录。中文是依据共同叙事原则作出的语言适配；这不是另有中文范文验证的宣称。行为测试与用户新稿验收尚未完成。

## 名称与格式

| 用途 | 名称 |
|---|---|
| GitHub 仓库及界面显示 | `management_writing` |
| 标准 Skill 内部标识 | `management-writing` |
| 仓库内技能目录 | `skills/management-writing/` |
| 技能入口 | [`SKILL.md`](skills/management-writing/SKILL.md) |

Agent Skills 标准的 `name` 仅允许小写字母、数字与连字符，且须与技能目录名称相同；仓库名称与显示名称不受这一字段限制。因此保留用户指定的下划线名称，同时用连字符作为内部标识。

## 仓库结构

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
        ├── references/               # 八个分部分参考文件
        ├── assets/                   # 公开书目信息及来源边界索引
        └── tests/scenarios.md        # 待行为验证场景，不是已通过报告
```

进一步了解：[详细说明](skills/management-writing/README.zh-CN.md)。

## 本地使用

本仓库保存独立 Skill，不代表已经安装到 ChatGPT 或 Codex，也不代表已在任何插件市场发布。

Codex 的用户级技能位置是 `$HOME/.agents/skills/`。将整个 `skills/management-writing/` 文件夹复制到该目录，保留全部子目录。已有同名目录时先备份，不要直接覆盖。

安装后的预期位置：

```text
~/.agents/skills/management-writing/SKILL.md
```

Codex CLI/IDE 中可用 `$management-writing` 显式提及；是否成功被当前客户端发现，需要在该客户端实际检查。普通自然语言请求也可说明使用 management_writing。不要仅因在聊天里提到名字就宣称已加载技能。

## 隐私与分发

本仓库是整理后的公开版本，不包含三篇原始 PDF／Word、论文页面截图、大段原文摘录或未确认可公开的稿件内容。保留自行总结的写作方法；已发表文献只保留规范引用、DOI及写法观察，未确认公开材料不披露具体内容。

不新增任何开放许可证；公开可访问不等于取得第三方材料再分发授权。私人参考材料应放在已被 `.gitignore` 排除的 `private-references/` 等目录，不要提交。原附件及本地私人副本不属于本仓库。

公开整理保留核心写作要求和段落结构事前审批规则；仅清理受限制的来源内容及受影响的说明、索引和链接。八份参考文件均保留；T09采用通用冲突情境，不披露私人稿件。`checksums.sha256` 覆盖当前全部公开文件（校验清单自身除外），可在仓库根目录运行 `shasum -a 256 -c checksums.sha256` 核对。

## 格式来源

仅用以下资料核对 Skill 技术格式与本地使用方式；它们不是管理学文风的来源。核对日期：2026-09-22。

- [Agent Skills Specification](https://agentskills.io/specification)
- [OpenAI — Build skills](https://developers.openai.com/codex/skills)

## 当前分发状态

本公开版本供下载和本地使用；客户端安装与行为验收仍需分别进行。发布内容与排除范围见[公开整理记录](PUBLICATION.md)。
