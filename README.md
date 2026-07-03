# try-skills 🧪

初爱try 的学习工具箱。一套帮助诊断学习问题的 AI agent skill 体系。

## 这是什么

5 个 skill，覆盖一个学习目标的完整生命周期：

```
目标 → 定难度 → 配学法 → 排任务 → 搞巩固
```

| skill | 解决的问题 | 一句话 |
|-------|-----------|--------|
| **try-plan** | 这个目标要多久？可行吗？ | 5 个阶段 + 时间估算 + 可行性判断 |
| **try-stretch** | 太简单了提不起劲 / 太难了想放弃 | 找到舒适区与恐慌区之间的拉伸区 |
| **try-method** | 不知道该怎么学 | 判断知识/技能/行为/感受类型，匹配对应学法 |
| **try-task** | 有目标但不知道今天做什么 | 把大目标分解成今天唯一要做的事 |
| **try-review** | 学完就忘了 | 主动回忆+间隔重复+复盘策略 |

## 怎么用（选你的 agent）

```
hermes/          ← 用于 Hermes Agent
├── try-plan/SKILL.md
├── try-stretch/SKILL.md
├── try-method/SKILL.md
├── try-task/SKILL.md
└── try-review/SKILL.md

claude-code/     ← 用于 Claude Code
├── try-plan.md
├── try-stretch.md
├── try-method.md
├── try-task.md
└── try-review.md

codex/           ← 用于 Codex CLI
├── try-plan.md
├── try-stretch.md
├── try-method.md
├── try-task.md
└── try-review.md

cursor/          ← 用于 Cursor
├── try-plan.mdc
├── try-stretch.mdc
├── try-method.mdc
├── try-task.mdc
└── try-review.mdc
```

### Hermes 用户
每个 skill 通过触发词调用：

```
/try-plan       → 目标可行性检查
/try-stretch    → 难度定位
/try-method     → 学法匹配
/try-task       → 任务分解
/try-review     → 复习方案
```

### Claude Code / Codex / Cursor 用户
把对应目录下的 `.md` / `.mdc` 文件放到你的 agent 配置目录即可。内容结构与 Hermes 版一致。

## 设计原则

- **一个工具只做一件事** — 每个 skill 只诊断一个问题
- **给唯一动作** — 不给「三种选择」，只给下一步
- **不假装科学** — 背后有认知科学依据，但不说术语
- **不做学习规划师** — 定位、匹配、分解、巩固，不规划长期路径

## 如何贡献

欢迎提 Issue 和 Pull Request。

流程：
1. 提 Issue 描述你想改什么
2. Fork 这个仓库
3. 改对应的 skill 文件（4 个 agent 目录下的都要改）
4. 提 PR，我看了会合

> 注意：hermes/ 下的 SKILL.md 是主版本。其他 3 个目录是它的副本，改的时候保持同步。

## 背景

作者 [@初爱try](https://github.com/czz09)，一个用第一人称实验做学习行为研究的 25 岁内容创作者。

这些 skill 是为自己的内容创作体系 `try-` 而建，也公开供其他人使用。

## License

MIT
