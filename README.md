# Will-Leonardo Skills

个人 AI skills 集合仓库，用于沉淀可复用的学习、工作、代码协作和知识管理规则。

## Skills 目录

本仓库优先解决“有哪些可用 skill、什么时候该用、如何触发、具体怎么用”的发现问题。未来新增 skill 时，请同步更新下表。

| Skill | 能力说明 | 适用场景 | 触发关键词 | 具体使用 |
| --- | --- | --- | --- | --- |
| [`learning-coach`](./skills/learning-coach/SKILL.md) | 通用型温和学习教练。帮助用户从模糊方向开始澄清目标，制定个性化学习计划，通过解释、提问、练习、主动回忆和间隔复习陪伴学习，并记录学习进度。 | 学习任何领域；不知道该如何开始；需要学习路线图；需要复习旧知识；希望像老师一样一边聊天一边学习。 | `学习计划`、`我想学...`、`不知道怎么学`、`复习`、`考考我`、`费曼学习法`、`主动回忆`、`spaced review` | 在 Codex 中使用 `$learning-coach`，例如：`Use $learning-coach 帮我学习 AI，我现在只有一个模糊方向。` |

## Skill 结构约定

每个 skill 独立放在 `skills/<skill-name>/` 下，至少包含：

```text
skills/<skill-name>/
  SKILL.md
```

推荐包含 UI 元数据：

```text
skills/<skill-name>/
  agents/
    openai.yaml
```

## 维护规则

- 新增 skill 后，更新上方表格。
- Skill 名称尽量短、清晰、好记，使用小写 kebab-case。
- `SKILL.md` 只保留 agent 执行任务需要的核心规则，不放冗余说明。
- 如果 skill 需要记录、模板或脚本，再按需添加 `references/`、`assets/` 或 `scripts/`。
