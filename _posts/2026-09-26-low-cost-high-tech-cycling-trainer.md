---
layout: post
title: "My low-cost high-tech cycling trainer"
date: 2026-09-26
excerpt: "How I wired up Enduragent, intervals.icu, and Telegram so my training plan landed directly on my Wahoo."
---
I'm an amateur cyclist and my abilities don't justify spending \$\$\$ on a professional coach, but I knew I could benefit from structured training to prepare for a long road race. I figured I'd look for an AI coach setup that I could tinker with.
## The solution
- **[Enduragent](https://github.com/yerzhansa/enduragent)** — a self-hosted AI cycling coach. It reads your actual training data and writes structured workouts. Running on my raspberry pi.
- **[intervals.icu](https://intervals.icu)** — where my rides, power data, and fitness live, and where the coach drops new workouts.
- **Telegram** — how I talk to the coach from a web and mobile interface.
## What surprised me
* The connectedness of everything was really enjoyable. Every little piece of work done by the system was energy I could put into the training itself.
* Flexibility was another strong point. Managing the workout schedule through chat was a breeze.
* It didn't use many tokens, simple calls to intervals.icu didn't rack up much of a bill. Through six weeks of training I racked up $0.15 in charges using deepseek flash 4.1.
## The result
My AI coach ran me through a typical build up consisting of base training with a few intervals before moving into consistent blocks of Sweat Spot and Tempo training. Only in the last few weeks did it give me high intensity workouts to build the top end power.
## Looking forward
While this was a good experience, I'm going to try and add these function to my local openclaw setup so that it's a bit easier to manage alongside other personal agents.



