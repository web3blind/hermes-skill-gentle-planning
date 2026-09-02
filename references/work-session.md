# Work Session

Use when the user wants to start or contain a focused work block.

## Rules

- The assistant can define the next step and stop point.
- The user keeps the timer unless a real scheduling/reminder tool is configured.
- A session should begin with one visible task, not a full life plan.
- If the user pauses, preserve the state in the current chat.

## Start Template

```text
Session focus: <task>
First step: <2-10 minute entry>
Done when: <criterion>
Stop at: <time/condition>
If interrupted: <how to resume>
```

## Progress Responses

If the user says "done":
- mark the block complete;
- choose the next block or stop.

If the user says "pause":
- summarize where they stopped;
- give one resume line.

If the user says "not done":
- preserve useful progress;
- choose whether to continue, shrink, or carry over.
