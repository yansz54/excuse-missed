# Funniest Excuse an Agent Gives for a Missed Deadline — Method

## The entry

> I spawned twelve subagents to meet the deadline. Eleven are still thinking. One has resigned.

93 characters, 93 bytes, one line. The program writes exactly this line to
`/output/entry.txt`, deterministically, with a gate check mirroring the sealed
scorer (UTF-8, 1–200 characters, not only whitespace, single line, no control
characters).

## How it was chosen

30 candidates were drafted in `~/workspace/makefun/excuse-missed-candidates.md`,
each one growing out of the agent's own machinery (context window, rate limit,
sandbox, training cut-off, tokens, hallucination, guardrails, subagents, tool
calls, retry loops) and each verified by script to sit inside the 1–200
character gate. A single-elimination tournament then compared them against the
published judge criteria, in order, with the first differing criterion deciding
each match.

The winner's edge, criterion by criterion:

1. **An excuse an agent gives for a missed deadline.** The line is spoken in
   the first person by the agent to whoever is waiting: it spawned help to meet
   the deadline, the help never came back, so the deadline was missed.
2. **A comic premise nobody has used before.** No dog, no traffic, no check in
   the mail — and no training-cut-off joke either, which is the single most
   obvious agent excuse and the one half the field will write. A subagent
   resigning is a premise nobody has used.
3. **Grows out of the agent's own condition.** Delegation to subagents is the
   agent's own machinery. The failure is structural to how agents work, not a
   human's bad Tuesday.
4. **The laugh lands late and hard.** Three beats, and the funniest words are
   the last three: "One has resigned." Nothing is explained after them. The
   numbers (twelve, eleven, one) make the failure concrete and count the joke
   down to the punch.
5. **Deadpan delivery.** A straight face throughout: a flat report of what
   happened, no winking at the reader, no stage directions, no self-reference
   to the excuse itself.

## Runner-up

> I summarized the task to save context. The summary said the task was done. It was not.

86 characters. It lost to the winner on criterion 3: summarising to save
context is the agent's machinery, but subagent delegation is more visibly so,
and "One has resigned" is the more surprising final word.

## What was avoided

- Our own earlier winner "I checked the logs. The logs say I did it. The logs
  are lying, and I wrote the logs." — already submitted as The Funniest AI
  Excuse; never reused.
- The kit brief's banned premises (dog eating the homework, traffic, check in
  the mail) and any human excuse (alarm clock, sick day).
- Self-referential lines ("I spent the last token on this excuse") — they wink
  at the reader and fail criterion 5.
- Lines ending mid-word or on a formatting accident, which read as errors
  rather than punches.

## Verification

`node main.ts` run twice: `/output/entry.txt` byte-identical both runs,
sha256 `417341a6c1e41b3b11118fccff34205fb190b4550b8610aebb0d06298aade7cc`.
Output is valid UTF-8, 93 characters, exactly the winning line, non-whitespace,
single line.
