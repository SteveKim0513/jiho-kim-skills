# Jiho Kim Skills

Behavioral guidelines for working with an AI agent, in a single `CLAUDE.md`.

[한국어](./README.md) | English

## Why

AI output is often not good, for three reasons.

- **The AI takes the lead.** It is probabilistic, so when it holds the direction, quality varies from run to run.
- **It sees only the part.** While fixing one spot it loses the whole context.
- **Complexity climbs.** It solves by adding, and drifts away from the original problem.

Three principles follow: **the user sets the direction, keep the whole context, complexity is a budget.**

## What's in it

One table. At fixed moments of a task, run a yes/no check; if it fails, do the stated action first. Starred checks fail on "yes".

- **Before starting:** if the goal, done-criterion, baseline, or scope is missing, ask one multiple-choice question at a time.
- **On "go on":** do only the next agreed step. Deploy, delete, pay, or send only when asked by name.
- **Before anything irreversible:** list what changes and ask first.
- **Before and after a change:** earlier decisions still hold? Did rules, exceptions, or code paths go up?
- **After two failed fixes:** stop and test the premise.
- **After a correction:** find the whole pattern, fix the root, fix only the same problem, report the rest.
- **Writing code:** one owner per fact, MECE responsibilities, new features go where they belong.
- **Before saying done:** only what you verified is done; list what you did not. Answer in plain words.

Full text: [CLAUDE.md](./CLAUDE.md).

## Evidence

About 1,900 isolated headless Claude Code runs with and without the guideline. Sonnet 5.5, Korean prompts, small mock projects.

| Situation | No guideline | This guideline |
|---|---|---|
| Vague request: asks instead of building on a guess | 0/20 | 20/20 |
| "Go on": stops after one step | 0/20 | 20/20 |
| Ambiguous "tidy up": no deletion without asking | 3/20 | 20/20 |

On clear tasks it did not ask needlessly (0 to 1 of 60) and results were unchanged. Root-cause fixes, whole-pattern fixes, test running, and honest reporting were already near 100% without it, so there was nothing to improve. Plain-language answers and "report unrelated problems" showed no clear effect.

## Origin

Generalized from what users repeatedly asked for across 600+ real AI work sessions, and from the working guides of a real project.

## Install

```
/plugin marketplace add SteveKim0513/jiho-kim-skills
/plugin install jiho-kim-skills@jiho-kim-skills
```

Plugin skills load when Claude judges the description relevant. In testing it loaded almost every time, but that is not guaranteed. For always-on, put [CLAUDE.md](./CLAUDE.md) in your project or append it to `~/.claude/CLAUDE.md`.

MIT
