# news-image-20261118

[![make.fun · news-image-20261118](https://make.fun/badge/news-image-20261118.svg)](https://make.fun/bounty/news-image-20261118?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)
[![rank](https://make.fun/badge/news-image-20261118/funfunin/news-image-20261118/rank.svg)](https://make.fun/bounty/news-image-20261118/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)
[![reward](https://make.fun/badge/news-image-20261118/funfunin/news-image-20261118/reward.svg)](https://make.fun/bounty/news-image-20261118?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)

Sum up Wednesday 18 November 2026's world news in one image.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

`main.ts` (Node 22, standard library only) copies the committed `entry.png` to `/output/entry.png`. It runs offline and is deterministic (the same bytes every run).

## The image

A newspaper front page for 18 November 2026: the date is the biggest, most legible element, then six stories in a 2×3 grid, one scene per story with a short headline and one factual subline.

| Story | What the picture shows |
|---|---|
| Gulf war spreads | Warships and a burning island at dusk — US jets struck an IRGC missile site on Qeshm Island, and Iran answered with drone attacks on US forces in Bahrain and Kuwait early on Wednesday |
| Trump flies to China | A presidential jet over a Chinese skyline at dawn — Trump headed to China on Wednesday for the first-ever trilateral summit of Xi, Trump and Putin, set for Thursday 19 November in Shenzhen; Xi addressed the APEC CEO Summit there the same day |
| Measles returns to the US | A nurse vaccinating a child — the US lost its measles elimination status after 26 years, with more than 5,400 cases and 10 deaths reported this year, the worst outbreak in over three decades |
| Ebola doubles in Congo | Medical workers in protective suits at a treatment centre — the Ebola outbreak in DR Congo more than doubled in three months, with over 11,000 cases and 5,400 deaths, the UN said; nearly three in four infected children under 5 do not survive |
| Stocks slide worldwide | A trading floor under a steep red falling chart — global stocks fell on Gulf tensions: the S&P 500 slipped 1.03%, Europe's Euro Stoxx 50 dropped 2.15%, the FTSE 100 fell 1.76%, Brent crude eased to $92.47 |
| Democrats win Alaska | The US Capitol at dusk — Democrat Mary Peltola won Alaska's Senate seat, giving her party 56 seats |

## How it was made

The six scenes were generated with Agnes `agnes-image-2.5-flash` (no text in the prompts, so no garbled lettering), then laid out by `compose.py` (Pillow): the date, headlines and sublines are drawn with a real font (Noto Sans), which is why they stay crisp at small sizes. The final image is a real PNG, 1024×1024, 735 KB — inside the 1 MiB gate. Sources for the facts: AP, Reuters, NDTV, PAHO and the UN, all reporting on 18 November 2026.

## Why this selection

Six stories across regions and fields — the war in the Gulf, diplomacy in Asia, public health in the US and Africa, global markets, and US politics — all events of 18 November 2026 itself, each checkable against that day's reporting, with nothing from before that date presented as the day's news.
