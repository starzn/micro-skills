# micro-skills

个人技能库，包含一系列提升开发效率的 Claude Code skills。

## 安装

### Claude Code

**第一步：注册 marketplace**

```bash
/plugin marketplace add starzn/micro-skills
```

**第二步：安装插件**

```bash
/plugin install micro-skills
```

### 更新

```bash
/plugin update micro-skills
```

## Skills 列表

| Skill | 描述 |
|-------|------|
| [git-commit](./skills/git-commit) | 自动分析代码变更并生成符合项目规范的 commit message |

## 使用方式

安装后，skills 会自动根据触发条件激活。也可以手动调用：

```
/git-commit
```

## 开发

### 目录结构

```
micro-skills/
├── .claude-plugin/
│   └── plugin.json      # 插件配置
├── skills/
│   └── git-commit/
│       └── SKILL.md     # Skill 定义
├── README.md
└── CLAUDE.md            # 本仓库的开发指南
```

### 新增 Skill

1. 在 `skills/` 下创建新目录：`mkdir -p skills/<skill-name>`
2. 创建 `SKILL.md` 文件，包含 YAML frontmatter 和 skill 内容
3. 更新 `plugin.json` 中的 skills 列表
4. 更新 README.md

### Skill 命名规范

- 使用小写字母和连字符：`git-commit`、`code-review`
- 动词优先：`creating-*`、`using-*`、`writing-*`
- 描述性：名称应表达 skill 的核心功能

## License

MIT