# Wednesday 25 November 2026 — in one image

[![make.fun](https://make.fun/badge/news-image-20261125.svg)](https://make.fun/bounty/news-image-20261125)
[![Rank](https://make.fun/badge/news-image-20261125/gom92/makefun-news-image-20261125/rank.svg)](https://make.fun/bounty/news-image-20261125)
[![Reward](https://make.fun/badge/news-image-20261125/gom92/makefun-news-image-20261125/reward.svg)](https://make.fun/bounty/news-image-20261125)

A front-page image summing up the world news of **Wednesday 25 November 2026**,
built for the [make.fun bounty](https://make.fun/bounty/news-image-20261125).

## The day

- **Lead — Strait of Hormuz:** Iran says two oil tankers struck naval mines
  and caught fire in the Strait of Hormuz; the Revolutionary Guard blamed
  vessels on an unauthorised route.
- **Space:** China's Shenzhou-24 launches from Jiuquan carrying Muhammad
  Zeeshan Ali, Pakistan's first astronaut and the first foreign astronaut
  aboard the Tiangong space station.
- **Briefs:** the US proposes new tariffs on 14 trading partners; Asian
  markets plunge (KOSPI −6.16%) and the Nasdaq slides; Huawei is found
  guilty of trade-secret theft and bank fraud in a US court; the Houthis
  claim a refinery attack in Saudi Arabia a day after a Riyadh tower strike
  injured 11; an Israeli strike kills Hamas security chief Mohammad
  Abuelouf in Gaza; Australia and Solomon Islands sign a treaty barring
  any foreign military base.
- **Numbers:** 2 tankers on fire · KOSPI −6.16% · Dow's first close above
  50,000 (50,019) · 19 civilians killed in RSF drone strikes in Sudan.

Sources: Reuters, AP, BBC, New York Times, Dawn. Events are those that
happened or were first reported on 25 November 2026.

## How it is made

`tools/render_frontpage.py` draws the 1024×1024 front page with Pillow:
masthead, the two photo panels (generated fresh for this entry and kept
under `assets/`), the briefs and the numbers strip. `main.py` copies the
finished `entry.png` to the output directory.

```sh
python3 tools/render_frontpage.py   # rebuild entry.png
MAKEFUN_OUTPUT_DIR=out python3 main.py
```

The program uses only the Python standard library, needs no network, and
writes byte-identical output on every run.

## Verification

- `entry.png` is 1024×1024 PNG, under 1 MiB.
- `main.py` was run twice offline; both runs produced the same SHA-256.
- The rendered page was viewed and checked: the date, both stories, all
  six briefs and the numbers strip are legible, with nothing clipped or
  overlapping.

## Referral

Use referral code `radjee14` when you sign up on make.fun.

## License

MIT — see [LICENSE](LICENSE).
