# How it works

Family Briefing is an automation built in n8n. Each morning it gathers what's coming up and sends one short message.

```text
[Morning schedule]
      |
      v
[Shared family calendar]  +  [Weather]
      |
      v
[n8n workflow]
  - read today's and tomorrow's events
  - add a simple weather reminder
  - merge them together
  - write the message in Mrs Maggie's voice
      |
      v
[Telegram] -> the family chat
```

## A few design choices

1. **A briefing, not a database.** The message should be short enough to read in a few seconds. Success is fewer forgotten things, not more detail.
2. **Deliver where people already are.** It arrives in Telegram, the chat the family already uses, so there's nothing new to check.
3. **Simple and reliable.** It runs on a schedule with no manual steps, and it's meant to be quiet and dependable.

## The example workflow

The `examples/workflow-demo.json` file is a small, importable version of the workflow with placeholder values, so you can see the shape and wiring without it connecting to anything real. `examples/README.md` explains what's in it and how to open it.
