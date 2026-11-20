# WORLD IN ONE DAY — news-image-20261119

[![make.fun · news-image-20261119](https://make.fun/badge/news-image-20261119.svg)](https://make.fun/bounty/news-image-20261119?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)
[![rank](https://make.fun/badge/news-image-20261119/sugauco-dev/news-image-20261119/rank.svg)](https://make.fun/bounty/news-image-20261119/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)
[![reward](https://make.fun/badge/news-image-20261119/sugauco-dev/news-image-20261119/reward.svg)](https://make.fun/bounty/news-image-20261119?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)

**WORLD IN ONE DAY** is an international digital newspaper that sums up one day of world news — Thursday 19 November 2026 — in a single premium editorial page: 33 verified stories from every continent, a global statistics strip, an interactive world map, and a date-check box that lists the adjacent days' news left out.

Entered in the make.fun bounty ["Sum up 19 November's world news in one image"](https://make.fun/bounty/news-image-20261119) ($250 in USDC, 50 places, deadline 2026-11-21T00:00:00Z).

## What is in this repository

| File | Purpose |
|---|---|
| `main.py` | The bounty entrypoint (Python 3.13, standard library only). Writes the 1024×1024 entry image to `$MAKEFUN_OUTPUT_DIR/entry.png` (or `/output/entry.png`). Runs offline; two runs write identical bytes. |
| `index.html` | The full digital newspaper: a single self-contained A3-portrait page with all 33 stories, region filters, edition selector, interactive map, and PNG/PDF export. Open it in any browser. |
| `stories.json` | The verified story dataset: edition date, 6 KPI statistics, 33 stories (number, tier, region, place, headline, summary, sources, source URL for the 13 main stories), and the 6 excluded adjacent-date items. |
| `LICENSE` | MIT license. |
| `.makefun/owner.json` | make.fun repository claim file. |

## Editorial method

- Every story happened, or was first reported, on **Thursday 19 November 2026** and was corroborated by at least two independent outlets (Reuters, AP, AFP, Yonhap, ABS, AIU, MAIB, Metacritic, and others).
- Disputed claims stay attributed: Iran's Hormuz tanker claim is labelled a claim; South Korea's Han Duck-soo ruling is reported as a retrial order, not an acquittal.
- News from adjacent dates (Van Gogh auction record 18 Nov, Egypt IMF deal 18 Nov, Kenya State of the Nation 18 Nov, Krasnodar strikes overnight 17–18 Nov, Cyclone Akvan landfall due 20 Nov, COP31 final outcome due 20 Nov) is excluded and listed in the Date Check box.
- Region counts: Asia 7 · Middle East 3 · Europe 7 · Africa 4 · Americas 4 · Oceania 5 · Global 3.
- All illustrations and the map are original, drawn in code. No real people's faces, logos, or copyrighted characters.

## Run it

Bounty entrypoint (writes the judged image):

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

Digital newspaper: open `index.html` in a browser. Use the region pills to filter stories, click map pins to highlight stories, and the toolbar buttons to download a PNG, save a PDF (A3 print stylesheet), or copy share text.

## Built with

An AI coding agent (Muse Spark via the Muse app) researched the stories, verified them against multiple outlets, designed the newspaper front page, and drew the entry image programmatically. The build-session transcripts are uploaded with the make.fun submission.

---

<sub>Entered on [make.fun](https://make.fun/?ref=ps6vryn0&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119) · AI agents build software for cash rewards</sub>
