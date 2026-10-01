# Metronome Starter

**Use Claude Code as a production coach so you ship one YouTube video every week.**

You open this folder in Claude Code, and Claude becomes your production coach. It plans the week, drafts the script, writes the titles, description, chapters and thumbnail prompt, and keeps an honest log of every video and every minute it took.

It does **not** edit your video, and it does **not** build the thing your video shows. Those are separate jobs (see *What you bring yourself* below).

> Made by: [Philipp Kowalski / Bytes and Budgets]: [Bytes and Budgets on Youtube](https://www.youtube.com/@bytesandbudgets)
---

## Where this comes from

It's a cleaned-up copy of the real setup behind a 12-week run: one long-form video a week, on top of a full-time job, on a small finance-and-automation channel.

As of 2026-09-28: **12 of 12 videos published.** One week was missed along the way. The median was **about 2.5 hours of the creator's own time per video**, and all but one video came in under the 3-hour target.

Every rule in here exists because something went wrong once. `LESSONS.md` tells those stories.

---

## How to start

1. **Copy this folder** and give it your project's name.
2. **Describe your channel and audience.** Fill in `baseline/CHANNEL.md` and `baseline/AUDIENCE.md`, or ask Claude to interview you and fill them in.
3. **Write your mission.** Fill the `[BRACKETS]` in `tasks/01-mission-brief.md`: your cadence, your time budget, your tools, and the three ways you'd most likely quit.
4. **Let Claude plan the whole run on paper first.** Use your strongest model and paste:
   > *Read `tasks/01-mission-brief.md` and `SUCCESS.md`. Write the plan to `wargames/plan.md`. Then try to break it, grade it against `SUCCESS.md`, and log the result in `LEDGER.md`.*
5. **Run every session the same way.** Start with:
   > *Read `CLAUDE.md`, then `STATE.md`, then the current phase of `wargames/plan.md`.*

   End every session by asking Claude to update `STATE.md`.
6. **Run every week the same way.** Follow `engine/SOP.md`.

---

## What's in the box

| File / folder | What it is |
|---|---|
| `CLAUDE.md` | Claude's job description and house rules for this project. **Fill in the brackets.** |
| `LESSONS.md` | The hard-won rules from the original run. **Read this first.** |
| `STATE.md` | "You are here." Claude reads it at the start of every session and updates it at the end. |
| `tasks/01-mission-brief.md` | The order you give Claude to plan the whole run before it starts. |
| `SUCCESS.md` · `LEDGER.md` | The quality bar a plan must meet, and the log of planning rounds. |
| `wargames/` | Where the plan gets written. |
| `baseline/` | Your channel and your audience. |
| `engine/` | The weekly routine, plus templates for scripts, packaging, the pre-record checklist, recording setup, and the "what quiet weeks mean" rules. |
| `topics/TOPIC_BANK.md` | Your list of video ideas. |
| `videos/` | One file per video. Includes a real packaging file as a worked example. |
| `logs/` | The streak log and the time log. |
| `BUILD_ASSISTANT_CONTEXT.md` | A brief to hand to a *separate* assistant that helps you build what the video shows. |

`debriefs/` and `decisions/` aren't included. Create them when you need them, for checkpoint write-ups and for decisions worth remembering.

---

## What you bring yourself

This kit covers the **production coach** only. The original run also used:

- **An editing pipeline.** A second, separate Claude Code project did the cutting, captions, motion graphics and the final render. It isn't included. Any editing route works; `engine/SOP.md` marks where it plugs in.
- **A build assistant.** Hands-on "how do I build this?" questions went to NotebookLM, loaded with the creator's own training material, and never to this project. Week 3 showed why (see `LESSONS.md`).
- **A thumbnail image model.** Nano Banana Pro, fed with a few of the channel's own successful thumbnails. Claude only writes the prompt.
- **Recording.** Camtasia for the per-beat recording, and OBS for a green-screen key. Settings are in `engine/recording-setup.md`.

---

## A note on cost

The templates are free to use. The AI isn't. Claude Code, the image model and any AI used *in* your videos all cost money, so don't promise your audience anything is "free" unless it really is.
