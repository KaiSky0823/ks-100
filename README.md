# ks-100

**满血执行标准**：复杂任务的侦察、并行、独立复核与验收纪律。

## 安装

本仓库根目录即技能目录。任选当前使用的宿主安装：

```bash
# Claude Code
git clone https://github.com/KaiSky0823/ks-100.git ~/.claude/skills/ks-100

# Codex
git clone https://github.com/KaiSky0823/ks-100.git ~/.agents/skills/ks-100
```

目标目录已存在时，在该目录检查改动后更新，避免覆盖本地修改。

## 使用

Claude Code 使用 `/ks-100`；Codex 使用 `$ks-100`，并附上具体任务、材料与约束。自动发现取决于宿主设置。工作流正文见 [SKILL.md](SKILL.md)。

## 运行要求

需要当前宿主提供文件读取与任务所需工具。涉及事实、行情或外部资料时需要网络检索；多 agent 流程依赖当前宿主提供的协作能力。工具缺失时应明确报告，不能虚构调用或结果。
