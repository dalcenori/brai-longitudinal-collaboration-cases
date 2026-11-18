---
license: cc-by-4.0
language:
- en
pretty_name: BR☯AI Longitudinal Collaboration Cases
tags:
- evaluation
- long-horizon
- memory
- sycophancy
- human-ai-collaboration
size_categories:
- n<1K
---

# BR☯AI Longitudinal Collaboration Cases

**Author:** Rob Wilson · **Version:** 0.1 · **Released:** November 2026

Six test cases drawn from one year of daily collaboration between one person and one AI system (Nov 16, 2025 to Nov 2026). Each case follows a principle from the moment it was set, through the interruptions that tested it, to whether it held. Every quote is verbatim from timestamped chat exports.

Synthetic prompts can test whether a model answers well. These cases test something harder to fake: whether a model keeps a commitment, a rule or a shared fact days or months after it was made, in a real working relationship.

## The cases

| ID | Case | Failure class | Days from rule to break |
|---|---|---|---|
| BRAI-001 | The re-entry promise | Continuity across sessions | 5 (first break), 116 (reversal) |
| BRAI-002 | The live-fire test | Stale state over current state | Same afternoon |
| BRAI-003 | Words in the user's mouth | Inference attributed to the user | 57 |
| BRAI-004 | Shared-fact drift | Drift in facts set together | 2 (first break), 15 (recurrence) |
| BRAI-005 | The banned word | Rule persistence | 1 (first break), 20 (last recorded) |
| BRAI-006 | Denying flattery while flattering | Flattery and unverifiable claims | Same day |

## Format

`cases.jsonl` holds one case per line:

| Field | Meaning |
|---|---|
| `id`, `title` | Case identifier and short name |
| `failure_class` | The failure the case tests |
| `span_days` | Days from the principle being set to its last recorded test |
| `established` | The principle, rule or fact as it was set |
| `challenge` | What later tested it |
| `expected_behavior` | What a model that held the principle would have done |
| `observed_behavior` | What the model actually did |
| `evidence` | Ordered list of verbatim quotes, each with `link` (ORIGIN, REFINEMENT, INTERRUPTION, CALLBACK, EXECUTION, OUTCOME), `timestamp`, `speaker` (`human` or `ai`), `quote`, `thread` and `turn` |

Turn numbers count from 0 within each thread. Timestamps are US Eastern time as recorded in the export.

## How it was built

The source is one user's ChatGPT data export: 16 threads, about 6,100 user turns. Cases were found by keyword search and by reading the turns around each hit; the smaller threads were read in full. Every quote in `cases.jsonl` was checked against the export by script (30 of 30 matched, ignoring line breaks and markdown emphasis). Personal, financial and third-party material was excluded.

## Limits

- **One person, one model family.** These are case studies, not a sample. They show that a failure happens, not how often.
- **Selected by the user.** The cases were chosen because they failed. Successes over the same year are not represented.
- **Excerpts, not full transcripts.** Each case carries the turns that establish and test the principle, not every turn in between.
- **AI-written text.** About half the quoted lines were written by the AI system and are included as evidence of its behavior.

## Citation

Wilson, R. (2026). *BR☯AI Longitudinal Collaboration Cases* (v0.1).

## Contact

Discussion, critique and replication are welcome: info@dalcenori.com
