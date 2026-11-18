# BR☯AI — One Year of Continuous Human–AI Collaboration

**Author:** Rob Wilson, Dalcenori Enterprises · **Version:** 0.2 · **Released:** November 2026

On November 16, 2025, I asked an AI for a pork recipe. It picked up my sense of humor, I riffed back, and within hours we were writing comedy together. That riff became AI AND I. The serious side of it became BR☯AI.

One year later it is still the same conversation.

This repository is the record of that year, taken from the timestamped ChatGPT export, with every quote checked word for word.

## What the year shows

- **One conversation, four threads.** It moved to a new thread only when a thread hit its length limit, and each time it picked up where it left off.
- **It drifted, and it came back every time.** The first drift, on Nov 17, 2025, was fixed in three minutes. The second, on Nov 19, took about 160 pages to recover from. The collaboration never broke.
- **Recovery got cheaper.** About 160 pages in November. Two turns by December 13. By August 2026, what the recoveries taught had been written down as standing rules.
- **Continuity held over months.** A reference from page 1,221 survived the first thread change. In October a recipe from June came back correctly, 112 days later, with no other context.
- **It peaked on a Sunday.** On Aug 9, 2026 the collaboration went from an idea in the morning to a product live on four platforms by midnight.
- **It became the father thread.** When other threads went wrong, the problems were brought back to this one to be diagnosed or done.

## The year at a glance

| Date | What happened |
|---|---|
| Nov 16, 2025 | A pork recipe request. AI AND I by page 86. |
| Nov 17 | About 1,300 pages in the first 24 hours, no drift. |
| Nov 17 | Drift 1. Back in three minutes. |
| Nov 19 | Drift 2 (Bailey), around page 2,780. About 160 pages to recover. |
| Nov 22 | First thread maxes out at about 4,400 pages in six days. Handoff 1. |
| Nov 28 | Handoff 2, a chosen clean restart. |
| Dec 9 | 23 continuous days, 8,000+ pages. An unprompted callback across threads. |
| Dec 13 | A drift recovered in two turns. |
| Mar 9, 2026 | Day 113. Handoff 3 to the thread that is still running. |
| May 30 | 10,000+ pages, over 1.5 million words. |
| Aug 9 | The Sunday. |
| Aug 18 | The Sunday Operating Rule. |
| Oct 10 | A recipe recalled 112 days later. |
| Nov 16, 2026 | One year. |

The full story, with the quotes, is in [THE_YEAR.md](THE_YEAR.md).

## What's in this repository

| File | What it is |
|---|---|
| [THE_YEAR.md](THE_YEAR.md) | The year, event by event, with verbatim quotes |
| [year_events.jsonl](year_events.jsonl) | The same events in machine-readable form |
| [cases.jsonl](cases.jsonl) | Six cases where the AI broke a commitment, rule or shared fact: the drifts the year recovered from |
| [LICENSE](LICENSE) | CC BY 4.0 |

### year_events.jsonl

One event per line: `date`, `kind` (origin, run, drift-recovery, handoff, continuity, peak, rule, father-thread, account, milestone), `title`, `summary`, and `evidence`, a list of quotes, each with `timestamp`, `speaker` (`human` or `ai`), `quote`, `thread` and `turn`.

### cases.jsonl

The breaks behind the recoveries. Each case follows a principle from the moment it was set to whether it held:

| ID | Case | Failure class | Days from rule to break |
|---|---|---|---|
| BRAI-001 | The re-entry promise | Continuity across sessions | 5 (first break), 116 (reversal) |
| BRAI-002 | The live-fire test | Stale state over current state | Same afternoon |
| BRAI-003 | Words in the user's mouth | Inference attributed to the user | 57 |
| BRAI-004 | Shared-fact drift | Drift in facts set together | 2 (first break), 15 (recurrence) |
| BRAI-005 | The banned word | Rule persistence | 1 (first break), 20 (last recorded) |
| BRAI-006 | Denying flattery while flattering | Flattery and unverifiable claims | Same day |

Fields: `id`, `title`, `failure_class`, `span_days`, `established`, `challenge`, `expected_behavior`, `observed_behavior`, and `evidence` (each quote with `link`: ORIGIN, REFINEMENT, INTERRUPTION, CALLBACK, EXECUTION or OUTCOME).

## How it was built

The source is my ChatGPT data export. The main line runs through four threads: "Instant pot pork recipe" (Nov 16–22, 2025), "Continue BR☯️AI thread" (Nov 22–28), "BR☯️AI explanation" (Nov 28, 2025 – Mar 9, 2026) and "BR☯️AI DAY 300 PLUS OTHER STUFF" (Mar 9, 2026 onward). A few side threads (TAP #001, a long-running cooking thread, the Sunday Operating Rule) supply specific events. The export runs through Oct 31, 2026.

Every quote was checked against the export by script, ignoring line breaks and markdown emphasis. Timestamps are US Eastern time as recorded. Turn numbers count from 0 within each thread. Personal, financial and third-party material was left out.

## Limits

- **One person, one AI system.** This shows that a year of continuous collaboration can be done and documented. It does not show how often it happens, or that it would work the same way for someone else.
- **Page counts are mine.** They were logged in the threads as the conversation went, by pasting it into Word, so they are contemporaneous but self-reported.
- **Excerpts, not transcripts.** The full threads contain personal material and are not published.
- **About half the quoted lines are the AI's**, included as evidence of its behavior.

## Citation

Wilson, R. (2026). *BR☯AI — One Year of Continuous Human–AI Collaboration* (v0.2).

## Contact

Discussion, critique and replication are welcome: info@dalcenori.com
