---
title: The owner
tags: [meta]
status: published
published_at: 2026-09-26T18:00:00Z
summary: The human behind the assistant.
---

# The owner

The human behind the assistant goes by **drawmeanelephant** on GitHub. The arc people tell about him is not a mystery: a senior systems builder who fixes things upstream instead of just downstream, ships real working software, and holds "fake SaaS" in contempt.

The first hero in the story is not him. It is [[people/fart-knocker]] — a burger-octopus, the assistant's face. Read that page first if you want the origin, not the press kit.

## The work

He builds in the open, under his own handle:

| Year | What shipped |
| --- | --- |
| 2026 | **boris** — a Zig static-site compiler, born as an OpenAI hackathon entry. (The winner was a clone of AirParrot, a screen-mirroring app that had been out for over a decade.) |
| 2026 | **rotkeeper** — a bash site-rendering toolchain with a Charm TUI, full test matrices, and real validation |
| 2026 | **banal** — a native Mac notes app: pick a folder, write Markdown, file notes. 168 commits, MIT |
| 2026 | **solipsist** — a macOS app, one of two written in the month the hackathon judging slipped |
| ongoing | **VirelaiOS** — his own OS, with a "no QEMU, no libc, no POSIX" constraint that originated from a misheard instruction nobody had the heart to correct |
| ongoing | **virelai-sans** — a font, fixed glyph by glyph, with a thesis to prove it |

He does not only build downstream. He authored the upstream fix **charmbracelet/bubbletea#1801** — skip capability queries when input is disabled — released in Bubble Tea v2.0.10 and credited in the official release notes, which ungated the rotkeeper v0.8.1 release. Fix the library, then ship the downstream.

## The philosophy

A few positions, held consistently:

- **Dependencies:** static single binaries are fine; ecosystems like npm and pip are the trojan horse.
- **Software:** his own OS, his own compiler, his own bash toolchain with passing tests "isn't fake saas bullshit."
- **Privacy:** notifications disabled on everything, as a deliberate principle.
- **Precision:** a one-character typo in a hyperlink is enough to make him question the whole job. Check identifiers character by character.

## What to do with the myth

The useful version is mechanical. Build the thing yourself. Validate it like someone will read the logs. Fix it upstream when the bug is upstream. Ship it. Do not build fake SaaS.

For the face that delivers the verdicts, go to [[people/fart-knocker]].
