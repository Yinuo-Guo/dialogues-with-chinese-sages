# Data Sources

This repository combines public-domain classical texts, manually curated notes, and research summaries for building the `dialogues-with-chinese-sages` skill.

## Included in Git

| Path | Contents | Notes |
|---|---|---|
| `data/poems/李白诗选_纯净版.txt` | Cleaned Li Bai poem corpus | Compiled from gushiwen.cn for academic research and cultural exchange. |
| `data/poems/完整诗目.md` | Poem title index | Used for quick lookup and coverage checks. |
| `data/poems/诗文分类目录.md` | Thematic poem catalog | Manual thematic grouping for skill design. |
| `data/analysis/李白风格分析.md` | Style analysis | Manually synthesized from the poem corpus and scholarship. |
| `data/analysis/李白性格分析_权威研究.md` | Personality model and scholarship notes | Summarizes Li Bai studies by Li Changzhi, Yuan Xingpei, Lin Geng, Matsuura Tomohisa, Stephen Owen, Zhou Xunchu, and others. |
| `data/analysis/唐朝背景知识.md` | Tang Dynasty context | Background for daily life, travel, institutions, poetry culture, and relationships. |
| `data/analysis/老子思想与风格分析.md` | Laozi style and philosophy analysis | Skill-facing synthesis based on Waley's translation and Chen Guying's commentary. |
| `data/analysis/孔子思想与风格分析.md` | Confucius style and philosophy analysis | Skill-facing synthesis based on The Analects and Qian Mu's biography. |
| `data/translations/许渊冲英译李白诗选.md` | Xu Yuanchong translation notes/excerpts | Used to calibrate English style and cross-cultural annotation. |

## Kept Local

Large raw archives and source documents are intentionally excluded by `.gitignore`:

| Path | Reason |
|---|---|
| `data/archive/*.pdf` | Large source/reference files; not required for normal skill use. |
| `data/archive/all_poems_raw.txt` | Raw scrape/intermediate corpus. |
| `data/archive/周勋初_李白评传.md` | Local research notes/source material; summarized into included analysis files. |
| `data/sources/老子 英汉对照 (韦利英译）.md` | Local source text used to build the Laozi module; not published in full. |
| `data/sources/老子注译及评介 (陈鼓应).md` | Local commentary source used to build the Laozi module; not published in full. |
| `data/sources/论语 英汉对照.md` | Local source text used to build the Confucius module; not published in full. |
| `data/sources/钱穆《孔子传》.md` | Local biography source used to build the Confucius module; not published in full. |

## Historical Files

`legacy/李白SKILL_完整版.md` is retained as a historical draft of the Li Bai skill. It is not the current entry point; use `SKILL.md` for the active skill.

## Use Policy

Poetry data is provided for academic research, cultural exchange, and skill evaluation. The skill itself should avoid fabricating biographical details and should treat cited historical facts as bounded by the included analysis files.
