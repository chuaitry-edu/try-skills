# 安装指南

## 一键安装

```bash
bash <(curl -s https://raw.githubusercontent.com/chuaitry-edu/try-skills/main/scripts/install.sh)
```

脚本会自动检测你使用的 agent 并将 skill 安装到对应目录。

## 手动安装

### Hermes Agent
```bash
cp -r hermes/* ~/AppData/Local/hermes/skills/
```

### Claude Code
```bash
cp claude-code/*.md .claude/skills/
```

### Codex CLI
```bash
cp codex/*.md .agents/skills/
```

### Cursor
```bash
cp cursor/*.mdc .cursor/rules/
```

## 验证安装

安装后，对你的 AI 说：

```
「帮我看看我的学习问题」
```

如果能正常响应，说明安装成功。
