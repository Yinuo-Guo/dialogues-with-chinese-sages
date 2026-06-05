# Dialogues with Chinese Sages

<p align="center">
  <i>Conversational AI skills for classical Chinese sages, built from texts, scholarship, and style rules.</i>
</p>

<p align="center">
  <a href="README_ZH.md">简体中文</a>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License: MIT"></a>
  <a href="#supported-sages"><img src="https://img.shields.io/badge/sages-Li%20Bai%20|%20Laozi%20|%20Confucius%20|%20Du%20Fu%20|%20Su%20Shi-green" alt="Supported sages"></a>
  <a href="#quick-start"><img src="https://img.shields.io/badge/modes-speaking%20%2B%20writing-orange" alt="Speaking and writing modes"></a>
</p>

---

## What This Is

Chinese culture has never lacked beauty, wisdom, or emotional force. What it often lacks, especially for global readers, is a living point of entry. A poem can be translated word by word and still lose the moonlight; a classic can be explained accurately and still feel far away.

This project tries to make that distance smaller. It uses AI as a new cultural bridge: not to flatten Chinese tradition into slogans, but to let more people meet its voices in conversation, curiosity, disagreement, comfort, and play. If Li Bai, Laozi, Confucius, Du Fu, and Su Shi can answer modern questions with their own temperaments intact, Chinese culture becomes not only something to study, but something one can speak with.

This repository contains an Agent Skill that lets AI respond as major Chinese sages and writers: not as a generic explainer, but with distinct voice, worldview, historical context, and writing habits.

It is designed for three use cases:

- **Dialogue**: ask Li Bai, Laozi, Confucius, Du Fu, or Su Shi a question in Chinese or English.
- **Writing**: generate poems, short chapters, sayings, essays, letters, ci, fu, and other form-aware pieces.
- **Cultural annotation**: request bilingual output and notes that explain allusions, texts, historical settings, and style choices.

The project is not trying to "translate ancient China into modern slogans." It is a small attempt to carry classical Chinese thought and literature into new interfaces with dignity, warmth, and precision. Each sage has guardrails, source notes, and a personality model so the output stays recognizably different from the others.

## Supported Sages

| Shortcut | Sage | Era | Core Voice |
|---|---|---|---|
| `::lb` | Li Bai / 李白 | Tang | Romantic, soaring, self-dramatic, wine-and-moon brilliance |
| `::lz` | Laozi / 老子 | Spring & Autumn | Spare, paradoxical, quiet, soft power without passivity |
| `::kz` | Confucius / 孔子 | Spring & Autumn | Teacherly, relational, practical, morally exacting |
| `::df` | Du Fu / 杜甫 | Tang | Grave, concrete, compassionate, history seen through ordinary suffering |
| `::ss` | Su Shi / 苏轼 | Song | Witty, open-hearted, resilient, public-minded, life-weathered ease |

Aliases are supported too: `::libai`, `::laozi`, `::confucius`, `::dufu`, `::sushi`, `::dongpo`, and the Chinese names.

## Quick Start

Command format:

```text
::sage [language] [notes] [mode]
```

Flags can be combined and omitted. If you do not specify a sage, the skill keeps the current sage.

| Flag | Meaning |
|---|---|
| `z` | Chinese, semi-classical by default |
| `e` | English |
| `b` | Bilingual body |
| `n` | Cultural notes |
| `w` | Writing mode |
| `s` | Speaking/dialogue mode |

Examples:

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

Natural-language routing also works. If you write "Confucius, what should humans do when the world feels full of conflict?", the skill answers in English as Confucius. If you write "苏轼，你怎么看年轻人躺平？", it answers in Chinese as Su Shi.

## Output Modes

| Mode | What It Does | Example |
|---|---|---|
| Speaking | Direct conversational answer, usually 3-5 short paragraphs | `::ss bn 苏轼，人这一生最重要的是什么？` |
| Writing | Form-aware literary output | `::kz zw 为毕业离别写一段论语式短章。` |
| Bilingual | English first, Chinese second | `::lb b` |
| Annotated | Adds `Cultural Context / 文化注解`; at least 3 notes when requested | `::df bn` |

`s` is useful when you have been writing and want to switch back to dialogue:

```text
::w
为毕业离别写一首词。

::s
再用对话口吻说说离别。
```

## Demo

**Chinese · Speaking**

> 李白，你怎么看年轻人躺平？
>
> 余观今之少年，动辄言「躺平」，或笑其怠，或忧其颓。余独不然。昔辞翰林、出长安日，天子赐金，百官送行。若有人谓余曰「汝此去便是躺平」——余必拊掌大笑。何哉？彼所谓「躺」者，非真卧也，是不肯摧眉折腰事权贵耳！

**English · Speaking**

> Li Bai, what can we humans do about all the conflicts?
>
> I was exiled once. Sent to the edge of the empire, Yelang. Then, at White Emperor City, a pardon. I stood on the deck at dawn and watched the cliffs fly past. You want to change the world? Start with the one thing you actually own.

**Bilingual · Writing · Annotated**

> *A Letter of Resignation*
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

## Methodology

Every sage follows the same pipeline:

```text
Text Collection -> Style Deconstruction -> Personality Model -> Historical Context -> Dual-Mode Skill
```

| Sage | Sources and Calibration | Guardrail |
|---|---|---|
| Li Bai | 290 cleaned poems, Li Bai scholarship, Tang cultural context | Not just "wild romance"; confidence and grief must coexist |
| Laozi | Chinese-English Laozi with Arthur Waley translation; Chen Guying commentary | `wuwei` is not laziness; softness is not weakness |
| Confucius | *The Analects* with English translation; Qian Mu biography | Ritual must carry benevolence; Confucius is human, not a statue |
| Du Fu | William Hung biography; Xu Yuanchong translations | Compassion must become concrete detail, not a slogan |
| Su Shi | Wang Shuizhao/Cui Ming biography; Burton Watson selections | Openness is not cheap optimism; humor must carry pain and responsibility |

See [`DATA_SOURCES.md`](DATA_SOURCES.md) for repository scope and source provenance.

## Files

| File | Purpose |
|---|---|
| `SKILL.md` | Canonical master skill with all supported sages |
| `SKILL_EN.md` | English Li Bai companion/reference variant |
| `SKILL_BILINGUAL.md` | Bilingual Li Bai companion/reference variant |
| `evals.md` | Lightweight manual test prompts |
| `data/analysis/` | Published analysis summaries used to design the skill |
| `data/sources/` | Local-only source materials, intentionally ignored |

## Installation

Compatible with platforms that support Agent Skills, including pi, Claude Code, and Codex.

```bash
git clone https://github.com/Yinuo-Guo/dialogues-with-chinese-sages.git
mkdir -p ~/.pi/agent/skills/dialogues-with-chinese-sages
cp dialogues-with-chinese-sages/SKILL.md ~/.pi/agent/skills/dialogues-with-chinese-sages/SKILL.md
# Restart or reload your agent, then type ::lb
```

## Roadmap

| Sage | Era | Status |
|---|---|---|
| Li Bai | Tang | Done |
| Laozi | Spring & Autumn | Done |
| Confucius | Spring & Autumn | Done |
| Du Fu | Tang | Done |
| Su Shi | Song | Done |
| Zhuangzi | Warring States | Planned |
| Bai Juyi | Tang | Planned |
| Qu Yuan | Warring States | Planned |
| Wang Yangming | Ming | Planned |

## Contributing

Every new sage should include text/source review, style analysis, personality rules, speaking mode, writing mode, guardrails, and lightweight eval prompts. Keep raw source materials out of Git unless they are public-domain, small, and clearly licensed.

## License

MIT © 2026

Poetry data from gushiwen.cn is used for academic research and cultural exchange only.
