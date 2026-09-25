# ks-100 · 满血执行标准 🔋

> *Full-power execution standard for AI coding agents: recon → fan-out → verify → close.*

你有没有遇到过这种事：让 AI 做一件复杂的活，它三分钟交了一份「看起来什么都有」的东西，你一细看，最难的那 30% 全靠一句「建议后续验证」糊过去了。

不是它不会。是你没告诉它这次要**满血**。

## 🎯 这个 skill 做什么

一句 `$ks-100`，把助手切进另一种工作模式：

- 🔍 **先侦察再动手** —— 先把事实底座、边界、work list 列清楚，不带着模糊假设开跑
- 🚀 **把并发槽占满** —— 能拆的维度全部派 agent 并行，每个 agent 边界清晰、可独立验收，只留一个人写共享文件
- 🧐 **载重结论亲自复核** —— 最反直觉、影响最大、agent 之间打架的结论，主线程回到原始证据自己再查一遍
- 📏 **按任务类型设验收线** —— 研究要交叉信源，代码要行为级测试，迁移要备份 + 回滚 + 冒烟
- 🧾 **交付前逐项补漏** —— 对着 work list 一条条标：完成 / 不适用 / 阻塞 / 需你授权。**不许用模糊措辞假装完成**
- ⚖️ **客观优先** —— 证据不够就写「无法证实」，不为了显得完整而编

## 💬 你说什么，它给什么

你说：「$ks-100 把这个仓库的安全隐患全部查一遍」

它不会回你一段泛泛的清单。它会先扫结构、定范围，派 6～8 个 agent 分别盯凭据、依赖、注入面、权限、配置、CI；然后自己去核最吓人的那两条是不是真的；最后交一份「查了什么 / 没查什么 / 为什么没查」都写清楚的报告。

## 📖 它从哪来

从一台真实机器上几十次「地毯式」任务里蒸馏出来的纪律——包括一次 130+ agent 的资产盘点、一次挖矿木马的取证清除、若干次对网络宣称的深度核查。每条规则背后都有一次「差点漏掉」。

## 🧩 和谁搭配

- 派活防冲突：[ks-agent-team-collaboration](https://github.com/KaiSky0823/ks-agent-team-collaboration)
- 收活防糊弄：[ks-agent-team-review](https://github.com/KaiSky0823/ks-agent-team-review)

## ⚙️ 安装

```bash
# Claude Code
git clone https://github.com/KaiSky0823/ks-100.git ~/.claude/skills/ks-100
# Codex
git clone https://github.com/KaiSky0823/ks-100.git ~/.agents/skills/ks-100
```

然后在任何复杂任务前面加一句 `$ks-100`。日常小事别用，它真的会把并发槽全占了。

## License

MIT © 2026 KaiSky0823
