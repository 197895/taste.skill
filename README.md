<div align="center">

# 🔪 taste.skill（科研审美.skill）

### “当一个思想真正变得”优美”时，它往往已经经过了反复的打磨与精简，并以最优雅的形式呈现出来。”

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python 3.9+](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://python.org)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-green)](https://agentskills.io)
[![Stars](https://img.shields.io/github/stars/197895/taste.skill?style=social)](https://github.com/197895/taste.skill/stargazers)

[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-blueviolet)](https://docs.anthropic.com/en/docs/claude-code)
[![Hermes](https://img.shields.io/badge/Hermes-Skill-orange)](https://hermes-agent.nousresearch.com/)
[![OpenClaw](https://img.shields.io/badge/OpenClaw-Skill-teal)](https://docs.openclaw.ai/)
[![Codex](https://img.shields.io/badge/Codex-Skill-black)](https://developers.openai.com/codex)


</div>

---

🧑‍🔬 你每天刷 arXiv，被铺天盖地的 “novel / efficient / SOTA” 吓哭了？

📈 你不想看作者机构、会议 title、只想知道：这份工作是否足够优雅？对培养我的论文审美是否有帮助？

🧨 你受够了换壳迁移、小修小补、调参 trick、工程 patch stack，却还被包装成“重大创新”？

🧠 你需要一个真正有 taste 的论文筛选器！培养论文审美，从用批判的眼光看论文开始。**该留就留，该 ban 就 ban。**

### ✨ 一切尽在 taste.skill。

`taste.skill` 不是论文总结器。

它是一个 **严格科研审美评估器**。

它会帮你判断一篇论文：

* 是不是只是已有方法换壳；
* 是不是只在弱 baseline 上赢；
* 是不是靠调度 trick 和工程 patch 堆出来；
* 是不是有真正的新抽象；
* 是不是值得复现、跟进、作为 baseline；
* 是不是应该直接 ban。

---

## 🧬 taste.skill 是什么？

一句话：

> **一个专门筛选高质量、有品位的论文的 AI Skill。**

输入：

* arXiv 链接；
* 论文标题；
* PDF；
* abstract / method / experiment 摘要；
* 或者你丢给 agent 的任意论文材料。

输出：

* Keep / Borderline / Ban；
* A / A- / B+ / B / B- / C 评级；
* 核心方法拆解；
* related work 对比；
* 方法新意判断；
* 实验硬度评估；
* baseline 公平性检查；
* trick 和核心创新分离；
* 影响力潜力判断。

---


## ⚡ 安装

```text
帮我安装 taste.skill 这个 skill：https://github.com/197895/taste.skill
```
Agent 应该自动识别当前宿主的 skills 目录，完成安装和入口加载。


#### Hermes
```bash
hermes skills install 197895/taste.skill/skills/taste
```

#### OpenClaw
```bash
clawhub install taste-paper
```

---

## 🚀 使用

直接说：

```text
用 taste.skill 看这篇 paper.
```

---

## 🔍 它会怎么搜？

taste.skill 不会只看论文自己的 related work。

它会主动查：

1. 论文标题；
2. 核心方法关键词；
3. 最接近 baseline；
4. 同路线 SOTA；
5. 相邻路线；
6. 同期工作；
7. 后续工作；
8. GitHub 实现；
9. benchmark 结果；
10. 是否已有工业或开源系统采用。

搜索目的不是找引用数，而是判断：

* 是不是换壳；
* 是不是漏掉关键前作；
* 是不是 baseline 太弱；
* 是不是已经被后续工作绕开；
* 是不是只在作者自己的设定里强。

---

## 🧭 适合谁用？

* 每天刷 arXiv 的研究生；
* 想快速筛方向的本科生；
* 组会前临时判断论文价值的人；
* 做 AI infra / LLM serving / video generation / world model 的研究者；
* 不想被 SOTA 表格骗的人；
* 想训练自己论文审美的人；
* 想知道“这篇到底值不值得追”的人。

---

## 🧨 不适合谁用？

* 想要温和总结的人；
* 想让 AI 帮论文找优点的人；
* 想给投稿论文润色的人；
* 只关心会议等级的人；
* 接受不了论文被直接 ban 的人。

---


## 🧩 原理

具体评估原则、打分标准、ban 规则、搜索流程和输出格式都写在 skill 本体里：

[查看 taste.skill 的完整规则](skills/taste/SKILL.md)

---



## 🤝 贡献

欢迎提交：

* 新领域 rubric；
* 典型论文案例；
* 被误判的反例；
* 更严格的 ban 规则；
* baseline 公平性检查模板；
* 不同方向的 paper triage workflow。

你也可以直接开 issue：

```text
这篇你评错了，为什么？
```

taste.skill 会把纠正沉淀进审美规则。

---
