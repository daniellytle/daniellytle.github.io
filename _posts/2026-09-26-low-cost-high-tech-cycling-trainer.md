---
layout: post
title: "My low-cost high-tech cycling trainer"
date: 2026-09-26
excerpt: "How I wired up Enduragent, intervals.icu, and Telegram so my training plan landed directly on my Wahoo."
---

I don't have a coach, and I didn't want to build my own training plan. But I did want some structure leading into my last race. So I pieced together a small stack and let an AI coach do the programming.

## The stack

Three tools, one loop:

- **[Enduragent](https://github.com/yerzhansa/enduragent)** — a self-hosted AI cycling coach. It reads your actual training data and writes structured workouts.
- **[intervals.icu](https://intervals.icu)** — where my rides, power data, and fitness live, and where the coach drops new workouts.
- **Telegram** — how I talk to the coach from my phone instead of a terminal.

The key detail for me was the sync chain. Enduragent doesn't just chat — it writes the workout to my intervals.icu calendar, and intervals.icu pushes it straight to my Wahoo. That means I never transcribe an interval session by hand. The coach says "here's your 5x3 VO2max session," and it's waiting on my head unit the next time I get on the bike.

## The loop

A typical week looked like this:

1. I ride. The Wahoo records power, HR, and the route, and uploads to intervals.icu when I get home.
2. I message the coach on Telegram — `/workout` for today, or a sentence like "my legs are dead, give me something easier."
3. The coach reads my actual numbers — FTP, recent load, fitness/fatigue/form — not a questionnaire.
4. It writes the session to my intervals.icu calendar with structured intervals and power targets.
5. intervals.icu syncs it to my Wahoo. I just show up and ride.

What I liked most was that a late meeting or a bad night of sleep didn't derail the plan. I'd message the coach that my evening was shot, and it would rewrite the session — same intent, shorter — and update the calendar before I'd even changed into kit.

## What it cost

Nothing for the tool itself. Enduragent is MIT-licensed and free, my intervals.icu data stays in intervals.icu, and the only ongoing cost is whatever my LLM provider bills for the chat. No new account, no subscription, no server holding my training history.

## The result

The plan wasn't magic — it was just consistent and specific. Structured intervals showed up on my head unit every session, aimed at the race, and I followed them. That consistency is exactly what I was missing when I was winging it week to week.

For my next race I'll run the same setup. The coach already remembers my goals, my numbers, and how the last block went — and that's more continuity than I'd managed on my own in years.
