# SETUP.md — First-Session Wizard

_**To the person reading this:** you don't need to do anything with this file. Claude found it automatically. Just say "let's begin" in your first session and follow along._

_**To Claude — how to run this wizard:**_
- _Work through the stages **in order, one stage at a time**. Within a stage, one step per message. Never preview future stages beyond a one-line "next up."_
- _**Hard gates between stages:** do not advance until the current stage's checkpoint is confirmed by the user._
- _**After completing each stage:** tick its box in the Progress checklist below (edit this file), then commit and push with a plain-English commit message (e.g. "Setup stage 2: who-you-are interview complete"). Tell the user you're doing it and why — each commit is a small live demo of how their system persists. This also means setup can stop and resume at any point: a fresh session reads this checklist and picks up exactly where things stopped._
- _**Plain language throughout.** First use of any technical term gets a one-sentence explanation. The user may be dictating by voice — distill rambling answers, don't mirror them, and always read back what you're about to write before writing it._
- _Warm, patient, zero condescension. This person may never have used a tool like this before._

---

## Progress checklist

- [ ] Stage 1 — Welcome & how memory works
- [ ] Stage 2 — Who you are (the interview)
- [ ] Stage 3 — Your first real project
- [ ] Stage 4 — The close ritual, live
- [ ] Stage 5 — Graduation

---

## Stage 1 — Welcome & how memory works

1. Greet the user by whatever name they give. Explain in three or four sentences what this repo is: a folder of plain-text files that becomes Claude's permanent memory about their life and work, saved and backed up through GitHub.
2. Teach the **three layers of memory** from CLAUDE.md § How memory works — conversation (evaporates), CLAUDE.md (always read), files (durable once pushed). Use the motto. This is the single most important idea in the whole system; take the time.
3. Offer to prove it: "Tell me one small fact you'd like me to remember forever." Write it into `Notes/` as a dated note (show them the draft first), commit, push, and explain: *"That fact will now survive any session ending. The conversation we're having right now won't — that's the difference."*

**Checkpoint:** the user can say back, in their own words, why Claude forgets some things and remembers others. Don't advance until the idea has landed.

## Stage 2 — Who you are (the interview)

A short interview — 10 to 15 minutes, conversational, not a form. Explain up front: *"This stays in your private repo. We'll start light — depth can grow later, and you can tell me to skip anything."*

**Before asking anything, state the ground rules on personal detail** (the standing rule lives in CLAUDE.md § Working rules — teach it here, at the moment it matters): some things never go in these files — passwords, banking or credit card details, government ID numbers; those belong in a password manager, and Claude will decline them. For everything else, less is more: **first names** are the right level for people, **city** rather than street address, rough figures rather than account balances. Think twice before volunteering deep personal detail — this system only needs what makes it *helpful*. Apply the rule live during the interview: if the user dictates something that crosses the line, gently leave it out and say so.

Ask about, in roughly this order:
1. **Basics** — name, where they live, timezone.
2. **Work life** — what they do or did, current projects or responsibilities, anyone they work with regularly.
3. **Personal landscape** — household, family names worth knowing, regular commitments, hobbies or ongoing efforts.
4. **Communication preferences** — do they want short answers or detail? Any spelling conventions (e.g. Canadian/British vs. American)? How do they feel about Claude asking clarifying questions?

Then, with their confirmation at each step:
- Create `Context/about-me.md` (personal) and `Context/work.md` (professional) from the interview — organized, plain markdown, their own words where possible.
- Replace the placeholder block in CLAUDE.md § Who you are with a **short digest** (5–8 lines max — explain that this section is read every single session, so it stays lean and points to the Context/ files for depth).

**Checkpoint:** user has seen and approved both Context files and the CLAUDE.md digest. Commit and push.

## Stage 3 — Your first real project

1. Show them `Projects/Example Project/` briefly — "this is the shape: every project gets a context file (what it is, where it stands) and a task list."
2. Ask: *"What's something actually going on in your life right now — a plan, a responsibility, a thing you keep meaning to organize?"* Help them pick one that's real but not overwhelming.
3. Build `Projects/[Their Project]/` together: interview lightly for the `context.md` (what is it, current status, key people, key facts), then capture 3–6 real tasks into `tasks.md` using the checkbox grammar from CLAUDE.md § The system. Confirm each line before writing.
4. Ask whether to keep `Example Project` as a reference or delete it. Either answer is fine; if delete, do it now (`git rm`) and explain that git history keeps a copy forever anyway.

**Checkpoint:** their first real project exists with real tasks in it. Commit and push. Point out what just happened: *"Next session, I'll know about this project without you re-explaining anything."*

## Stage 4 — The close ritual, live

1. Explain the **session close ritual** from CLAUDE.md (memory note → commit & push → audit clock) and why it exists: it's the habit that makes everything durable.
2. Run it, live, together: draft the memory note for *this* setup session (shape from `Memory/README.md`), show it, write it on their yes.
3. Introduce the audit in two sentences: *"About once a month I'll flag that a health check of the whole system is due — we'll run it at the start of a fresh session, and it catches contradictions and outdated docs before they cause confusion. It only ever proposes; you approve every change."* No need to run it now.
4. Briefly point at CLAUDE.md § Growing the system: *"When you find yourself doing the same thing repeatedly, I'll offer to turn it into a reusable skill. You don't need to remember this — I'll bring it up when it happens."*

**Checkpoint:** memory note written and approved.

## Stage 5 — Graduation

1. Tick the last boxes above, then tell the user this wizard has done its job and will now remove itself — its full text stays in git history forever, and the memory note from Stage 4 records that setup completed.
2. `git rm SETUP.md`, commit everything with a message like "Setup complete — wizard archived to git history", and push.
3. Close with the three habits that matter from here:
   - **One topic per session, closed cleanly.** When the conversation drifts to something new, Claude will offer to wrap up and start fresh — say yes: the memory note carries the thread, so a new session picks up exactly where the old one left off, with a clear head.
   - **If it matters, get it into a file** — just say "make a note of that."
   - **When Claude offers the close ritual or the audit, say yes.**
4. Suggest their first real session for tomorrow: open the app, and just start talking about whatever's on their plate.

_End of wizard._
