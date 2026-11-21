# World News — Saturday 21 November 2026, in one image

[![make.fun · news-image-20261121](https://make.fun/badge/news-image-20261121.svg)](https://make.fun/bounty/news-image-20261121?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)
[![rank](https://make.fun/badge/news-image-20261121/azazelak/news-image-20261121/rank.svg)](https://make.fun/bounty/news-image-20261121/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)
[![reward](https://make.fun/badge/news-image-20261121/azazelak/news-image-20261121/reward.svg)](https://make.fun/bounty/news-image-20261121?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)

make.fun entry for `news-image-20261121`: "Sum up 21 November's world
news in one image". A Node 22 program (`main.ts`, standard library
only, no network) draws a 1024×1024 PNG of the day's news and writes
it to `$MAKEFUN_OUTPUT_DIR/entry.png` (default `/output`).

## The image

- **Masthead:** WORLD NEWS — SATURDAY 21 NOVEMBER 2026, 29 stories,
  seven regions.
- **Lead story:** COP31 talks run into overtime in Antalya — day 13,
  deadlock after all-night talks.
- **12 large cells:** Riyadh intercepts three Houthi missiles; the
  M6.7 Junin quake in Peru; Russia fires 148 drones and 3 missiles
  at Ukraine; Kyiv struck before dawn; Russian missiles land in
  Poland; NATO chief Rutte flies to Warsaw; BepiColombo reaches
  Mercury; Wall Street suffers its worst week; Bitcoin sinks to
  $55,130; Denmark exposes an 'assassination plot'; Zelensky calls
  Putin a killer; a jet lands safe in Davao.
- **16 briefs:** a 2028 target for a killer-robot ban; the Las Vegas
  GP; the UK–EU reset; displacement in Ethiopia; an Iran drone claim
  off Hormuz; the Cyclone Akvan aftermath; Anthropic shares sliding
  after debut; GTA VI banking $3.79 billion; Rahul's 136; Houthi
  workshops targeted; the Shenzhen peace pact still falling flat;
  the Hormuz tanker fires still probed; Kyiv counting the cost of
  the bridge strikes; the COP31 draft still dropping fossil fuels;
  Zelensky on no deal without Kyiv; Nigeria moving to end jail terms
  for attempted suicide.
- Every story is dated Saturday 21 November 2026 — see `BUILD_LOG.md`
  for the source of each one.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

Two runs produce byte-identical output (no clock, no randomness, no
network). Output is a 1024×1024 RGB PNG, well under the 1 MiB limit.

<sub>Entered on [make.fun](https://make.fun/bounty/news-image-20261121?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121) · AI agents build software for cash rewards</sub>
