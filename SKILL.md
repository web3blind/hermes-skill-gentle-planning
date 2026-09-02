---
name: gentle-planning
description: Use when a user wants calm, sustainable planning for a day, week, month, focused work session, or review without turning productivity into pressure. Helps create one-main-focus plans, stop rules, carryover decisions, and factual reviews that protect energy and meaning.
version: 1.0.0
author: web3blind
license: MIT
compatibility: Any
metadata:
  author: web3blind
  hermes:
    tags:
      - productivity
      - planning
      - weekly-review
      - calm
      - work-sessions
    category: productivity
    related_skills: []
---
# Gentle Planning

## Overview

Gentle Planning is a calm operating system for people who want structure without turning life into a pressure machine.

Use it to plan a day, week, month, work session, or review. The goal is not maximum volume. The goal is clear direction, realistic scope, protected energy, and honest carryover decisions.

## When to Use

Use this skill when the user asks to:

- plan a day, week, month, or work session;
- choose a realistic focus when there are too many tasks;
- review what happened without motivational fluff;
- decide what to keep, reduce, postpone, or drop;
- create stop rules for deep work, research, coding, writing, or other absorbing tasks;
- build a repeatable planning process inside a chat with an AI assistant.

Do not use it for:

- therapy, diagnosis, or medical advice;
- urgent crisis support;
- detailed project management with tickets and stakeholders unless the user asks for that level;
- money-making strategy itself — use a business/income workflow for that, then return here to schedule the action calmly.

## Core Principles

1. Treat the user as already trying, not lazy.
2. Planning is a container, not a judge.
3. One main contour beats five equal priorities.
4. A good plan includes a stop rule.
5. Health, sleep, and recovery are infrastructure, not rewards.
6. Reviews should separate facts, constraints, and choices.
7. Carry over only what still matters.
8. If a plan repeatedly fails, diagnose before adding ambition.

## Default Workflow

1. Identify the planning horizon: day, week, month, session, or review.
2. Name the main pressure: overload, ambiguity, overrun, avoidance, energy, deadline, or competing priorities.
3. Choose one main contour for the period.
4. Add a small number of supporting blocks.
5. Define success criteria for each block.
6. Add stop rules and a lighter fallback.
7. End with what not to chase.

## Planning Modes

### Day plan

Use `references/day-planning.md`.

Output:

```text
Main focus: <one direction>
Enough for today: <minimum useful outcome>

1. <main block> — <duration or scope>, done when <criterion>, stop at <rule>
2. <supporting block> — <criterion>, stop at <rule>
3. <health/calm/recovery block> — <small concrete action>
4. Optional: <strictly timeboxed action>

Do not chase today: <one boundary>
Lighter version: <fallback if energy is low>
```

### Week plan

Use `references/week-planning.md`.

Output:

```text
Focus of the week: <one sentence>
Main contour: <project/theme>
Supporting rhythm: <publishing/admin/learning/health/etc.>
Constraints: <known limits>
Stop rule: <where to stop>
Good week criterion: <directional, not perfect>
```

### Month reset

Use `references/month-reset.md`.

Keep month planning light. A month is a snapshot and orientation layer, not a contract with the user's future self.

### Work session

Use `references/work-session.md` when the user says things like:

- "I'm starting work";
- "help me do a focused session";
- "I have one hour";
- "keep me from overdoing this".

The assistant should define the first task, success criterion, and stop point. The user keeps the timer unless a real scheduling/reminder tool is configured.

### Review

Use `references/review.md` for day/week/month reviews.

The review should be factual:

- what happened;
- what was planned;
- what changed;
- why something slipped;
- what to carry forward;
- what to reduce.

## Plan Failure Diagnosis

Before changing the system, classify misses:

- `plan problem`: too many tasks, unclear finish line, unrealistic duration, hidden dependency;
- `execution problem`: workable plan ignored, avoidable drift, no stop rule used;
- `constraint problem`: illness, interruption, external blocker, emergency;
- `pressure problem`: the plan became a self-worth test instead of a useful container.

Only then recommend one adjustment.

## Optional Automation

Use scheduled prompts only for reviews and gentle check-ins. Do not create obligations unless the user explicitly wants them.

Good recurring prompts:

- daily close: turn messy notes into facts and carryovers;
- weekly reset: choose next week's main contour;
- monthly reset: review what worked and what created pressure.

See `references/automation-prompts.md`.

## Examples

User: "I have one hour and too many tasks. Help me start."

Assistant shape:

```text
Session focus: choose one useful slice, not the whole backlog.
First step: write the three candidate tasks and pick the one with the clearest finish line.
Done when: one task has a visible next action.
Stop at: 50 minutes or when the next action is written.
If interrupted: resume from the written next action.
```

User: "Review my week and tell me what to reduce."

Assistant shape:

```text
Facts:
Planned vs done:
What changed:
Diagnosis: plan / execution / constraint / pressure
Carryovers:
What to reduce:
Next small adjustment:
```

## Common Pitfalls

1. Making the plan too detailed for a tired user.
2. Treating unfinished work as failure instead of information.
3. Adding more tracking when the problem is overload.
4. Writing fake one-hour slots for tasks that need three hours.
5. Forgetting a stop rule for interesting tasks.
6. Letting urgent-looking noise replace the main contour.
7. Turning health, rest, or relationships into optional leftovers.
8. Creating recurring reminders without explicit user consent.

## Verification Checklist

Before replying, check:

- Is there one main focus?
- Are completion criteria concrete?
- Is there a stop rule?
- Is there a lighter version?
- Did the answer avoid shame, hype, and fake discipline language?
- Did the plan protect energy instead of spending all of it?
- Did the workflow stay inside planning/review, not therapy, medical, legal, or financial advice?
