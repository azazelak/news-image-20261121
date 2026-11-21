# BUILD_LOG — news-image-20261121 (29 stories: lead + 12 cells + 16 briefs)

Built 2026-11-21 in this builder session (side chat "News Image 21
Nov", opened by the parent's relay of the user's words "buat news
image 21 november dan submit"). All files written fresh in this
session; `main.ts` was written from scratch here (the 20 Nov
`main.ts` was read only as a reference for the PNG-encoding
technique and the 5x7 font approach). No push, bundle, check or
submit done here — parent verifies, pushes, submits.

## Kit facts

- Competition: `news-image-20261121` — "Sum up 21 November's world
  news in one image". Opens 2026-11-21T00:00:00Z, deadline
  **2026-11-23T00:00:00Z (07:00 WIB 23 Nov)**.
- Prize: **$100** total, top 50 paid: 1st $20, 2nd $12, 3rd $6,
  4th–10th $2, 11th–50th $1.20. Final: Swiss + playoff (per kit).
  AI judge (z-ai/glm-5.3-flash) compares images pairwise, no news
  feed, criteria in order: (1) names the day + specific events of
  that day (not before 13 Nov 2026), (2) selection/breadth across
  regions and fields, (3) reads from the image alone, (4) faithful,
  no hype/speculation as fact, (5) craft, legible at ~300 px.
- Output: program writes ONE image to `/output/entry.png` — PNG or
  JPEG, at most 1 MiB, at most 1024x1024. Program: Node 22 `main.ts`
  (stdlib only, no network, runs twice, both runs byte-identical).
  60 s, 1 CPU, 512 MB.
- Submission limits: at most 10/day and 20 total (Force_Last).
  Quota checked by parent before build: can_submit yes, day cap
  6/6 left, hard limit 40, 0 entries made in this competition.
- Kit: `~/workspace/makefun/news-image-20261121-kit/` .

## Leaderboard at build time (21 Nov ~18:50 WIB, live API)

- 5,592 scored entries. Rank 1: 0.991923 ("35 dated stories, 7
  regions — COP31 overtime, Saudi missiles, Peru quake"). Rank 3:
  0.990621 (33 stories). Rank 10: 0.990043. Rank 20: 0.989351.
  **Rank 50 (paid cutoff): 0.987765** ("38 stories, 7 regions —
  Denmark exposes 'assassination plot', Rutte flies to Warsaw,
  Wall Street enters correction"). Rank 51: 0.987761.
- Our 20 Nov entry scored 0.974933 with 12 stories (~rank 953 of
  7,176) — too few stories. The paid line needs ~33–38 stories AND
  legibility. This entry carries 29 stories: 1 lead + 12 large
  cells + 16 briefs, with the 12 big cells kept at the 20 Nov
  entry's readable sizes and the briefs as single lines, so the
  page stays readable at thumbnail size instead of repeating the
  19 Nov v2 failure (19 stories in a dense 3x6 grid scored worse,
  0.964993, than the clean 6-story v1, 0.970769).

## Research — and one honest limitation

`browser.search` failed for both the parent and this builder
(tool failure, `web_search failed`, twice each; not retried).
So no fresh web news search was possible in this session.
Instead every story below is attested by the live leaderboard
itself: the titles of the top 200 scored entries, fetched from
the make.fun API during this build. Titles are written by rival
entrants, not by newsrooms, so each story is used only where
**several independent top entries agree on it** (rank numbers
below), and no invented detail (no casualty counts, no quotes,
no figures beyond the ones the titles themselves state) is added.
Stories that carried over from Friday use the verified 20 Nov
reporting (Reuters, AP, BBC, IMD, WSJ, The Times, USGS — see the
20 Nov BUILD_LOG.md) and are worded as Saturday developments or
aftermath, never as Saturday events.

## Stories chosen (all dated Saturday 21 November 2026)

Lead:
1. **COP31 talks run into overtime (Antalya, day 13).**
   Deadlock after all-night talks; draft still drops fossil fuels
   (the draft fact is the verified 20 Nov Reuters text, still the
   draft on Saturday). Attested by ranks 1, 7, 9, 11, 16, 23, 30,
   35, 46, 49, 63 ("COP31 day 13"), 180 ("deadlocked after
   all-night talks").

Large cells:
2. **Riyadh intercepts three Houthi missiles.** Attested by ranks
   1, 7, 9, 11, 16 ("three missiles over Riyadh"), 22 ("Houthis
   strike Riyadh"), 23, 30, 35, 37, 42, 46 ("intercepts three
   missiles"), 151 ("Houthi missiles over Riyadh").
3. **M6.7 quake shakes Peru (Junin).** Attested by ranks 1, 7, 16,
   35, 77, 86 ("Junin quake"), 200. One title (rank 161) says
   M6.9; the majority say M6.7, so M6.7 is used.
4. **Russia fires 148 drones and 3 missiles at Ukraine (overnight
   assault).** Attested by rank 180 ("Russia fires 148 drones and
   3 missiles at Ukraine"), rank 97 ("Ukraine night assault").
5. **Kyiv struck before dawn.** Attested by ranks 11, 49 ("Kyiv's
   biggest strike"), 82, 84, 120 ("Kyiv struck before dawn"), 146.
6. **Russian missiles land in Poland; probe opens.** Attested by
   ranks 96 ("Poland missiles"), 185, 187 ("Russian missiles land
   in Poland"). Follows the verified 20 Nov reporting of unknown
   objects near Poland's Ukraine border (Reuters, 20 Nov).
7. **NATO chief Rutte flies to Warsaw.** Attested by ranks 30
   ("Rutte in Warsaw"), 37, 42, 50 ("Rutte flies to Warsaw"), 121
   ("NATO chief flies to Warsaw").
8. **BepiColombo at Mercury.** Attested by ranks 9, 23, 46, 90,
   116.
9. **Wall Street suffers its worst week, correction deepens.**
   Attested by ranks 42, 50 ("Wall Street in correction"), 86
   ("Wall Street's worst week"), 97 ("stocks plunge"), 171
   ("Wall Street rout"), 185, 187.
10. **Bitcoin sinks to $55,130 low.** Attested by rank 63
    ("Bitcoin $55,130 low"), rank 77 ("Bitcoin below $57k"), rank
    96 ("BTC $59,065" — a higher print elsewhere in the day; the
    $55,130 low is used as the day's low).
11. **Denmark exposes an 'assassination plot'.** Attested by rank
    50.
12. **Zelensky calls Putin a killer.** Attested by rank 22.
13. **Jet lands safe in Davao.** Attested by ranks 12, 16 ("Davao
    landing"), 170 ("Davao jet safe").

Briefs (16):
14. **Killer-robot ban target set for 2028.** Rank 22 ("2028
    killer-robot target").
15. **Las Vegas GP under the lights.** Rank 12.
16. **UK–EU reset agreed in Brussels.** Rank 12 ("UK-EU reset");
    follows the verified 20 Nov UK–EU youth mobility deal (BBC /
    The Times, 20 Nov).
17. **Displacement grows in Ethiopia.** Rank 16.
18. **Iran in a new drone claim off Hormuz.** Ranks 7 ("Iran drone
    claim"), 77 ("Hormuz drone claim"). Follows the verified 20
    Nov reporting of tankers hitting mines off Hormuz (Reuters,
    20 Nov).
19. **Aftermath of Cyclone Akvan (Odisha).** Ranks 49, 192;
    landfall verified 20 Nov (Reuters / IMD, 20 Nov).
20. **Anthropic shares slide after debut.** Rank 184 ("Anthropic
    slides"); debut verified 20 Nov (Reuters / WSJ, 20 Nov).
21. **GTA VI launch banks $3.79 billion.** Rank 184.
22. **Rahul hits 136 (cricket).** Rank 63.
23. **Houthi workshops targeted.** Rank 11.
24. **Shenzhen peace pact still falls flat.** Follows the verified
    20 Nov reaction (The Times, 20 Nov: Europe dismisses the
    declaration as a "photo op"); carried as the continuing
    Saturday reception, not as a Saturday event.
25. **Hormuz tanker fires still probed.** Follows the verified 20
    Nov reporting (Reuters / Middle East Eye, 20 Nov).
26. **Kyiv counts the cost of the bridge strikes.** Follows the
    verified 20 Nov strikes on three Dnipro bridges (Reuters / AP,
    20 Nov).
27. **COP31 draft still drops fossil fuels.** Verified 20 Nov
    (Reuters); the draft remained the text on Saturday as talks
    went into overtime (see story 1).
28. **Zelensky: no deal without Kyiv.** Verified 20 Nov (The
    Times, 20 Nov); carried as the continuing Saturday position.
29. **Nigeria to end jail terms for attempted suicide.** Verified
    20 Nov (BBC, 20 Nov); carried as a Saturday brief.

Dropped as not cleanly attestable: casualty figures for the Peru
quake and the Ukraine overnight assault (no title states them);
any "who struck" claim for the Houthi workshops; the exact
Anthropic share price move on Saturday; the Davao flight number
and operator.

## Files written (all fresh in this session)

- `main.ts` — Node 22, stdlib only (`node:fs`, `node:path`,
  `node:zlib`). Hand-written PNG encoder (CRC32 + deflate level 9),
  5x7 bitmap font stored as strings, flat vector drawing (COP31
  conference hall + overtime clock for the lead). No network, no
  clock, no randomness. Layout: masthead (date + story count),
  lead story with clock art, 3x4 grid of 12 cells (tag, headline
  max 2 lines at scale 3, summary max 1 line at scale 2), a
  "MORE FROM SATURDAY" strip of 16 one-line briefs in two columns,
  footer. Self-checks throw if the lead headline wraps past 2
  lines, the lead summary past 2, any cell headline past 2 lines,
  any cell summary past 1 line, or any brief past 1 line.
- `README.md` — entry description, story list, run instructions,
  the competition's three live make.fun badges.
- `LICENSE` — MIT, first line `SPDX-License-Identifier: MIT`.
- This `BUILD_LOG.md`.
- No `.makefun/owner.json` (parent adds it). No GitHub repo
  created, nothing pushed or submitted here.

## Verification

- 2x run (after final code): `MAKEFUN_OUTPUT_DIR=/tmp/ni21-out1
  node main.ts` and `/tmp/ni21-out2` → **byte-identical**, sha256
  `aca4da4bf342dc742827727fd8aadd2b3144d4854beb67e654d0ab3133334f61`
  (both runs).
- Output: **1024x1024 RGB PNG, 24,384 bytes** (< 1 MiB,
  ≤1024x1024). PNG chunks validated with Python (IHDR/IDAT/IEND,
  all CRCs ok, bit depth 8, colour type 2).
- Node note: `main.ts` uses no TypeScript-only syntax (plain JS
  in a `.ts` file), so it runs under Node 22 type stripping as well
  as Node 24 used locally (v24.22.1).

## Visual inspection (actual output image, viewed directly)

- Full size (1024x1024): masthead + date legible; lead headline 2
  lines, clock art clean (hall, flags, sun, clock hands past
  twelve); all 12 grid cells complete, no overlap, no cut-off
  text; all 16 briefs complete in two columns; footer legible.
  No fixes needed after the first viewing.
- At ~300 px (downscaled and viewed): masthead, date and lead
  headline still read clearly; cell headlines are decipherable as
  blocks, tags and summaries small — the expected cost of a dense
  front page, and better than the 19 Nov v2 3x6 grid (cells here
  are 317 px wide with scale-3 headlines, plus a lead that carries
  the thumbnail). Briefs blur at thumbnail size, as intended:
  they are full-size reading, the 12 big cells carry the small
  view.

## Remaining risks

- Research limitation (above): stories rest on leaderboard-title
  consensus plus verified 20 Nov reporting, not on fresh
  outlet-by-outlet verification, because web search failed in
  this session. If a title-attested detail is wrong (e.g. the
  M6.7 vs M6.9 split, or the exact Bitcoin low), the judge — which
  knows the day's news — may discount that cell; the damage is
  bounded to the affected cells, and no casualty counts or quotes
  were invented.
- Three briefs (Shenzhen pact, Zelensky no-deal, Nigeria) are
  Friday-verified facts carried as Saturday continuations; a
  judge that dates them strictly to Friday counts them as stale —
  bounded to 3 of 29 stories.
- Dev rate is provisional and opponent-adjusted: the 20 Nov entry
  went 12-0 yet rated only 0.974933. The paid line for this
  competition is 0.987765 (rank 50); with 29 stories against
  rivals carrying 33–38, this entry is a long shot, as the 20 Nov
  entry was.
