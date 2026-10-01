WARGAME ORDER. You are not executing this mission, you are purely planning it on paper.
[EXECUTOR MODEL] will run the brief below session by session, so tailor the plan
to how that model behaves.

Fight the mission on paper, move by move, and write it to wargames/plan.md.

For every move, state:
- the expected observation if it worked,
- the expected observation if it failed,
- the most likely failure mode, its warning signals, and the counter-move.
Every fork gets a trigger: if you observe X, take route A, else route B.
Flag any assumption your research could not resolve as a (VARIABLE) placeholder.
End with abort conditions: the states where the plan must stop instead of pushing on.

## Mission brief

Goal, in full context (written for an agent with none of my context):

[2–4 sentences about you: what you do by day, how much time you really have,
what else competes for it. Keep it as specific as you're comfortable sharing
with the model, but nothing you wouldn't want in a file.]

The mission: design and prove a sustainable YouTube CONTENT ENGINE: a
repeatable production system (video formats, scripting, recording,
packaging with thumbnails and titles, publishing) for my channel
[CHANNEL: size, topic, language]. The machine is the product, and
CONSISTENCY is the success metric.

Engine parameters (fixed, not up for reinterpretation):
- Cadence: [1 long-form video per week].
- Time budget: [~2–3 hours per week ALL-IN] (topic, script, recording,
  editing, thumbnail, publishing). The engine must fit the budget, not
  the budget stretched to fit the engine.
- Production stack: [how you record, how you edit, which AI tools help].
- Topic scope: [what the channel covers].
- The engine must coexist with: [job, family, other projects, training...].

Expected result (definition of done): BEHAVIORAL PROOF, not documents.
A [12]-week streak: [12] consecutive weekly videos shipped, each produced
within the time budget, with the time actually logged. The streak is
checked against the channel's public upload dates plus the time log.

Things you would not guess (treat as hard constraints):
*Examples from the original run. Keep, change or delete them.*
1. ONE TAKE OR NOTHING: if a video needs more than one recording session
   or a re-shoot on another day, it dies. Every script must be deliverable
   in a single sitting.
2. The audience responds to sober, proof-driven content; anything smelling
   of hype burns trust.
3. Retention-maximising edits (jump cuts every two seconds, constant
   b-roll) are WRONG here: they don't fit tutorial content and they kill
   the time budget. Editing stays lean.
4. Chasing the algorithm is WRONG here: no trend-jacking, no picking
   topics by search volume.
5. Nuance: bold PACKAGING (strong thumbnails, sharp titles) is fine.
   Packaging may be bold, editing stays lean, topics stay authentic.

Pre-mortem: the realistic ways this dies. The plan must carry a
structural defence against each.
*The original three. Check which are true for you.*
- Perfectionism creep: videos slowly get more ambitious until each one
  blows the budget and the streak quietly collapses.
- Demoralised by silence: weeks of flat views and no comments, with no
  agreed way to read them, until motivation dies. The engine needs
  pre-committed rules for interpreting silence, without turning them
  into performance gates.
- Priorities eat the slot: [your other priorities] take the weekly
  recording window; the side project is always the first thing cut.

Break the mission into phases. For each phase give:
- objective,
- an optimistic assumption AND a pessimistic assumption,
- likely failure modes with fixes,
- verifiable exit criteria,
- a token budget.
Simulate consequences down to the 3rd order.

Add a master failure table (production & time budget, packaging quality,
audience response & how to read it, platform/algorithm, AI pipeline/tooling,
executor discipline, streak protection/motivation) with detection and
recovery for each. Call out exactly where [EXECUTOR MODEL] tends to go
wrong, in particular its tendencies to flatter my content instead of
judging it, to declare success on weak evidence, and to estimate numbers
instead of demanding real data (YouTube Studio exports, actual upload dates,
actual logged hours).

How the executor must check before reporting something done:
- The streak is checked against the channel's public upload list (dates),
  never against intentions or claims.
- Every video gets a time-log entry (planned vs. actual); budget compliance
  is checked against the log, not against memory.
- Any analytics claim rests on real YouTube Studio data I pulled myself,
  never on estimates.
- The engine's artifacts (script template, pre-record checklist, packaging
  template, weekly routine) exist as files in this folder, not as chat advice.

Open variables (resolve during research or week 1, never guess):
- (VARIABLE: exact tool list of my editing pipeline.)
- (VARIABLE: cash budget; may any NEW paid tool be added?)
- (VARIABLE: the fixed weekly recording slot.)
- (VARIABLE: start date of week 1.)

Abort conditions (the plan stops dead, no adaptation):
- Cadence collapse: [three] missed weeks in a row → a written freeze note,
  never a silent fade-out. A single missed week is flagged, not frozen.
- Budget blowout: clearly unsustainable time cost (e.g. [7–8 h] per video)
  → halt and redesign the engine before further production.

Deliverables:
1. A markdown plan written for an agent starting cold (who, what, critical
   path, stack, folder structure, method, phases).
2. Optional: an HTML visual version with diagrams.

Assume you will hit barriers no matter how intelligent you think you are.
Plan for them before doing anything.
