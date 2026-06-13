# Example workflow

This folder has a small, made-up version of the Family Briefing workflow so you can see how it's wired together. It uses placeholder addresses and demo values, so it won't connect to anything real or send any messages.

## What's in `workflow-demo.json`

A small n8n workflow with six steps:

1. A schedule trigger that runs in the morning.
2. Read the shared calendar for today and tomorrow (points at a placeholder address).
3. Fetch the weather (same placeholder pattern).
4. Merge the calendar and weather together.
5. Write the morning message in Mrs Maggie's voice. In the real workflow this step calls an AI model; here it returns a fixed example message.
6. Send the message to Telegram, using a demo chat value.

## How to open it

Import `workflow-demo.json` into any self-hosted n8n instance and you'll see the layout and how the steps connect. It won't produce real output, because it has no real calendar, weather, or Telegram credentials — and on purpose, no keys or tokens are stored in the workflow file.

All the values in this file are invented for the demo. The placeholder addresses use the reserved `example.invalid` domain, which never resolves.
