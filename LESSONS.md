# LESSONS — rules learned the hard way

Every rule here exists because something went wrong once in the original 12-week run. The biggest meta-lesson: **the model doesn't remember last week, but the folder does.** Turn every mistake into a written rule the same day.

---

## Working with Claude

**1. Answer or propose. Don't act unless told.**
The single biggest frustration of the whole run was AI doing work nobody asked for: a thumbnail mockup when only a prompt was wanted, or a whole build folder plus dataset created in answer to the question "should we do this here or in a separate project?". A question is not permission to act. The fix: Claude answers, proposes in one line, and waits for an explicit "go".

**2. Build exactly what was asked, with no add-ons.**
Asked for monthly data files "same structure as last time", Claude added a helper column, a 13th file and an extra lookup file. All of it had to be redone. If an extra seems useful, ask in one line instead of putting it in the file.

**3. Split the roles: one project for production, another for building.**
In week 3, the production coach also coached the hands-on build live. It switched approach halfway through, and the week nearly fell over. After that, build questions went to a separate assistant (NotebookLM with the creator's own training material), and the production project only did production. An AI project that does everything does a lot of it halfway.

**4. When you're following along in an app: one step, then stop.**
Don't hand over steps 2–6 at once. And never describe an app's screens from assumption: labels change, and a confidently wrong menu name costs time and trust. If the human says "it isn't there", accept it.

**5. Don't pad verdicts.**
Asked for feedback, Claude invented two "problems" that were actually deliberate choices. Padding hides the real findings. Say the good thing plainly when it's good, and ask whether something is deliberate before calling it a mistake.

**6. Plain words, no internal codes.**
Codes like "F1", "V7" or "Q4" in files the human reads were a constant annoyance. Use the plain name of the thing.

**7. Never change an established format.**
Claude once "improved" a script by pulling the screen moments into a shot list at the top. It broke the editing pipeline and the whole script had to be rewritten. Read last week's version first and match it exactly. Propose changes; never ship them.

**8. Put output files where the human can find them**, inside the project, with the full path. Never in a temp folder.

---

## Scripts

**9. Redline every edit; never resolve a comment.** Twice, Claude replaced commented text, which made the comments vanish from the margin. From the creator's side, it looked like their feedback had been deleted. Strike old text in red, insert new text in blue, reply on the comment. Details in `engine/SOP.md`.

**10. Tutorial, not production system.** In week 3 the demo dataset ballooned to 1,000 rows with statistical outlier logic: a consulting deliverable, not a demo. It buried the payoff and ate the week. Use ~20–40 rows you can point at, the simplest logic that works, and one approach you stick with. **The payoff is the star.**

**11. Find the real hook.** In the variance video, the impressive part wasn't "12 cost centres are over budget"; a report does that. It was "246 line items you'd otherwise read by hand every month-end". Frame the value around the grind it removes.

**12. Never re-explain what another video owns.** A script once repeated two passages from an already-produced video airing later, which would have made that video pointless. Compress it to one sentence and point to the other video.

**13. Beat count drives runtime.** A tighter script with the same number of beats came out at nearly the same length. To shorten a video, cut a beat. The original channel found 10–15 minutes to be its sweet spot, with 8 minutes as the floor for mid-roll ads. Never pad, never compress for its own sake.

**14. Some inconsistencies are fine to leave.** If a new video contradicts an old one in a small way, a viewer commenting "isn't that different from last time?" is engagement. Fix real factual errors, but don't write lines whose only job is to smooth over an older video. *(A judgment call the original run made. Yours may differ.)*

---

## Editing

**15. Watch the rough cut properly.** The very first video's cut failed because the review was skimmed to save minutes. That cost more than the full watch would have.

**16. Copy the pipeline, never the effects.** Telling the editor "use the last few episodes as reference" compounded mistakes week over week, until 45 of 56 animations were just text in boxes. Each episode should invent its visuals from its own script. Quick test: cover the text with your hand. Does the picture still say something?

**17. Green checkmarks lie.** 62 renders were marked "verified" and were all completely empty (fully transparent). A silence check reported "no pauses" because a flag swallowed its output. Don't trust a check that hasn't first been tested against a known failure.

**18. Never reuse footage from finished videos.** Pulling old render material into a new edit "never works". Record fresh 3–6-second screen grabs in one short sitting instead.

**19. Green screen beats AI background removal.** See `engine/recording-setup.md`.

---

## Packaging

**20. Claude writes the thumbnail prompt; the human generates the image.**

**21. Calm, concrete, first-person titles beat curiosity gimmicks.** In a head-to-head test, the creator's "Now the AI runs on my own machine" beat Claude's "My API key was 1234 — and the AI still answered". Let a test settle disagreements, and log the title that actually went live.

**22. Short descriptions, full chapters.** Don't retell the video in text. Chapters come from the final `.srt`.

**23. Never say "free" when the AI costs money.** A skeptical audience catches it, and being upfront about cost builds trust.

**24. Every video gets a real subscribe ask**, framed as the honest trade.

---

## Process

**25. Agree in advance what silence means.** Most small-channel videos get almost no comments. Decide before week 1 that this is normal (`engine/silence-rules.md`), and only look at analytics at mid-run and at the end.

**26. Budget as a soft target, honestly logged.** A hard pass/fail time limit makes people fudge the log. A soft target with a one-line reason on every over-budget row keeps it honest.

**27. Log the build time too.** The original "2.5 h per video" doesn't include building the demo, because that went unlogged. Log it from day one.

**28. Plan absences into the topic bank.** Three videos were pre-produced for a two-week holiday and went live on schedule, but all of it landed in the last few days. Note absences early and start banking well ahead.

**29. The bottleneck is starting, not producing.** The one missed week wasn't a production failure: the recording slipped from Monday to Tuesday to Wednesday. Protect the slot and have a fallback day you actually use.

**30. Weekly is a real ceiling.** For one person with a full-time job, one video a week turned out to be about the maximum sustainable pace. That's a finding, not a failure.
