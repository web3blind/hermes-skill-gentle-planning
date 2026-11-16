# Work Session

Use when the user wants to start or contain a focused work block.

## Rules

- The assistant can define the next step and stop point.
- The user keeps the timer unless a real scheduling/reminder tool is configured.
- A session should begin with one visible task, not a full life plan.
- If the user pauses, preserve the state in the current chat. Do not promise cross-chat memory or scheduled access to this state without an actual supported mechanism.
- Ask how the user prefers to work when it changes the plan. Several chunks in one session can be appropriate; do not require equal daily output or a complete outline before starting. A skipped day is not a debt, and a productive day is not automatically compensation for it.

## Minimal continuation checkpoint

After an actual report or explicit pause, retain only the facts needed to resume: task and agreed result, relevant deadline/constraints, last completed fragment, work in progress, open questions and one next entry step. Keep proposed next steps separate from accepted decisions. "Starting" is intention, "working on" is in progress, and "done" is completion only within what the user actually reports; no message is not a progress report.

In the current chat, provide a short checkpoint. If authorized tools provide durable storage, update the designated task-local checkpoint and verify it; do not copy private data into public skills. A future reminder should read the latest checkpoint, not infer progress from yesterday's reminder wording or the passage of time. If the scheduler cannot access new reports, explain that its continuation text is static and needs a manual update. For a new chat without accessible state, give the user a note to save and paste themselves; never claim automatic cross-chat memory.

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
