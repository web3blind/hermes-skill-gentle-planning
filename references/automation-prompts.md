# Automation Prompts

Use these only if the user wants scheduled check-ins, session-start reminders, or recurring reviews.

## Read is not started: optional reminder choices

A notification can be read and forgotten during another task. Do not diagnose laziness, infer a start from a read receipt, or infer failure from silence. Offer this protocol only when useful and accepted by the user:

- **Starting now**: record the user's intention to start, not completion. Show one small entry step and the latest continuation point. Cancel and verify any pending follow-up for this same session; if cancellation is unavailable, say so and ask the user to cancel it manually.
- **Later at <time>**: agree a specific date, local time and timezone. Offer one follow-up, not a new daily series. A time such as 18:00 is an example, never a global default. If today's time has passed, clarify the date rather than silently choosing tomorrow.
- **Skip today**: close this occurrence without debt or extra follow-ups. Cancel and verify any pending follow-up for this same session. Keep the previously agreed recurring rhythm unless the user asks to change it.

No reply means no decision or progress is known. It does not authorize repeated messages, automatic postponement, snoozes or escalation. After the agreed one-shot follow-up, do not generate another follow-up without a new explicit request. Repeated clicks or repeated "later" replies for the same time must not create duplicate jobs; an explicitly changed time replaces the earlier follow-up, with cancellation confirmed before claiming replacement.

### Capability and consent gate

1. Determine whether the current environment actually exposes scheduling and notification tools. A product name, subscription, prompt or uploaded TXT does not grant capabilities. Some environments offer native scheduled tasks; other chats cannot send messages later. Say when this is unknown.
2. Confirm the requested action, destination, date/time/timezone and once-only scope. Do not create a reminder, change an existing rhythm or send a test notification without permission. Confirm notification permission with the user where needed; do not claim to inspect device settings you cannot access.
3. Prefer real supported native controls if available. Offer buttons only when the integration supports their action handling, not decorative labels or permanent menus. Always keep text replies such as "Starting now", "Later at 18:00" and "Skip today" usable; an optional address prefix may be needed in group chats.
4. If a scheduler is available and the action is authorized, create/update the one-shot reminder through it. Claim it is scheduled only after a successful task receipt or visible task confirmation. Distinguish scheduled from delivered; actual delivery needs its own evidence. On an unknown outcome, inspect the existing task before retrying; never create a second job to hide uncertainty.
5. If no scheduler is available, say so and offer a manual phone/calendar reminder with the continuation point, or invite the user to return here at an agreed time. The person creates that reminder. If capability is unclear, discuss which route they can use instead of claiming a promise will execute.

The prompt itself never enables scheduling, notifications or buttons. Do not require an agent installation for the manual route. Keep reminder responses short, accessible and free of shame. On each real scheduled fire, retrieve the latest permitted checkpoint or user report if tools support it; a static task body without access to later reports must not be presented as an automatically updated checkpoint.

## Daily Close

```text
Use gentle-planning to turn this raw day report into:
1. facts,
2. planned vs done,
3. diagnosis for misses: plan, execution, constraint, or pressure,
4. carryovers,
5. one adjustment for tomorrow,
6. one thing not to chase.

Raw report:
[paste notes]
```

## Weekly Reset

```text
Use gentle-planning for a weekly reset.
Return:
1. what repeated,
2. what caused overruns,
3. whether the plan supported calm direction or created pressure,
4. what stays stable,
5. what should be reduced or replaced,
6. one main contour for next week,
7. one thing not to chase.

Notes:
[paste notes]
```

## Monthly Reset

```text
Use gentle-planning for a month reset.
Return:
1. what worked,
2. what created pressure,
3. plan/execution/constraint diagnosis,
4. one main contour for the next month,
5. supporting rhythm,
6. stop rule,
7. weekly check,
8. one thing not to chase.

Month notes:
[paste notes]
```
