# Jiho Kim Skills

A single `CLAUDE.md` in the layout of [andrej-karpathy-skills](https://github.com/forrestchang/andrej-karpathy-skills), built from 615 real sessions (5,855 messages, 2025-09-11 to 2025-10-23). The guideline text is Korean on purpose, because replies must be in Korean.

[한국어](./README.md) | English

## Why

AI output is often not good, for three reasons.

- **The AI takes the lead.** It is a probabilistic model, so when it holds the direction, quality varies from run to run.
- **It sees only the part.** While fixing one spot it loses the whole context.
- **Complexity climbs.** It solves problems in increasingly complex ways and drifts away from the original problem.

Three principles follow: **the user sets the direction, keep the whole context, complexity is a budget.**

## Structure

**Common rules** (every task)

| # | Rule | Prevents |
|---|---|---|
| 1 | If direction is missing, keep asking | Gaps filled by guessing |
| 2 | The user decides; keep the whole context | Lost initiative, the whole bent to fit a part |
| 3 | Complexity is a budget | Piling on, stacking attempts on one problem |
| 4 | When corrected, find the whole pattern | Fixing one spot, band-aids |
| 5 | Only verified work is "done" | Unchecked "all done" |

**Conversation:** plain Korean, multiple choice with a recommendation, show instead of tell, read short commands narrowly, fixed completion report.

**Development:** MECE structure, code that keeps the core design instead of patching on, replace old features rather than keeping both, verify directly, safe deploys and git.

Full text: [CLAUDE.md](./CLAUDE.md). Examples: [EXAMPLES.md](./EXAMPLES.md).

## Versus Karpathy

**Rule 4 is the opposite of Surgical Changes:** one correction widens to the same pattern everywhere, but only the same problem, and other problems are reported, not fixed. If both are installed, this rule 4 wins. The rest extends Karpathy's direction: ask until no gap remains, keep the whole context, keep the design MECE, and verify as a real user.

## Install

```
/plugin marketplace add SteveKim0513/jiho-kim-skills
/plugin install jiho-kim-skills@jiho-kim-skills
```

Plugin skills load when Claude judges the description relevant, so they are not always on. For always-on, append [CLAUDE.md](./CLAUDE.md) to `~/.claude/CLAUDE.md`.

MIT
