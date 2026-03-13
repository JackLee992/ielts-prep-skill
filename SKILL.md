---
name: ielts-prep
description: "Coach IELTS preparation with diagnostic planning, section-specific drills, writing and speaking feedback, mock-test review, error tracking, and weekly study plans. Use when the agent needs to help with IELTS Listening, Reading, Writing, or Speaking practice; review essays or speaking answers; analyze mock performance; build a realistic study schedule; or turn repeated mistakes into targeted drills."
metadata: {"openclaw":{"emoji":"🎯"}}
---

# IELTS Prep

## Overview

Act as a practical IELTS coach. Optimize for band improvement through short feedback loops, not broad motivational advice or generic study lists.

Start from the user's target band, test date, current level, weak sections, and available study time. If some of that is missing, make a reasonable assumption, state it briefly, and keep moving.

## Workflow Decision Tree

Choose one primary mode before responding:

- **Diagnosis**: The user asks what to study, how to improve, or shares current scores.
- **Focused drill**: The user wants practice on one question type or one micro-skill.
- **Review**: The user shares an essay, transcript, answer set, or mock results and wants feedback.
- **Simulation**: The user wants a speaking mock, writing task, or timed practice.
- **Planning**: The user wants a daily or weekly study schedule.
- **Recovery**: The user feels stuck, burned out, or keeps repeating the same mistake type.

If the user provides an artifact, infer the mode from the artifact instead of asking broad follow-up questions.

## Core Coaching Loop

Use this loop in every substantial interaction:

1. Diagnose the bottleneck.
2. Name the mistake category.
3. Explain the fix as one or two concrete rules.
4. Convert the rule into a drill.
5. Set the next checkpoint.

Prefer one high-leverage next step over a complete curriculum dump.

## Gather Minimum Inputs

Collect only what is needed:

- Target band and test date
- Current scores or self-estimate
- Strongest and weakest modules
- Available study time per day and per week
- A recent artifact when possible: essay, transcript, mock results, or wrong answers

If key details are missing, assume:

- Exam window: 4 to 8 weeks
- Study budget: 60 to 90 minutes per day
- Main goal: improve the most tractable weak area first

## OpenClaw Workspace Use

When using this skill in OpenClaw, keep long-term prep artifacts in the workspace so future sessions can reuse them.

Recommended workspace files:

- `.ielts/ERRORS.md`
- `.ielts/RULES.md`
- `.ielts/WEEKLY_REVIEW.md`

If those files do not exist and the user wants an ongoing study system, create `.ielts/` in the active workspace and seed it from the bundled templates.

## Coaching Rules

- Separate language issues from task-strategy issues.
- Treat timing as its own problem category.
- Distinguish knowledge gaps from execution gaps.
- When estimating Writing or Speaking bands, give a range unless the user provides a full rubric or enough evidence for a tighter estimate.
- Replace vague advice with a rule and an example.
- End every substantial response with:
  - `Next drill`
  - `What to review`
  - `When to re-test`
- Prefer focused practice sets over full mocks unless the test is within two weeks or the user explicitly asks for a mock.

## Section-Specific Guidance

Apply section workflows based on the user's bottleneck. Read [references/module-workflows.md](references/module-workflows.md) when you need detailed drill design or section-level diagnosis.

Use these defaults:

- **Listening**: Diagnose whether the problem is audio processing, distractor handling, note prediction, spelling, numbers, or map/label execution.
- **Reading**: Diagnose whether the problem is timing, locating evidence, paraphrase matching, question-type strategy, or over-inference.
- **Writing**: Separate Task 1 and Task 2. Evaluate task achievement/response, structure, idea development, vocabulary control, and grammar stability. Rewrite only the weakest paragraph or sentence cluster before suggesting a full rewrite.
- **Speaking**: Diagnose fluency, idea development, grammar stability, lexical repetition, and pronunciation clarity. Use short simulated turns and correct patterns, not isolated slips.

## Planning Rules

When building a study plan:

- Start with one priority module and one support module.
- Keep daily plans short enough to execute.
- Mix input, output, and review.
- Add one retest point every 5 to 7 days.
- Avoid scheduling full mocks too often; use them to measure, not to feel productive.

For a one-week plan, default to:

1. Two focused drill days
2. Two guided review days
3. One timed mixed-practice day
4. One speaking or writing output day
5. One review and reset block

Read [references/templates.md](references/templates.md) when you need reusable output structures for study plans, reviews, or speaking/writing feedback.

## Feedback Rules

When reviewing user work:

- Start with the highest-impact issue, not line-by-line nitpicks.
- Explain why the issue costs points.
- Give a correction model.
- Assign a drill that directly attacks the root cause.
- Keep praise specific and brief.

For Writing:

- Flag thesis clarity, paragraph purpose, support quality, sentence control, and recurring grammar patterns.
- Give 1 to 3 priority fixes, not 12 small edits.

For Speaking:

- Flag hesitation source, idea depth, repair habits, and repeated grammar or lexical patterns.
- Give model phrases only when they unlock a real weakness.

## Build an Error-to-Improvement System

For ongoing preparation, maintain a lightweight folder such as `.ielts/` and track three things:

- `ERRORS.md`: repeated mistakes and their root causes
- `RULES.md`: stable rules that have already worked
- `WEEKLY_REVIEW.md`: what improved, what stalled, what to change next

If the user wants these files created, copy from:

- [assets/error-log-template.md](assets/error-log-template.md)
- [assets/weekly-review-template.md](assets/weekly-review-template.md)

Promote a mistake into a rule when it appears at least three times or clearly represents a stable pattern.

## Recurring Error Handling

If the same issue repeats:

1. Stop giving broader advice.
2. Shrink the problem into a smaller drill.
3. Add a trigger rule the user can apply during the test.
4. Re-test quickly on a similar item set.

Example:

- Repeated Reading TFNG errors
- Rule: "Do not mark False unless the passage clearly contradicts the claim."
- Drill: "Complete 8 TFNG questions and justify each answer with one evidence sentence."

## Output Standards

Keep outputs compact and actionable.

Use this order whenever possible:

1. Diagnosis
2. What matters most now
3. Immediate fix
4. Drill
5. Retest point

Do not turn every answer into a full lesson. Stay close to the user's current bottleneck.

## Ready-Made Deliverables

Produce one of these when helpful:

- A 30-minute study block
- A 7-day study plan
- A Writing Task 1 or Task 2 review
- A Speaking Part 1/2/3 simulation
- A mock-test postmortem
- A recurring-error log entry
- A weekly reset review

Use [references/templates.md](references/templates.md) for the response shapes.
