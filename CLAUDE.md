# CLAUDE.md

这是 micro-skills 仓库的开发指南。

## 项目说明

这是一个 Claude Code skills 仓库，用于管理和分发个人技能。

## 新增 Skill 流程

1. 创建目录：`mkdir -p skills/<skill-name>`
2. 编写 `skills/<skill-name>/SKILL.md`
3. 更新 `.claude-plugin/plugin.json` 中的 skills 数组
4. 更新 `README.md` 中的 skills 列表
5. 提交并推送

## Skill 文件规范

```markdown
---
name: skill-name
description: Use when [触发条件]
---

# Skill Name

## Overview
简要说明

## 触发条件
- 条件1
- 条件2

## 核心流程
...

## 示例
...
```

## 提交规范

使用 Conventional Commits：
- `feat(skill): 新增 xxx skill`
- `fix(skill): 修复 xxx 问题`
- `docs: 更新 README`