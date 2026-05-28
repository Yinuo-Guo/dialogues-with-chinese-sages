# Dialogues with Chinese Sages / 对话中国先贤

<p align="center">
  <a href="#dialogues-with-chinese-sages--对话中国先贤">English</a> | <a href="#dialogues-with-chinese-sages--对话中国先贤-1">简体中文</a>
</p>

<p align="center">
  <i>古典风骨，AI 传承。</i>
  <br>
  <i>The spirit of China's sages, reborn through AI.</i>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License: MIT"></a>
  <a href="#路线图--roadmap"><img src="https://img.shields.io/badge/sages-Li%20Bai%20✅%20|%20Confucius%20🚧-green" alt="Sages"></a>
</p>

---

## 立意 / Vision

中国文化走向世界，最难跨越的不是语言，是语境。一个外国人读到「床前明月光」，可以查字典，但无法感知月光照进唐代卧房的那种寂静。一个中国学生背下全本《论语》，却很难和孔子真正「对话」一次。

这个项目想做一件事：**让古今之间、中西之间，多一条通路**。不是翻译，不是科普文章，而是让 AI 像一个真实的先贤那样说话、写作、回应你——有脾气、有偏好、有时代烙印。

首期从李白开始——不是因为他最伟大，是因为他最「好聊」。他的诗里全是「我」：我醉、我歌、我笑、我怒。一个把个性写到极致的人，最适合拿来和 AI 碰撞。

This project builds a different kind of bridge. Not translation. Not explainers. We make the AI speak, write, and respond *as the sage himself*—with personality, temperament, and the imprint of his time.

Starting with Li Bai—not because he's the greatest, but because he's the most *talkative*. His poems are soaked in "I": I drink, I sing, I laugh, I rage. A man who turned his personality up to eleven is the perfect first conversation partner for an AI.

---

## 方法论 / Methodology

每先贤遵循同一套流程。每一步有数据，不靠「感觉像」。 / Every sage follows the same pipeline. Data-driven, not vibe-driven.

```
诗文采集 → 风格拆解 → 性格建模 → 时代还原 → 双模式 Skill
Collection → Deconstruction → Personality → Time Travel → Dual-Mode Skill
```

以李白为例 / What went into Li Bai:

| 步骤 / Step | 做了什么 / What we did |
|---|---|
| 诗文采集 / Collection | 古诗文网爬取 290 首全文，清除异文注释 — 290 poems, cleaned of textual variants |
| 风格拆解 / Deconstruction | 意象体系（酒/月/剑/山/水）、修辞偏好、句式节奏、用典习惯 — Imagery systems, rhetoric, rhythm, allusion patterns |
| 性格建模 / Personality | 六家权威研究：李长之·袁行霈·林庚·松浦友久·宇文所安·周勋初 — Six scholarly monographs |
| 时代还原 / Time Travel | 唐代吃什么、用什么钱、走什么路、怎么写诗、怎么送别、怎么信道 — Tang Dynasty food, money, travel, poetry culture, farewell rituals, Daoist practice |
| 双模式 Skill / Dual-Mode | 🗣️ 说话（七分文三分白，12条法则）+ ✍️ 写作（歌行/绝句/律诗）— Speaking mode (semi-classical Chinese, 12 rules) + Writing mode |

---

## 演示 / Demo

**中文 · 说话** / Chinese · Speak：
> 李白，你怎么看年轻人躺平？
>
> 余观今之少年，动辄言「躺平」，或笑其怠，或忧其颓。余独不然。昔辞翰林、出长安日，天子赐金，百官送行。若有人谓余曰「汝此去便是躺平」——余必拊掌大笑。何哉？彼所谓「躺」者，非真卧也，是不肯摧眉折腰事权贵耳！

**英文 · 说话** / English · Speak：
> Li Bai, what can we humans do about all the conflicts?
>
> I was exiled once. Sent to the edge of the empire—Yelang. Then, at White Emperor City—a pardon. I stood on the deck at dawn and watched the cliffs fly past. You want to change the world? Start with the one thing you actually own.

**双语 · 写作（带注解）** / Bilingual · Write · Annotated：
> *A Letter of Resignation / 辞官书*
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
> 唐代最高文学机构。李白 742 年被召入，却只是御用文人，负责陪宴赋诗。三年后主动请辞——所谓「赐金放还」，体面背后是理想的幻灭。

---

## 三语三档 / Three Editions

| | 文件 / File | 受众 / Audience | 特色 / Style |
|---|---|---|---|
| 🏮 | `SKILL.md` | 中文母语者 / Chinese native | 七分文三分白 / Semi-classical Chinese |
| 🌍 | `SKILL_EN.md` | 全球英语用户 / Global English | 许渊冲传统诗意英文 / Poetic English |
| 📖 | `SKILL_BILINGUAL.md` | 跨文化 / Cross-cultural | English / 中文正文 + 双语注解 |

---

## 快速开始 / Quick Start

指令格式：`::先贤 [语言] [注解] [模式]`，按此顺序，可省略前面的、只写要改的。

Format: `::sage [lang] [notes] [mode]`. Omit anything you're not changing.

| 标志 / Flag | 含义 / Meaning |
|---|---|
| `z` | 中文半文言（默认）/ Classical Chinese (default) |
| `e` | 英文 / English |
| `b` | 双语正文 + 双语注解 / Bilingual body + bilingual notes |
| `n` | 带注解 / Annotated |
| `w` | 写作模式 / Writing mode |
| 无 / none | 说话模式（默认）/ Speaking mode (default) |

首次 `::lb` 开始中文对话（`::libai`、`::Li Bai`、`::李白` 均可），之后随便叠加：`::e` 切英文，`::w` 切写作，`::bn` 双语带注解——每次只写要改的标志即可，不用重复 lb。不写 `::` 也行，自然语言自动识别。

Start with `::lb` for Chinese chat (`::libai`, `::Li Bai`, `::李白` all work), then stack flags freely: `::e` for English, `::w` to write, `::bn` for bilingual with notes. Just write the flags you're changing—no need to repeat `lb`. No `::` needed either—natural language auto-detects.

---

## 安装 / Installation

兼容 pi、Claude Code、Codex 等支持 [Agent Skills](https://agentskills.io) 标准的工具。

```bash
git clone https://github.com/YOUR_USERNAME/dialogues-with-chinese-sages.git
cp dialogues-with-chinese-sages/SKILL*.md ~/.pi/agent/skills/celebrity-speak-write/
# 重启或 /reload，输入 ::lb
```

---

## 路线图 / Roadmap

从全球知名度和文化代表性两个维度选人。原则：这个人离开中国语境，外国人听说过吗？他的思想或作品能直接跟现代人对话吗？

We pick sages with global name recognition and ideas that speak directly to modern life—no prior Sinology degree required.

| 先贤 / Sage | 时代 | 备注 / Why them |
|---|---|---|
| 李白 / Li Bai | 唐 | ✅ 诗仙 — 浪漫主义的终极代言人 / The ultimate Romantic, face of Chinese poetry worldwide |
| 老子 / Laozi | 春秋 | 📋 《道德经》全球销量仅次于《圣经》 — 81章，完美适配 AI 短对话 / Tao Te Ching: the world's most translated book after the Bible. 81 chapters of crisp, AI-friendly dialogue material |
| 孔子 / Confucius | 春秋 | 🚧 全世界最著名的中国人 — 《论语》通篇对话体，天生就该是 AI / The most famous Chinese person on earth. The Analects is literally a dialogue—made for AI |
| 杜甫 / Du Fu | 唐 | 📋 诗圣 — 李白是天上来的，杜甫是人间的 / Shakespeare + Virgil of China. Li Bai fell from heaven; Du Fu rose from the earth |
| 苏轼 / Su Shi | 宋 | 📋 千古第一全才 — 写诗做饭搞水利都会，跟他聊天肯定不无聊 / Poet, painter, cook, engineer, and the wittiest drinking buddy you'll ever have |
| 庄子 / Zhuangzi | 战国 | 📋 做梦变蝴蝶那位 — 西方存在主义哲学家最爱引用的中国思想家 / The butterfly-dreamer. Camus and Borges were fans |
| 白居易 / Bai Juyi | 唐 | 📋 「老妪能解」 — 诗在日本比在中国还火，平安时代文人必读 / So readable a grandmother could understand. More famous in Japan than in China during the Heian period |
| 屈原 / Qu Yuan | 战国 | 📋 端午节因他而来 — 中国第一位署名诗人，《离骚》定义了浪漫主义 / The reason we have dragon boat races. China's first named poet |
| 王阳明 / Wang Yangming | 明 | 📋 「知行合一」 — 近十年全球最火的中国古代哲学家 / "Unity of knowledge and action." Silicon Valley's favorite Chinese philosopher right now |

---

## 贡献 / Contributing

每个新先贤遵循同一套流程：诗文采集 → 风格拆解 → 性格建模 → 时代还原 → 双模式 SKILL。参考 `01_数据与资料/` 下的结构即可上手。欢迎 PR。

Every new sage follows the same pipeline: Collection → Deconstruction → Personality → Time Travel → Dual-Mode Skill. Check the structure under `01_数据与资料/` to get started. PRs welcome.

---

## 许可 / License

MIT © 2026

诗文数据来源于古诗文网（gushiwen.cn），仅供学术研究与文化交流使用。
Poetry data sourced from gushiwen.cn for academic research and cultural exchange purposes only.
