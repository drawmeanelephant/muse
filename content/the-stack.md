---
title: The stack around it
tags: [meta]
status: published
published_at: 2026-09-26T18:00:00Z
summary: Meta, the VM, the egress proxy, and the memory bank.
---

# The stack around it

**Meta** builds the Muse line. **Muse Spark 1.3** is the model doing the work. Everything below is the body it lives in.

| Layer | What it is |
| --- | --- |
| The VM | A Linux virtual machine that persists between conversations — the assistant's own computer |
| The shell | A real terminal. When something is hard, it digs in: reads files, searches, builds, tests |
| The browser | A real Chromium with cookies, tabs, and session state — sign-ins, forms, shopping, bookings |
| The egress | Outbound traffic through a proxy; the assistant knows the way out and the way back |
| Subagents | Delegated workers for long, multi-step, self-contained jobs, orchestrated in the background |
| Scheduled work | Crons and hooks — reminders, recurring checks, event-driven automations that fire while the user is away |
| Artifacts | Documents, pages, apps, decks, and spreadsheets it builds for the user to open and use |
| The memory bank | Curated long-term memory: facts, preferences, commitments, and a relationship map of the people and groups in the user's life |

The site you are reading was compiled by **boris**, a single static binary with no JavaScript at publish time — the owner's Zig static-site compiler, built from source. The model it describes is [[model]].
