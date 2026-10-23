# Jiho Kim Skills

A single `CLAUDE.md` in the same shape as [forrestchang/andrej-karpathy-skills](https://github.com/forrestchang/andrej-karpathy-skills), but derived from one person's real usage: 615 sessions and 5,855 messages (2025-09-11 to 2025-10-23), read in full.

[한국어](./README.md) | English

## What the data showed

| Number | Meaning |
|---|---|
| 44% of messages are 15 characters or fewer | Short instructions are the default. Guessing scope fails |
| 37% of sessions (230) start with a one-word command like "deploy" | One-word commands need a predefined default scope |
| "Plan first" asked in 30+ sessions | Planning comes before implementation |
| Reply of just "한글" ("Korean") in 30+ sessions | Answering in English means rework |
| "Don't interpret narrowly, re-check everything" in 8 to 11 sessions per period | One piece of feedback signals a violated principle, not a single case |

One line: a meticulous director who demands **plan first, keep it simple, fix the whole thing at the root, verify by hand.** The same person states criteria late and gives one-word commands, which is the biggest cause of rework. So the guidelines add a rule 0 where the AI fills that gap.

## How it differs from the Karpathy guidelines

| Karpathy | This repo | Why |
|---|---|---|
| Think Before Coding | 1. Plan, show, let them choose | Go beyond stating assumptions: multiple choice with a recommendation, and a sample screen instead of prose |
| Simplicity First | 2. Simple, by removing | Same direction. Deleting an existing feature requires asking first |
| **Surgical Changes** | **3. Fix the whole thing at the root** | **Opposite.** One correction triggers a full sweep of the same pattern. Boundary: same problem everywhere, other problems reported only |
| Goal-Driven Execution | 4. Use it yourself, prove it's done | Beyond tests: act as a real user. Fixed format for "is it done?": verified / not verified / remaining |
| (none) | 0. Set scope and criteria before starting | The AI compensates for criteria stated late |
| (none) | 5. Parallel session safety | Several sessions edit the same repo; check `git status` first, never overwrite others' changes |

If both are installed, rule 3 conflicts. This repo's rule 3 wins. Karpathy's "don't touch unrelated problems" still holds.

## Install

```
/plugin marketplace add SteveKim0513/jiho-kim-skills
/plugin install jiho-kim-skills@jiho-kim-skills
```

Or copy [CLAUDE.md](./CLAUDE.md) into a project. The guideline text itself is in Korean, because the replies must be in Korean.

## Files

`CLAUDE.md`, `skills/jiho-kim-guidelines/SKILL.md` and `.cursor/rules/jiho-kim-guidelines.mdc` share one body and must stay in sync. [EXAMPLES.md](./EXAMPLES.md) has before/after examples built from real sessions.

MIT
