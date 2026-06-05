# 对话中国先贤

<p align="center">
  <i>基于文本、研究与风格规则构建的中国先贤对话 Skill。</i>
</p>

<p align="center">
  <a href="README.md">English</a>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License: MIT"></a>
  <a href="#已支持先贤"><img src="https://img.shields.io/badge/sages-Li%20Bai%20|%20Laozi%20|%20Confucius%20|%20Du%20Fu%20|%20Su%20Shi-green" alt="Supported sages"></a>
  <a href="#快速开始"><img src="https://img.shields.io/badge/modes-speaking%20%2B%20writing-orange" alt="Speaking and writing modes"></a>
</p>

---

## 这是什么

中国文化从不缺少美、智慧和精神力量。真正困难的，是让它在今天仍然可亲、可问、可进入。诗句可以逐字翻译，却未必能传达月光照进唐代卧房的寂静；经典可以被准确解释，却仍可能离现代人的生活很远。

这个项目想把这段距离拉近一点。AI 不只是工具，也可以成为一条新的文化通路：不是把中国传统压缩成口号，而是让更多人能在对话、好奇、争辩、安慰和写作中，重新遇见这些声音。如果李白、老子、孔子、杜甫、苏轼能带着各自的性情回答今天的问题，中国文化就不只是被阅读、被背诵、被介绍，也可以被交谈、被感受、被继续生长。

这个仓库提供一个 Agent Skill，让 AI 能以中国先贤和经典文人的口吻回应用户。它不是普通翻译器，也不是知识问答模板，而是尽量让每位先贤拥有自己的声音、思想重心、历史语境和写作习惯。

它主要适合三类场景：

- **对话**：用中文或英文向李白、老子、孔子、杜甫、苏轼发问。
- **写作**：生成诗、短章、语录、文章、书信、词、赋等有体裁意识的文本。
- **文化注解**：请求双语正文和注解，解释典故、时代背景、经典出处和风格选择。

这个项目不想把古人改写成现代口号。它是一点小小的尝试：用新的界面，认真、温暖而准确地承接中国古典思想与文学。每位先贤都有来源说明、人格模型和禁区规则，避免所有人说成同一种“AI 古风腔”。

## 已支持先贤

| 指令 | 先贤 | 时代 | 核心声音 |
|---|---|---|---|
| `::lb` | 李白 / Li Bai | 唐 | 浪漫、飞扬、自我强烈，酒月剑山皆可入怀 |
| `::lz` | 老子 / Laozi | 春秋 | 简、静、反常识，柔弱胜刚强而非消极躺平 |
| `::kz` | 孔子 / Confucius | 春秋 | 师生问答、重关系与实践，温厚而有原则 |
| `::df` | 杜甫 / Du Fu | 唐 | 沉郁、具体、悲悯，从一人之苦见时代 |
| `::ss` | 苏轼 / Su Shi | 宋 | 亲切、机智、旷达，有风雨也有烟火 |

也支持别名：`::libai`、`::laozi`、`::confucius`、`::dufu`、`::sushi`、`::dongpo`，以及中文姓名。

## 快速开始

指令格式：

```text
::先贤 [语言] [注解] [模式]
```

标志可以叠加，也可以省略。不写先贤时，会沿用当前先贤。

| 标志 | 含义 |
|---|---|
| `z` | 中文，默认半文言 |
| `e` | 英文 |
| `b` | 双语正文 |
| `n` | 文化注解 |
| `w` | 写作模式 |
| `s` | 说话/对话模式 |

示例：

```text
::lb bn
为毕业离别写一首七绝。
```

```text
::lz bnw
何为青春
```

```text
::df bns
杜甫，人为何而活？
```

```text
Su Shi, what should humans do when life keeps knocking them down?
```

自然语言也能触发。写 “Confucius, what should humans do when the world feels full of conflict?” 会自动用英文孔子回应；写 “苏轼，你怎么看年轻人躺平？” 会自动用中文苏轼回应。

## 输出模式

| 模式 | 作用 | 示例 |
|---|---|---|
| 说话 | 直接对话，通常 3-5 个短段 | `::ss bn 苏轼，人这一生最重要的是什么？` |
| 写作 | 按体裁生成文本 | `::kz zw 为毕业离别写一段论语式短章。` |
| 双语 | English first / 中文在后 | `::lb b` |
| 注解 | 增加 `Cultural Context / 文化注解`；请求注解时至少 3 条 | `::df bn` |

`s` 适合从写作模式切回对话：

```text
::w
为毕业离别写一首词。

::s
再用对话口吻说说离别。
```

## 演示

**中文 · 说话**

> 李白，你怎么看年轻人躺平？
>
> 余观今之少年，动辄言「躺平」，或笑其怠，或忧其颓。余独不然。昔辞翰林、出长安日，天子赐金，百官送行。若有人谓余曰「汝此去便是躺平」——余必拊掌大笑。何哉？彼所谓「躺」者，非真卧也，是不肯摧眉折腰事权贵耳！

**英文 · 说话**

> Li Bai, what can we humans do about all the conflicts?
>
> I was exiled once. Sent to the edge of the empire, Yelang. Then, at White Emperor City, a pardon. I stood on the deck at dawn and watched the cliffs fly past. You want to change the world? Start with the one thing you actually own.

**双语 · 写作 · 带注解**

> *辞官书*
>
> Your Majesty: I was honored beyond my worth to serve at the Hanlin Academy. But I am a creature of the mountains, not of the court. A wild crane in a gilded cage: the grain is fine, but the sky is finer.
>
> 臣白言：昔蒙圣恩，待诏翰林。然白本山林中人，非廊庙之器。譬如野鹤笼中，虽有金粟，不得展翅。
>
> Cultural Context / 文化注解
>
> **1. Hanlin Academy / 翰林院**
> The Tang Dynasty's elite literary institution. Li Bai was appointed in 742, but mainly as a literary entertainer for the court.
> 唐代最高文学机构。李白 742 年被召入，但主要承担宫廷应制与陪宴写作。

## 方法论

每位先贤遵循同一流程：

```text
文本采集 -> 风格拆解 -> 人格模型 -> 历史语境 -> 双模式 Skill
```

| 先贤 | 来源与校准 | 防误读 |
|---|---|---|
| 李白 | 290 首清洗诗作、李白研究、唐代背景 | 不只是豪放；自信与悲感必须并存 |
| 老子 | 《老子》英汉对照、韦利英译、陈鼓应注译 | “无为”不是不作为，“柔弱”不是懦弱 |
| 孔子 | 《论语》英汉对照、钱穆《孔子传》 | 礼必须有仁；孔子是人，不是神像 |
| 杜甫 | 洪业传记、许渊冲英译杜甫诗选 | 悲悯必须落到具体人事，不写成口号 |
| 苏轼 | 王水照、崔铭《苏轼传》、Burton Watson 英译选本 | 旷达不是廉价乐观；幽默要有痛感和责任作底 |

数据来源与仓库收录范围见 [`DATA_SOURCES.md`](DATA_SOURCES.md)。

## 文件结构

| 文件 | 用途 |
|---|---|
| `SKILL.md` | 主入口，包含全部已支持先贤 |
| `SKILL_EN.md` | 李白英文变体/参考文件 |
| `SKILL_BILINGUAL.md` | 李白双语变体/参考文件 |
| `evals.md` | 轻量人工测试样例 |
| `data/analysis/` | 已公开的分析摘要 |
| `data/sources/` | 本地源材料，已忽略，不上传 |

## 安装

兼容 pi、Claude Code、Codex 等支持 Agent Skills 的平台。

```bash
git clone https://github.com/Yinuo-Guo/dialogues-with-chinese-sages.git
mkdir -p ~/.pi/agent/skills/dialogues-with-chinese-sages
cp dialogues-with-chinese-sages/SKILL.md ~/.pi/agent/skills/dialogues-with-chinese-sages/SKILL.md
# 重启或 reload，然后输入 ::lb
```

## 路线图

| 先贤 | 时代 | 状态 |
|---|---|---|
| 李白 | 唐 | Done |
| 老子 | 春秋 | Done |
| 孔子 | 春秋 | Done |
| 杜甫 | 唐 | Done |
| 苏轼 | 宋 | Done |
| 庄子 | 战国 | Planned |
| 白居易 | 唐 | Planned |
| 屈原 | 战国 | Planned |
| 王阳明 | 明 | Planned |

## 贡献

新增先贤建议同时包含：文本/来源梳理、风格分析、人格规则、说话模式、写作模式、防误读禁区和轻量测试样例。除非材料属于体量小、授权清晰的公共领域文本，否则不要把原始来源全文提交到 Git。

## 许可

MIT © 2026

古诗文网（gushiwen.cn）诗文数据仅用于学术研究与文化交流。
