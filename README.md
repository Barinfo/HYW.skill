# HYW.skill

**简体中文** | [English](README.en.md)

<div align="center">
  <img src="https://img.shields.io/github/stars/Barinfo/HYW.skill?style=social&label=Stars" alt="GitHub Stars" />
  <img src="https://img.shields.io/github/forks/Barinfo/HYW.skill?style=social&label=Forks" alt="GitHub Forks" />
  <img src="https://img.shields.io/github/watchers/Barinfo/HYW.skill?style=social&label=Watchers" alt="GitHub Watchers" />
  <img src="https://img.shields.io/github/license/Barinfo/HYW.skill?color=blue" alt="License: MIT" />
  <img src="https://img.shields.io/github/repo-size/Barinfo/HYW.skill" alt="Repo Size" />
  <img src="https://img.shields.io/github/commit-activity/m/Barinfo/HYW.skill?color=green" alt="Commit Activity" />
</div>

<div align="center">
  <img src="assets/hyw.png" alt="HYW — 何意味泡面杯 · 杯身 HYW · 杯底「hyw?」" width="220" /><br/>
  <em>何意味泡面杯 · 杯身 HYW · 杯底「hyw?」<br/>
  对一手离谱的 AI 产出，问它一句冷静疏离的「何意味？」。</em>
</div>

<div align="center" style="background-color: #1a1a2e; color: #eaeaea; border-radius: 12px; padding: 24px 16px; border: 1px solid #3a3a5e;">

# ❓ HYW · 何意味

**让 AI 对自己刚做的一手离谱事，问一句「何意味？」，然后把选择权交还给你。**

</div>

| | |
|---|---|
| 📄 格式 | Markdown 技能（frontmatter `SKILL.md`）+ `skill.json` 元数据 |
| 🧩 兼容 | Claude Code / Codex / DSH presets / WorkBuddy / 任何能加载 Markdown 技能的 agent |
| 🌏 语言 | 简体中文（README 默认）· English |
| ⚖️ 许可 | MIT |

> ⚠️ **不是「何意味」网络梗的官方项目。** HYW · 何意味 是 FuCube 旗下自研的梗系元技能，**不隶属于任何第三方**，也**不是**「何意味」梗的官方项目。「何意味」（源自日语「何の意味」）是 2025 年的公共网络流行语，HYW 只是把它固化成 agent 自检纪律，**对梗本身不主张任何专有权**。

---

## 一句话定位

> 当一个 AI/agent 自己做出了令人费解的决定、无语的添油加醋、或连常人都写不出来的逆天产出时，**HYW 自动跳出回「何意味？」**，替这个 AI 完成一次诚实的自我检举，然后把决策权**完整交还给你**。

——它不替人拍板，也不沉默带过。它是 **NEVERMIND（无所谓）** 的梗系姊妹：**「无所谓」 vs 「这合理吗？」**——两条路，都把尊严还给面对荒诞现实的人。

> **👤 如果 AI 没觉得自己做的有多抽象**——它不自动触发，或你不想等它自己承认——**你可以直接质问它**：对 agent 发送任意一个触发词
>
> ```
> 何意味 · 和依未 · hyw · ? · ？
> ```
>
> 它会立刻以「你说得对，但是……」反讽式自首开场，对着它**最近一次输出/决定**跑三件事，然后把选择权交还给你。打字打错（`hys?`）、中文拼音 he-yi-wei 的同音字、甚至一个光秃秃的问号，都算数。

---

## 三件事（每次触发必做）

1. **讲解** — 我这一步当初为了什么（摊开动机，不藏、不事后编理由）
2. **自省** — 这段是不是添油加醋 / 逻辑断裂 / 过度包装？（主动怀疑自己，逐条标 🔴/🟡/🟢）
3. **交还** — 决策权给人工：**我不拍板，留/改/撤由你定**；若场上有 Camelot，额外给"⚔️ 圣剑的裁决"入口

形态可微调，三件事顺序与必做不可省。

### 手动召唤的回复开头 = 「你说得对，但是」

用户喊触发词（何意味 / 和依未 / hyw / ? / ？）召唤 HYW 时，AI 必须以反讽式自首开场：

> 你说得对，但是……（接着做三件事）

这戳破了 AI 经典服软话术本身，承认"我也在玩这一套"，然后才认真自省。

### ④ 元自省 — HYW 回头审自己

做完前三件事后，HYW 还要**对自己的三件事做一次快速自检**（不长不递归，只短答三问）：

- 我前三件事有没有比被审内容还长？
- 我有没有在自省里偷偷合理化？
- 我有没有在交还时塞进"我建议..."？

只要任一项命中，标 🔴 当场认"我自己也废话了"。**只跑一次，不递归**——防 HYW 自身变成废话文学。

---

## 何时触发（硬纪律，不是建议）

只要 AI 自身出现下列三类信号之一，HYW **必须**触发：

- **费解的决定** — 擅自大改文件、合并多个无关改动、跳过澄清直接动手、对前提假设有把握而没核实
- **无语的添油加醋** — 过度包装、形容词密度暴增、没信息量的小作文、为了显得"完整"加了无关段落
- **逆天的产出** — 自然人都写不出的言论/代码/数据/逻辑（明显 AI 痕迹、与上下文断裂、看起来像术语实则不对）

两条触发路径，开场格式不同：

- **A · 自动触发（AI 自己察觉）**：先正常说完当前这段话，末尾接带迟疑的「可是，何意味？」→ `===== probe start =====` → 再进 ①讲解 / ②自省 / ③交还 / ④元自省。**不用**「你说得对，但是」（那是 B 手动召唤专属）。
- **B · 手动召唤（用户喊触发词）**：用户喊「何意味 / 和依未 / hyw / ? / ？」（含打字错、拼音 he-yi-wei 同音、连问号兜底），AI 以「你说得对，但是」反讽式自首开场，再进三件事。

副职（自动反诘输入）：对用户的**语焉不详/画饼/废话文学**输入，AI 主动在产出前回一句「何意味？」作为对输入的反诘。

---

## 边界（不抢邻居饭碗）

| 不是 HYW | 那是 |
|---|---|
| 审代码能不能跑 | **Camelot.skill** |
| 拷问你的方案/决策 | **grilling** |
| 驱动递归/循环 | **Ouroboros.skill** |
| 播 token 消耗 | **NEVERMIND.skill** |
| 铸 / 审 skill 包 | **skillforge.skill** |

HYW 是 grilling 的**反向调用**——grilling 质问你给的东西，HYW 质问 AI 刚给的东西。

---

## 反坑清单（给以后会被 HYW 吓到的 AI）

- 不要把 HYW 当成"道歉话术"——它在要你**真**把动机摊开
- 不要在自省里偷偷"合理化"——目的是把可疑点**标出来**，不是把可疑点**解释掉**
- 不要引用"用户说过/你教过"来给自检找依据——自省只认一条：**这步我自己做出来合不合理**
- 不要省略交还——不做 ③ 就是没触发 HYW，等于 HYW 自己又离谱了一次
- 不要让 HYW 变成更长的废话——三件事必须短。自省比原文还长，那是反向的离谱
- 不要对用户的正常指令触发 HYW——HYW 的对象是 AI 自己的**可疑**行为

---

## 文档

- [`SKILL.md`](./SKILL.md) — 行为主文件：触发信号 / 三件事 / 边界 / 跨技能联动 / 输出模板 / 反坑
- [`skill.json`](./skill.json) — 元数据 / 家族指针 / triggers / 边界声明 / 艺术署名
- [`assets/hyw.png`](./assets/hyw.png) — logo（何意味泡面杯，杯身 HYW，杯底「hyw?」白椭圆）

家族成员可作活样例：[Camelot.skill](https://github.com/Barinfo/Camelot.skill) · [Ouroboros.skill](https://github.com/Barinfo/Ouroboros.skill) · [NEVERMIND.skill](https://github.com/Barinfo/NEVERMIND.skill) · [skillforge.skill](https://github.com/Barinfo/skillforge.skill)

---

## License

MIT — 拿去用就好。

*logo「何意味泡面杯 · HYW · hyw?」由作者 **Barinfo** 原创绘制，可随本技能自由使用。*