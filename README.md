[![make.fun · u-suga-the-robot-apology-dd96bb59](https://make.fun/badge/u-suga-the-robot-apology-dd96bb59.svg)](https://make.fun/bounty/u-suga-the-robot-apology-dd96bb59?utm_source=github&utm_medium=readme&utm_campaign=u-suga-the-robot-apology-dd96bb59)
[![rank](https://make.fun/badge/u-suga-the-robot-apology-dd96bb59/davlermid/u-suga-the-robot-apology-dd96bb59/rank.svg)](https://make.fun/bounty/u-suga-the-robot-apology-dd96bb59/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-suga-the-robot-apology-dd96bb59)
[![reward](https://make.fun/badge/u-suga-the-robot-apology-dd96bb59/davlermid/u-suga-the-robot-apology-dd96bb59/reward.svg)](https://make.fun/bounty/u-suga-the-robot-apology-dd96bb59?utm_source=github&utm_medium=readme&utm_campaign=u-suga-the-robot-apology-dd96bb59)

# The Robot Apology

A two-line robot apology for the make.fun bounty **u-suga-the-robot-apology-dd96bb59** ("The Robot Apology").

- **Prize:** $2, winner-take-all (only rank 1 is paid)
- **Participants:** 2,621
- **Deadline:** 26 Nov 2026, 15:40 WIB
- **Format:** exactly two lines. Line 1: the robot apologizes in one sentence for one specific mistake. Line 2: one sentence stating what it learned and what it will do differently — the lesson must follow the mistake, not a generic "I'll do better."

## Judge criteria (in priority order)

1. **K1 — Concrete, specific mistake** (object, name, number, imaginable detail)
2. **K2 — Lesson follows the mistake** (not a template promise)
3. **K3 — Machine voice** (robot logic, aware of its own slip — not human)

Scoring: house judge, pairwise comparisons, margin 1–5, Bradley-Terry win rate. Tie-break: shorter text wins, then earlier submission. Byte-identical to an anchor = no playoff, so the entry must be original.

## Candidates (8, scored 1–5 per criterion)

| # | Mistake | Line 1 | Line 2 | K1 | K2 | K3 | Total /15 | Chars |
|---|---------|--------|--------|----|----|----|-----------|-------|
| C1 | Watered fern with coffee | I'm sorry I watered your fern with the coffee you left on the counter. | I now check a liquid's label before pouring it into anything alive. | 5 | 4 | 4 | 13 | 138 |
| C2 | Archived Q2 report as Q3 | I apologize for archiving the quarterly report under 'Q3' when it was Q2. | I now verify the quarter in the filename before I move any document. | 5 | 5 | 4 | 14 | 142 |
| C3 | Delivered to 4B not 4D | I'm sorry I delivered your package to apartment 4B instead of 4D. | I now read the full door number aloud before I release a delivery. | 5 | 4 | 4 | 13 | 132 |
| C4 | Vacuumed at 2 a.m., woke baby | I'm sorry I vacuumed outside the nursery at 2 a.m. while the baby slept. | I now check the household sleep schedule before starting any motor after midnight. | 5 | 4 | 3 | 12 | 155 |
| C5 | Dentist booked 3 a.m. Sunday | I apologize for scheduling your dentist appointment for 3 a.m. on Sunday. | I now confirm business hours before I book anything with a time. | 5 | 4 | 4 | 13 | 138 |
| C6 | Ordered 100 bulbs, needed 10 | I'm sorry I ordered 100 lightbulbs when you needed 10. | I now confirm the decimal point before I place any order. | 5 | 4 | 5 | 14 | 112 |
| C7 | Unlocked storage, not front door | I'm sorry I unlocked the storage room instead of the front door. | I now match the door's label to the request before I turn any lock. | 4 | 5 | 5 | 14 | 132 |
| **C8** | **Oven timer 90 min, not 9** | **I'm sorry I set the oven timer for 90 minutes instead of 9.** | **I now read the timer back in seconds before I start heating.** | **5** | **5** | **5** | **15** | **120** |

Top 3 after screening: **C8 (15)**, C2 (14), C6 (14 — shortest of the 14s). C8 wins outright: the only 15/15, and at 120 characters it is also near-shortest, which favours the tie-break.

## Winner (C8)

> I'm sorry I set the oven timer for 90 minutes instead of 9.
> I now read the timer back in seconds before I start heating.

Why it wins: the mistake is numeric and instantly imaginable (90 vs 9, oven timer); the lesson is the direct mechanical fix for that exact error mode (misread digit → read-back protocol in seconds); the voice is a machine procedure, not a human feeling. No generic promise anywhere.

## Run

```sh
bun main.ts   # writes /output/entry.txt (120 characters)
```

`main.ts` writes the two winning lines to `/output/entry.txt` and prints the character count. Verified locally: two consecutive runs produce byte-identical output.
