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
