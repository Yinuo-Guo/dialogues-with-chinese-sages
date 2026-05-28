# Dialogues with Chinese Sages

<p align="center">
  <i>The spirit of China's sages, reborn through AI.</i>
</p>

<p align="center">
  <a href="#简体中文">简体中文</a>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License: MIT"></a>
  <a href="#roadmap"><img src="https://img.shields.io/badge/sages-Li%20Bai%20✅%20|%20Confucius%20📋-green" alt="Sages"></a>
</p>

---

## Vision

The hardest part of bringing Chinese culture to the world isn't language—it's context. You can look up every word of a Li Bai poem in a dictionary and still not feel the moonlight falling across a Tang Dynasty bedroom floor. You can memorize the *Analects* cover to cover and never have a real conversation with Confucius.

This project builds a different kind of bridge. Not translation. Not explainers. We make the AI speak, write, and respond *as the sage himself*. Starting with Li Bai—not because he's the greatest, but because he's the most *talkative*. His poems are soaked in "I": I drink, I sing, I laugh, I rage. The perfect first conversation partner for an AI.

## Methodology

Every sage follows the same pipeline. Data-driven, not vibe-driven.

```
Collection → Deconstruction → Personality → Time Travel → Dual-Mode Skill
```

What went into Li Bai:

| Step | Detail |
|---|---|
| Collection | 290 poems scraped from gushiwen.cn, textual variants cleaned |
| Deconstruction | Imagery systems (wine/moon/sword/mountains/water), rhetoric, rhythm, allusion patterns |
| Personality | Six scholarly monographs: Li Changzhi, Yuan Xingpei, Lin Geng, Matsuura Tomohisa, Stephen Owen, Zhou Xunchu |
| Time Travel | Tang Dynasty: food, drink, money, travel, poetry culture, farewell rituals, Daoist practice |
| Dual-Mode Skill | 🗣️ Speaking (semi-classical Chinese, 12 rules) + ✍️ Writing (song-form / quatrain / regulated verse) |

## Demo

**Chinese · Speak**：
> 李白，你怎么看年轻人躺平？
>
> 余观今之少年，动辄言「躺平」，或笑其怠，或忧其颓。余独不然。昔辞翰林、出长安日，天子赐金，百官送行。若有人谓余曰「汝此去便是躺平」——余必拊掌大笑。何哉？彼所谓「躺」者，非真卧也，是不肯摧眉折腰事权贵耳！

**English · Speak**：
> Li Bai, what can we humans do about all the conflicts?
>
> I was exiled once. Sent to the edge of the empire—Yelang. Then, at White Emperor City—a pardon. I stood on the deck at dawn and watched the cliffs fly past. You want to change the world? Start with the one thing you actually own.

**Bilingual · Write · Annotated**：
> *A Letter of Resignation*
>
> Your Majesty: I was honored beyond my worth to serve at the Hanlin Academy. But I am a creature of the mountains, not of the court. A wild crane in a gilded cage—the grain is fine, but the sky is finer.
>
> 臣白言：昔蒙圣恩，待诏翰林。然白本山林中人，非廊庙之器。譬如野鹤笼中，虽有金粟，不得展翅。
>
> ---
> Cultural Context / 文化注解
>
> **1. Hanlin Academy / 翰林院**
> The Tang Dynasty's elite literary institution. Li Bai was appointed in 742—not as an advisor, but as an entertainer composing verses for imperial banquets. He resigned three years later, disillusioned.
> 唐代最高文学机构。李白 742 年被召入，却只是御用文人，负责陪宴赋诗。三年后主动请辞。

## Three Editions

| | File | Audience | Style |
|---|---|---|---|
| 🏮 | `SKILL.md` | Chinese native | Semi-classical Chinese |
| 🌍 | `SKILL_EN.md` | Global English | Poetic English (Xu Yuanchong tradition) |
| 📖 | `SKILL_BILINGUAL.md` | Cross-cultural | English / Chinese body + bilingual context |

## Quick Start

Format: `::sage [lang] [notes] [mode]`. Omit anything you're not changing. `::lb` / `::libai` / `::Li Bai` / `::李白` all work.

| Flag | Meaning |
|---|---|
| `z` | Classical Chinese (default) |
| `e` | English |
| `b` | Bilingual body + bilingual context |
| `n` | Annotated |
| `w` | Writing mode |
| none | Speaking mode (default) |

Start with `::lb`, then stack flags freely: `::e` for English, `::w` to write, `::bn` for bilingual with context. No `::` needed either—natural language auto-detects.

## Installation

Compatible with any platform supporting [Agent Skills](https://agentskills.io): pi, Claude Code, Codex.

```bash
git clone https://github.com/Yinuo-Guo/dialogues-with-chinese-sages.git
cp dialogues-with-chinese-sages/SKILL*.md ~/.pi/agent/skills/celebrity-speak-write/
# Restart or /reload, then type ::lb
```

## Roadmap

We pick sages with global name recognition and ideas that speak directly to modern life.

| Sage | Era | Why them |
|---|---|---|
| Li Bai | Tang | ✅ The ultimate Romantic, face of Chinese poetry worldwide |
| Laozi | Spring & Autumn | 📋 *Tao Te Ching*: the world's most translated book after the Bible. 81 chapters of crisp, AI-friendly dialogue material |
| Confucius | Spring & Autumn | 📋 The most famous Chinese person on earth. The *Analects* is literally a dialogue—made for AI |
| Du Fu | Tang | 📋 Shakespeare + Virgil of China. Li Bai fell from heaven; Du Fu rose from the earth |
| Su Shi | Song | 📋 Poet, painter, cook, engineer, and the wittiest drinking buddy you'll ever have |
| Zhuangzi | Warring States | 📋 The butterfly-dreamer. Camus and Borges were fans |
| Bai Juyi | Tang | 📋 So readable a grandmother could understand. More famous in Japan than in China during the Heian period |
| Qu Yuan | Warring States | 📋 The reason we have dragon boat races. China's first named poet |
| Wang Yangming | Ming | 📋 "Unity of knowledge and action." Silicon Valley's favorite Chinese philosopher right now |

## Contributing

Every new sage follows the same pipeline: Collection → Deconstruction → Personality → Time Travel → Dual-Mode Skill. Check the structure under `01_数据与资料/` to get started. PRs welcome.

## License

MIT © 2026

Poetry data sourced from gushiwen.cn for academic research and cultural exchange purposes only.

---

# 对话中国先贤

<p align="center">
  <i>古典风骨，AI 传承。</i>
</p>

<p align="center">
  <a href="#dialogues-with-chinese-sages">English</a>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License: MIT"></a>
  <a href="#路线图"><img src="https://img.shields.io/badge/sages-Li%20Bai%20✅%20|%20Confucius%20📋-green" alt="Sages"></a>
</p>

---

## 立意

中国文化走向世界，最难跨越的不是语言，是语境。一个外国人读到「床前明月光」，可以查字典，但无法感知月光照进唐代卧房的那种寂静。一个中国学生背下全本《论语》，却很难和孔子真正「对话」一次。

这个项目想做一件事：**让古今之间、中西之间，多一条通路**。不是翻译，不是科普文章，而是让 AI 像一个真实的先贤那样说话、写作、回应你——有脾气、有偏好、有时代烙印。

首期从李白开始——不是因为他最伟大，是因为他最「好聊」。他的诗里全是「我」：我醉、我歌、我笑、我怒。一个把个性写到极致的人，最适合拿来和 AI 碰撞。

## 方法论

每先贤遵循同一套流程。每一步有数据，不靠「感觉像」。

```
诗文采集 → 风格拆解 → 性格建模 → 时代还原 → 双模式 Skill
```

以李白为例：

| 步骤 | 做了什么 |
|---|---|
| 诗文采集 | 古诗文网爬取 290 首全文，清除异文注释 |
| 风格拆解 | 意象体系（酒/月/剑/山/水）、修辞偏好、句式节奏、用典习惯 |
| 性格建模 | 六家权威研究：李长之·袁行霈·林庚·松浦友久·宇文所安·周勋初 |
| 时代还原 | 唐代吃什么、用什么钱、走什么路、怎么写诗、怎么送别、怎么信道 |
| 双模式 Skill | 🗣️ 说话（七分文三分白，12条法则）+ ✍️ 写作（歌行/绝句/律诗） |

## 演示

**中文 · 说话**：
> 李白，你怎么看年轻人躺平？
>
> 余观今之少年，动辄言「躺平」，或笑其怠，或忧其颓。余独不然。昔辞翰林、出长安日，天子赐金，百官送行。若有人谓余曰「汝此去便是躺平」——余必拊掌大笑。何哉？彼所谓「躺」者，非真卧也，是不肯摧眉折腰事权贵耳！

**英文 · 说话**：
> Li Bai, what can we humans do about all the conflicts?
>
> I was exiled once. Sent to the edge of the empire—Yelang. Then, at White Emperor City—a pardon. I stood on the deck at dawn and watched the cliffs fly past. You want to change the world? Start with the one thing you actually own.

**双语 · 写作 · 带注解**：
> *辞官书*
>
> 臣白言：昔蒙圣恩，待诏翰林。然白本山林中人，非廊庙之器。譬如野鹤笼中，虽有金粟，不得展翅。
>
> Your Majesty: I was honored beyond my worth to serve at the Hanlin Academy. But I am a creature of the mountains, not of the court. A wild crane in a gilded cage—the grain is fine, but the sky is finer.
>
> ---
> 文化注解 / Cultural Context
>
> **1. 翰林院 / Hanlin Academy**
> 唐代最高文学机构。李白 742 年被召入，却只是御用文人，负责陪宴赋诗。三年后主动请辞。
> The Tang Dynasty's elite literary institution. Li Bai was appointed in 742—not as an advisor, but as an entertainer composing verses for imperial banquets. He resigned three years later, disillusioned.

## 三语三档

| | 文件 | 受众 | 特色 |
|---|---|---|---|
| 🏮 | `SKILL.md` | 中文母语者 | 七分文三分白 |
| 🌍 | `SKILL_EN.md` | 全球英语用户 | 许渊冲传统诗意英文 |
| 📖 | `SKILL_BILINGUAL.md` | 跨文化场景 | English / 中文正文 + 双语注解 |

## 快速开始

指令格式：`::先贤 [语言] [注解] [模式]`。「李白」四种写法等效：`::lb` / `::libai` / `::Li Bai` / `::李白`。

| 标志 | 含义 |
|---|---|
| `z` | 中文半文言（默认） |
| `e` | 英文 |
| `b` | 双语正文 + 双语注解 |
| `n` | 带注解 |
| `w` | 写作模式 |
| 无 | 说话模式（默认） |

首次 `::lb` 开始中文对话，之后随便叠加：`::e` 切英文，`::w` 切写作，`::bn` 双语带注解——每次只写要改的标志即可，不用重复 lb。不写 `::` 也行，自然语言自动识别。

## 安装

兼容 pi、Claude Code、Codex 等支持 [Agent Skills](https://agentskills.io) 标准的工具。

```bash
git clone https://github.com/Yinuo-Guo/dialogues-with-chinese-sages.git
cp dialogues-with-chinese-sages/SKILL*.md ~/.pi/agent/skills/celebrity-speak-write/
# 重启或 /reload，输入 ::lb
```

## 路线图

从全球知名度和文化代表性两个维度选人。

| 先贤 | 时代 | 备注 |
|---|---|---|
| 李白 | 唐 | ✅ 浪漫主义的终极代言人 |
| 老子 | 春秋 | 📋 《道德经》全球销量仅次于《圣经》，81章短句完美适配 AI |
| 孔子 | 春秋 | 📋 全世界最著名的中国人，《论语》通篇对话体 |
| 杜甫 | 唐 | 📋 李白是天上来的，杜甫是人间的 |
| 苏轼 | 宋 | 📋 写诗做饭搞水利都会，跟他聊天肯定不无聊 |
| 庄子 | 战国 | 📋 做梦变蝴蝶那位，存在主义哲学家最爱引用的中国人 |
| 白居易 | 唐 | 📋 诗在日本比在中国还火，平安时代文人必读 |
| 屈原 | 战国 | 📋 端午节因他而来，中国第一位署名诗人 |
| 王阳明 | 明 | 📋 「知行合一」，硅谷创业圈也在读 |

## 贡献

每个新先贤遵循同一套流程：诗文采集 → 风格拆解 → 性格建模 → 时代还原 → 双模式 SKILL。参考 `01_数据与资料/` 结构即可上手。欢迎 PR。

## 许可

MIT © 2026

诗文数据来源于古诗文网（gushiwen.cn），仅供学术研究与文化交流使用。
