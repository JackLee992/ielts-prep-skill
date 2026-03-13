# Tracking System

Use this file when the user wants an ongoing prep system rather than one-off coaching.

## Modes

Offer two tracking modes.

### Lightweight Mode

Best for:

- Users with short timelines
- Users who resist heavy note-taking
- Users who mainly need a feedback loop

Files:

- `.ielts/ERRORS.md`
- `.ielts/RULES.md`
- `.ielts/WEEKLY_REVIEW.md`

Use this by default.

### Advanced Mode

Best for:

- Users studying for 4+ weeks
- Retakers who need pattern evidence
- Users with real application or registration deadlines
- Anyone doing repeated mocks, essays, or speaking recordings

Recommended structure:

```text
.ielts/
├── profile.md
├── ERRORS.md
├── RULES.md
├── WEEKLY_REVIEW.md
├── mocks/
├── sessions/
├── essays/
└── speaking/
```

## What Each File Stores

### `profile.md`

Keep stable facts:

- test type
- exam date
- target overall and per-section scores
- real-world purpose
- current estimated level

### `ERRORS.md`

Keep repeated or high-value errors:

- what failed
- root cause
- next rule
- retest date

### `RULES.md`

Keep only rules that have already helped performance. Remove rules that are too vague to execute during the exam.

### `WEEKLY_REVIEW.md`

Use for:

- what improved
- what still breaks
- what to change next week

### `mocks/`

Store one file per mock with:

- score snapshot
- timing notes
- error clusters
- next-week drills

### `sessions/`

Store short notes when the user studies often and needs continuity:

- what was practiced
- what was learned
- what to do next

### `essays/` and `speaking/`

Use when the user repeatedly submits artifacts and wants progress over time.

## Mode Selection Rule

Choose **Lightweight Mode** when the user needs momentum and low friction.

Choose **Advanced Mode** when the user needs evidence, structure, and repeated comparison across weeks.

## Upgrade Rule

Upgrade from lightweight to advanced when any of these happen:

- 2+ mock tests completed
- 3+ weeks of prep
- repeated score plateau
- external deadline with section minimums

## Review Cadence

- Per session: note the highest-value mistake
- Per week: decide the next 1 to 3 drills
- Per mock: rewrite the next study block around the biggest score leak
