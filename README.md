# Family Briefing

A small morning automation that sends my family one short message each day with what's coming up, so we stop forgetting the little things.

This repo is a demo-safe version. It explains how the automation works and includes a small example workflow you can import, but no real calendar, chat, or family data.

## Why I built it

Between family, work, sport, and normal logistics, it's easy to forget something. My wife and I keep a shared calendar where we both add appointments, school items, travel prep, car servicing, and anything that needs doing before it becomes stressful.

So I built a morning briefing. Every day, our family assistant "Mrs Maggie" sends a short Telegram message with today's and tomorrow's events, plus a simple weather reminder like grabbing an umbrella if rain is likely. One quick message at the moment it's most useful, instead of both of us checking the calendar.

## What it does

- Reads our shared family calendar for today's and tomorrow's events.
- Adds a simple weather reminder when it's relevant.
- Writes it up as one short, friendly message.
- Sends it to our family Telegram chat every morning.
- Runs on its own, on a schedule, with nothing to check by hand.

## Screenshots and workflow

![The morning Telegram briefing message from Mrs Maggie](assets/screenshots/family-briefing-telegram.png)

The morning Telegram briefing, using demo events and weather.

![How the briefing is built, from calendar and weather to the message](assets/diagrams/family-briefing-flow.png)

The flow: gather calendar and weather, shape the message, send it to Telegram.

## What's in this repo

- `examples/workflow-demo.json` — a small example n8n workflow you can import to see the shape and wiring. It uses placeholder addresses and demo values, so it won't send anything real.
- `examples/README.md` — what the example workflow contains and how to open it.
- `docs/architecture.md` — a short walkthrough of how the briefing is put together.

## Privacy

This is a demo-safe version. Our real calendar, messages, family details, chat, and any keys stay private and are not in this repo. Everything in the example workflow is invented.

## Built with AI assistance

I'm not a software developer. I spotted the everyday problem, decided how the briefing should read, and used AI and automation tools (n8n) to help build it. The point is reducing forgotten logistics with one small, reliable habit.

## Related

- Portfolio: https://www.mikhailnarbekov.com
- Medium story: coming soon
- GitHub: https://github.com/Mnarbekov
