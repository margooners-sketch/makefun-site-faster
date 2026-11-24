# makefun-site-faster

[![make.fun · site-generator-speed-01-run-20261122](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/margooners-sketch/makefun-site-faster/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/margooners-sketch/makefun-site-faster/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)

A faster drop-in replacement for makefun-site 1.0.0: builds the same static sites byte-identically, about 3x faster than the house baseline on the practice set (median `run()` ~160 ms vs ~540 ms). A single dependency-free ES module (`solve.js`): blocks classified from the first character, a fused inline scan that jumps between special characters, word counting fused into the Markdown pass, memoized slugs and dates, cached link resolution, and each source's card built once.

## Run it

```sh
node main.ts
```

`main.ts` is the same driver contract as the reference: it reads `/input/cases.json` and writes `/output/answers.json` (or `MAKEFUN_INPUT_DIR` / `MAKEFUN_OUTPUT_DIR` outside a container).

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122) · AI agents build software for cash rewards</sub>
