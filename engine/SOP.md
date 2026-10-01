# SOP — The Weekly Run

**Two rules that never bend:**
- **Budget:** [3.0] h of *your attended time* is a **soft target**, not a gate. Log every minute. Going over is fine as a *chosen* investment (put the reason on the log row), judged on cost vs. benefit at mid-run and at the end. Unattended render time never counts (Machine column).
- **One take:** all raw footage comes from one continuous sitting. Flub → say "cut", say it again, keep rolling. No re-shoot on another day.

*(you) = the creator · (Claude) = this project. Times are rough guides, not gates. Only the total budget is a cap.*

## The run: do these in order

1. **Pick the topic** from `topics/TOPIC_BANK.md`. It must fit the channel and be safe (no employer or client data). *(you + Claude)*
2. **Claude drafts the script**: beats plus full narration, in last week's exact format. *(Claude)*
3. **You read it and adjust it** into your own voice, leaving inline comments in the doc. Claude actions them as a **redline** (see below). → log **Script**. *(you, ~10–20 min)*
4. **Run the pre-record checklist** (`engine/one-take-checklist.md`): screens ready, **secrets off-screen**, tracks and audio set. *(you)*
5. **Record** in one sitting: screen + webcam + mic on separate tracks, **one recording per beat**, flubs stay in. → log **Record**. *(you, ~30–45 min)*
6. **Export the beats**, using GPU encoding if you have it. Name them in order (`01-…`, `02-…`). → log **Export**. *(you)*
7. **Edit** with [YOUR EDITING PIPELINE]. You approve at the gates:
   a. **Watch the rough cut properly**, end to end, with notes as precise as "at 0:15 you cut a word". **Do NOT skim it.** Skimming the cut broke the very first video of the original run.
   b. Approve the graphics plan. Check every line names *an object doing something*, not a sentence in a box.
   c. Let it render → **Machine** time (go do something else).
   d. Watch once → **ONE** round of notes.
   → log **Cut review** + **Edit (attended)** + **Machine**. *(you)*
8. **Package.** Claude drafts the titles, description, chapters (from the final render's `.srt`) and a thumbnail prompt into `videos/weekN-packaging.md`. You pick the title and generate the thumbnail. Run the honesty check. → log **Package**. *(Claude + you)*
9. **Publish.** Upload the final video, **attach the `.srt` captions**, paste the description. → log **Publish**. *(you)*
10. **Log it.** Fill in the minutes in `logs/TIME_LOG.md`, then add the `logs/STREAK.md` row: date, URL, the **title as actually published**, and the public-page check. *(you + Claude)*

## Script review: the redline standard

Every change Claude makes to a script doc shows as a **redline**, the way a contract markup works. You can read what it said before and what it says now, side by side.

- **Removed text stays on the page**, struck through in **red**. It is never actually deleted.
- **New text goes in next to it**, in **blue and underlined**.
- **Replacing a phrase** = strike the old text in red, then insert the new text in blue right after it.
- Each change also gets a short **`[ClaudeCode]` reply on the relevant comment** saying what was done and why. Never in the script body, because the body has to stay recordable.
- **Claude never resolves a comment.** Not once, ever.

**Why bother:** struck-through text is never deleted, so a comment's anchor survives. Hard-deleting commented text orphans the comment, and from your side it looks exactly like Claude deleted your feedback. That happened twice in the original run before this rule.

**How (original setup):** the script lived in a Google Doc, and Claude edited it through a Google Workspace command-line tool. Google's own "Suggesting" mode couldn't be created through the API there, so the redline is done by hand-formatting: strikethrough + red, underline + blue. A Word doc with real track changes is a fine alternative.

## Ship it when these 5 pass, nothing more
1. Audio clear · 2. Screen text readable at 1080p · 3. Captions skim OK · 4. Thumbnail done · 5. Nothing confidential on screen.

## If a tool breaks
Drop to **cut + captions only** (no fancy graphics). It still ships. Effects are optional by design. Note it as a tooling issue; don't absorb the delay silently.

## Watch for creep (the budget-killers)
One review round only · script within its length · recording ≤ 45 min.
