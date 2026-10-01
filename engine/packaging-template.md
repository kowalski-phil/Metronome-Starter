# PACKAGING TEMPLATE (bold packaging · lean editing · every claim true)

**Deliverable:** one paste-ready file per video, `videos/weekN-packaging.md`. Title, description, chapters and thumbnail prompt each go in their own fenced block with **no markdown inside**, so you can copy them straight into YouTube. Worked example: `videos/EXAMPLE-week12-packaging.md`.

## Thumbnail: Claude writes the prompt, you generate the image
**Its only job is to stop the scroll.** Bold is the target, not the exception. "Honest" means *only*: no **false** claim, no clickbait **gap**, no **hype word**. It does NOT mean tame.
- **Generate, don't hand-build.** Use a strong image model (the original used **Nano Banana Pro**). Hand-building in Canva is a last resort: it burns an hour for a worse result.
- **Attach 2–4 of your own successful thumbnails as style references**, plus your headshot for likeness. Keep that reference set stable; it *is* your template.
- **What makes it pop:**
  - One idea, readable in half a second on a phone.
  - An expressive face when it fits.
  - Big bold text, ≤ 3–4 words.
  - High contrast and saturated colour.
- **Simpler usually wins.** In the original run, removing a before/after split from the thumbnail was the biggest single improvement measured.

## Titles: punchy, still true (≤ ~60 characters)
- **Lead with the calm, concrete, first-person option**: "Now the AI runs on my own machine". In a head-to-head test it beat the curiosity-gimmick option ("My API key was 1234 — and the AI still answered").
- Shapes that work: transformation ("I talk, my to-do list writes itself") · cheeky/relatable · payoff + keyword ("…(n8n)") · "X, not Y".
- If your audience lives in a big-brand tool (Excel, Notion…), **name it in the title**, ideally as the first word.
- **When you disagree on a title, test it.** YouTube's Test & Compare settles it with data.
- **Log the title that actually went live** in `logs/STREAK.md`, not the recommended one.

## Description: short
A hook, one line on what gets built, resources and links, a comment prompt, a subscribe line. **3–5 short lines.** Never retell the video; the captions already carry it.

## Chapters: full density, always from the final render's `.srt`
First mark `0:00` · each at least 10 s apart · ascending · plain-language titles. Put them inside the description block (that's how YouTube detects them).

## Honesty check (publish gate). A title or thumbnail FAILS only if it:
- makes an **unproven claim**, opens a **clickbait gap** ("you won't believe…"), or uses a **hype word**: *game-changer · revolutionize · 10x · secret · hack · unleash*;
- or calls something **"free"** that costs money (AI usually does).
- **PASS example:** "I automated a 3-hour finance report down to 12 minutes." Bold, true, no hype word → ships.

## Call to action: every video, no exceptions
A real subscribe ask in the outro, plus one mid-video where there's a natural seam. Word it as the honest trade ("you got the video; a subscribe helps the channel"), not as a plea.
