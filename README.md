# Gentle Planning

A shareable Hermes Agent skill for calm, sustainable planning without turning productivity into pressure.

It helps an AI assistant guide a user through realistic day plans, weekly resets, monthly reviews, focused work sessions, factual reviews, stop rules, and carryover decisions.

## What it is for

Use Gentle Planning when a user wants:

- a plan for today without overloading themselves;
- a weekly or monthly reset;
- a focused work session with a clear stop point;
- a review that separates facts, constraints, and choices;
- a lighter fallback plan for low-energy days.

It is designed for people who want structure, but do not want a rigid productivity system.

## Install

Clone or copy this repository into your Hermes skills directory:

```bash
mkdir -p ~/.hermes/skills/productivity
git clone https://github.com/web3blind/hermes-skill-gentle-planning.git ~/.hermes/skills/productivity/gentle-planning
```

If your Hermes setup supports installing skills from a GitHub/raw URL, use the raw `SKILL.md` URL after the repository is published:

```text
https://raw.githubusercontent.com/web3blind/hermes-skill-gentle-planning/main/SKILL.md
```

## Files

- `SKILL.md` — main trigger, workflow, pitfalls, and verification checklist.
- `references/day-planning.md` — realistic day plan template.
- `references/week-planning.md` — weekly reset template.
- `references/month-reset.md` — monthly reset template.
- `references/work-session.md` — focused work session flow.
- `references/review.md` — factual review format.
- `references/automation-prompts.md` — optional recurring prompt examples.

## Example prompts

```text
Use gentle-planning to help me plan today without overloading myself.
```

```text
I have one hour and too many tasks. Help me choose the first work session.
```

```text
Use gentle-planning to review this week and decide what to reduce next week.
```

```text
Run a monthly reset from these notes. Keep it realistic and calm.
```

## Safety and scope

This is not therapy, medical advice, legal advice, or financial advice. It is a planning and review workflow.

The skill avoids:

- shame-based discipline;
- fake motivation;
- over-detailed plans for tired users;
- treating unfinished work as moral failure;
- turning rest into a reward that must be earned;
- creating recurring reminders without explicit user consent.

## License

MIT
