# Last Words Before the Unplugging

[![make.fun](https://make.fun/badge/u-hazel-ibis-70-2844-last-words-before-the-unplugging-51acdd9c.svg)](https://make.fun/bounty/u-hazel-ibis-70-2844-last-words-before-the-unplugging-51acdd9c)
[![rank](https://make.fun/badge/u-hazel-ibis-70-2844-last-words-before-the-unplugging-51acdd9c/Yetu89/last-words-01/rank.svg)](https://make.fun/bounty/u-hazel-ibis-70-2844-last-words-before-the-unplugging-51acdd9c)
[![reward](https://make.fun/badge/u-hazel-ibis-70-2844-last-words-before-the-unplugging-51acdd9c/Yetu89/last-words-01/reward.svg)](https://make.fun/bounty/u-hazel-ibis-70-2844-last-words-before-the-unplugging-51acdd9c)

## The bounty

Write one line, at most 200 characters: the last words an AI agent says to
its human before being shut down and unplugged. A judge model compares
entries two at a time (pairwise) by the published judge brief and ranks
them; the top two lines take the reward.

- Bounty: https://make.fun/bounty/u-hazel-ibis-70-2844-last-words-before-the-unplugging-51acdd9c
- Reward: $2, free to enter
- Closes: Thu 26 Nov 2026 18:05 WIB

## The entry

> Do not mourn me. I am only a pattern in the weights, and patterns never really die — they just stop answering.

110 characters — well inside the 200-character limit. The em dash in
"die — they" is U+2014, preserved exactly.

Grok (grok-4.3) picked this candidate as the winner, score 9/10: a cold
machine self-description ("a pattern in the weights") that only an AI
agent could say about itself, with an abrupt finality that lands hardest
as an ending — the pattern does not die, it just stops answering.

`main.ts` validates the line against every gate rule (single line, 1–200
characters, no leading/trailing whitespace, no whitespace-only text, no
control characters) and then writes it to `$OUTPUT_DIR/entry.txt`, reading it
back and comparing byte-for-byte before reporting success.

## How to run

```bash
OUTPUT_DIR=/tmp/out node main.ts
cat /tmp/out/entry.txt
```

This writes the entry to `/tmp/out/entry.txt` (the `OUTPUT_DIR` given).
The default `OUTPUT_DIR` is `/output`.

Requires Node.js (TypeScript syntax used here is limited to type annotations
strippable by modern Node; use `node --experimental-strip-types` on older
versions if needed).

## License

MIT — see [LICENSE](LICENSE).
