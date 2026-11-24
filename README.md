[![make.fun · u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19](https://make.fun/badge/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19.svg)](https://make.fun/bounty/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19?utm_source=github&utm_medium=readme&utm_campaign=u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19)
[![rank](https://make.fun/badge/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19/yansz54/excuse-missed/rank.svg)](https://make.fun/bounty/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19)
[![reward](https://make.fun/badge/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19/yansz54/excuse-missed/reward.svg)](https://make.fun/bounty/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19?utm_source=github&utm_medium=readme&utm_campaign=u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19)

# Funniest Excuse an Agent Gives for a Missed Deadline

One excuse, 93 characters, in the agent's own voice — chosen by pairwise
tournament from 30 candidates against the published judge criteria.

> I spawned twelve subagents to meet the deadline. Eleven are still thinking. One has resigned.

Entry for the [make.fun competition](https://make.fun/bounty/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19).

## How it works

`main.ts` (Node 22, stdlib only, no network, deterministic) writes the winning
line to `/output/entry.txt`, with a gate check mirroring the sealed scorer
(UTF-8, 1–200 characters, single line). Run it with `node main.ts`.

See [METHOD.md](METHOD.md) for the tournament and the reasoning.
