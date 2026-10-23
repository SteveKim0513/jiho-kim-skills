# Jiho Kim Skills

A single `CLAUDE.md` in the layout of [andrej-karpathy-skills](https://github.com/forrestchang/andrej-karpathy-skills), built from 615 real sessions (5,855 messages, 2025-09-11 to 2025-10-23). The guideline text is Korean on purpose, because replies must be in Korean.

[한국어](./README.md) | English

## Why

AI output is often not good, for two reasons.

- **The AI takes the lead.** It is a probabilistic model, so when it holds the direction, quality varies from run to run.
- **Complexity climbs.** It solves problems in increasingly complex ways and drifts away from the original problem.

Two principles follow: **the user sets the direction; complexity is a budget.**

## Six rules

| # | Rule | Prevents |
|---|---|---|
| 0 | If direction is missing, keep asking | Gaps filled by guessing |
| 1 | The user decides, the AI proposes | Lost initiative, reversed decisions |
| 2 | Complexity is a budget | Piling on, stacking attempts on one problem |
| 3 | When corrected, find the whole pattern | Fixing one spot, band-aids |
| 4 | Only verified work is "done" | Unchecked "all done" |
| 5 | Never overwrite others' changes | Parallel-session conflicts |

Full text: [CLAUDE.md](./CLAUDE.md). Examples: [EXAMPLES.md](./EXAMPLES.md).

## Versus Karpathy

Rules 0 and 1 go beyond stating assumptions: they ask until no gap remains. Rule 2 matches Simplicity First and adds a stop after two failed fixes. **Rule 3 is the opposite of Surgical Changes:** one correction widens to the same pattern everywhere, but only the same problem, and other problems are reported, not fixed. Rule 4 adds using the product as a real user and a fixed completion report. Rule 5 is new. If both are installed, this rule 3 wins.

## Install

```
/plugin marketplace add SteveKim0513/jiho-kim-skills
/plugin install jiho-kim-skills@jiho-kim-skills
```

Plugin skills load when Claude judges the description relevant, so they are not always on. For always-on, append [CLAUDE.md](./CLAUDE.md) to `~/.claude/CLAUDE.md`.

MIT
