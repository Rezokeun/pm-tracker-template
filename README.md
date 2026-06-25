# Project Tracker

A lean, opinionated project-management tracker you run with an AI coding agent (e.g. Claude Code) inside a folder. The Markdown files **are** the system of record — no app, no database, no lock-in. Clone it per project; the agent then keeps the tracker, captures proof of work, logs your sessions, and writes status reports on demand.

It deliberately does a few things well rather than everything: it's built for one person steering one project, not for replacing a full PM suite.

## Why it's shaped this way

It encodes a lean, evidence-driven PM method:

- **Momentum milestones** — break the goal into milestones that each deliver a tangible, visible result every ~4–6 weeks. Progress you can see, not abstract phases.
- **Weekly items** — each milestone holds 1–6 items, ~one week of work each, run in sequence. A milestone is roughly a month of weekly steps.
- **Doer-defined proof, trust but verify** — the person doing the work names the *proof point* (a signed doc, a stakeholder confirmation, a passing test). You validate it and the proof is saved. A confirmation beats a slide deck.
- **Slips are tallied** — when a due date moves it's never silently overwritten; it's logged and counted. Two slips on one item is your signal to dig in.
- **The log writes itself** — every change appends a dated line to the session log as a byproduct, so you get a digestible history without remembering to write one.
- **Status reports are a view** — generated from the tracker and tailored to your audience; they never hold facts that aren't already tracked.

## Use it
1. Copy this folder to a new location named for your project.
2. Open your agent in that folder and fill in `project.md` — it's the gate; reports won't run until it's filled.
3. Break the goal into milestones in `tracker.md`, then add the first milestone's weekly items.
4. Work the project: feed updates in, capture proofs, ask for status reports. Logging and slip-tracking happen automatically as you go.

The agent reads `CLAUDE.md` as its full briefing, so each project clone is self-contained — it needs nothing outside its own folder.

## The files
| file | role |
|------|------|
| `CLAUDE.md` | the agent's briefing — the method and its rules |
| `project.md` | project source-of-truth: background, goal, people, timeline, reporting (the gate) |
| `tracker.md` | the live table: milestones → weekly items, proof points, slip tally |
| `session-log.md` | append-only dated history, written as a side effect of changes |
| `notes.md` | operational reference (guides, variable names, contacts) |
| `evidence/` | captured proofs, one file per proof |
| `reports/` | dated status reports rendered from the tracker |

## License
[MIT](LICENSE) — free to use, adapt, and share.
