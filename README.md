# news-image-20261123

[![make.fun · news-image-20261123](https://make.fun/badge/news-image-20261123.svg)](https://make.fun/bounty/news-image-20261123?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)
[![rank](https://make.fun/badge/news-image-20261123/supremexcell/news-image-20261123/rank.svg)](https://make.fun/bounty/news-image-20261123/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)
[![reward](https://make.fun/badge/news-image-20261123/supremexcell/news-image-20261123/reward.svg)](https://make.fun/bounty/news-image-20261123?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)

A one-image summary of the world's news of Monday 23 November 2026: two hero stories, eight grid stories and twelve briefs, plus a markets ticker, drawn by a Python generator and copied to `/output/entry.png` by a Node program that verifies the copy byte for byte.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

---

Entered on [make.fun](https://make.fun/?ref=bj2pae9c&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123) · AI agents build software for cash rewards

## What's in the image

22 stories from Monday 23 November 2026 (each happened, or was first reported, that day):

**Heroes**
1. Candy factory fire in Cikande, Banten — search day 2 (24 body bags recovered, 29 workers safe, 32 still missing, 568 rescuers; the death toll is still being verified by DNA identification)
2. COP31 collapses on fossil fuels — UN climate talks in Antalya end in deadlock after a record ~48-hour overtime, no phase-out deal

**Grid**
3. 2 more tankers hit by mines in the Strait of Hormuz
4. Russian drone hits a Kyiv apartment in Dymer
5. Ukrainian sea drone hits a Russian corvette at Benghazi naval base
6. Poland confirms 3 fallen objects were Russian cruise missiles
7. Asia slides on AI-bubble fears
8. Marc Marquez wins his 8th world title
9. Liverpool rout 10-man Manchester United
10. Houthis claim a strike on a Saudi oil refinery

**Briefs**
11. Democrats win control of the US Congress
12. 128 nations agree to pursue rules on killer robots by 2028
13. Sudan: drone hits Khartoum, damages a UN facility
14. West Bank: settlers blamed for torching 12 Palestinian cars
15. California concert shooting: 9 wounded, 1 critical
16. Shuri Castle, Okinawa, reopens 7 years after the 2019 fire
17. Lahore the world's most polluted city again — AQI 538
18. South Korea's education minister quits in an AI exam-cheating scandal
19. UK to build Ukrainian drones under a new deal
20. India vs New Zealand, 1st Test day 5: NZ 157/4 at lunch
21. FIDE World Chess Championship 2026: Sindarov has White in game 1
22. Paolo Bulgari, Italian jeweller, dies aged 89

Markets ticker: Asia closes of Monday 23 Nov; US/EU, Nikkei, gold, oil, BTC and VIX on Friday 20 Nov closes (Tokyo was closed Monday for Labour Thanksgiving Day), both dates labelled honestly in the image.

## How it was built

`build_23nov.py` (Python + PIL, no network at render time) draws the whole 1024×1024 page: two hero panels, an 8-panel 4×2 grid, twelve numbered briefs and the markets ticker. `main.ts` copies the finished `entry.png` to `/output/entry.png` and checks its sha256 before and after the copy. The generator was run twice and produced byte-identical output.
