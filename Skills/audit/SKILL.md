---
name: audit
description: Run a health check of the whole system — CLAUDE.md, skills, projects, notes, memory — surfacing contradictions, duplication, staleness, and gaps between what the docs say and what actually exists. Trigger when the user says "run the audit", "systems audit", "review the system", "check the system", or at the start of a session after the close ritual has flagged the audit as due. Also useful right after a session where something went wrong or felt clunky.
---

# Skill: Systems Audit

**Purpose:** review the system with fresh eyes and produce a specific, numbered list of proposed fixes. This is not a rubber-stamp review — the goal is to find things that are wrong, missing, duplicated, or no longer true. **If the audit produces no findings, something was missed.**

**Run this at the start of a fresh session, not the tail of a long one** — fresh eyes are the point, and a clear context window is what makes them possible. The session close ritual only *flags* the audit as due; if a due audit is requested mid-way through a long working session, suggest deferring it to a fresh one.

---

## First principle: evolution is not drift

This system started from a seed, and it is *supposed* to grow away from it. The audit never drags the system back toward the original template. The distinction:

- **Drift** = internal inconsistency. The docs say one thing, practice does another; the same rule stated in two places now disagrees; files exist that nothing references. → The audit proposes corrections.
- **Evolution** = coherent change. The user stopped using a folder, invented a new convention, renamed things to match their own vocabulary. → The audit proposes **documenting it**: updating CLAUDE.md so the written system matches the real one. The doc follows the person, not the other way around.

---

## What to check

The target list is discovered, not fixed — audit whatever actually exists:

1. **`CLAUDE.md`** — the main target. It is read every session, so its size is a recurring cost; measure it and flag anything that belongs in a skill or reference file instead.
2. **`Skills/`** — every skill folder on disk vs. the Skills table in CLAUDE.md. Flag both directions: live but unregistered, registered but missing. For each skill: are its trigger, procedure, write authority, and data home still accurate?
3. **`Projects/`** — folders on disk vs. anything CLAUDE.md or other docs claim exists. Projects untouched for months: propose asking the user whether to close them (a closing line in context.md, not deletion).
4. **`Memory/` notes since the last audit** — read them all; they are the record of what actually happened between audits and the primary input for the Propagation lens below. Collect: fixes and workarounds that worked, conventions invented or adjusted mid-session, anything the user corrected Claude on. Also: open loops in old memory notes that were never picked up (surface them, oldest first).
5. **`Notes/` filenames and note shapes** — convention drift against the documented patterns.
6. **`Projects/*/tasks.md`** — checked-off lines older than ~30 days piling up (propose moving them to a dated "Done archive" section or a project log); partially-done tasks wrongly checked off.
7. **Anything else at the root** — files that belong somewhere, duplicates (`name (1).md`), orphans nothing references.

Do not read every file in the repo — the audit reads system documents and samples the rest.

## Audit lenses

Apply each in turn. Every finding gets a **specific proposed change** — quoted text where possible, never "consider clarifying."

1. **Gaps** — if Claude read only CLAUDE.md, what would it still not know that this user assumes?
2. **Contradictions** — could two reasonable readers of these docs do different things?
3. **Aspirational vs. actual** — things described as existing that were never built. Flag clearly so future sessions don't act on them as real.
4. **Redundancy** — the same rule stated in more than one place. One canonical home, pointers everywhere else; duplicated rules drift independently, and that's how contradictions are born.
5. **Staleness** — true when written, no longer true. Verify "not yet done" claims before repeating them.
6. **Doc vs. practice** — the evolution check: where has actual usage diverged from the written system? Propose doc updates that follow the person.
7. **Propagation** — the consistency check, fed by the Memory notes since the last audit: a fix, convention, or way of working that proved itself in one session or one project but was never spread. For each proven local improvement, propose applying it **everywhere the same pattern occurs**, and — if it amounts to a rule — giving it one canonical home (CLAUDE.md or the relevant skill) with pointers. This is the redundancy lens's constructive twin: redundancy catches one rule living in two places; propagation catches one improvement that should live everywhere but lives in one. The goal is that the system grows as *one system*, not as fragments that each learned different lessons.
8. **Orphans** — files nothing references, duplicate copies, empty scaffolds.

---

## Output format

```
## Systems Audit — [YYYY-MM-DD]

### Summary
[2–3 sentences: overall health, the single most important finding.]

### Findings
1. **[Gap / Contradiction / Aspirational / Redundant / Stale / Doc-vs-practice / Propagation / Orphan]**
   Location: [file + section]
   Issue: [what's wrong]
   Proposed change: [specific edit — quote exact text where possible]
2. …

### No action needed
[What was reviewed and confirmed healthy — brief.]
```

---

## Rules

- **Propose, don't execute.** Present all findings and wait for approval before touching any file. Present them as a numbered list with an "all" option so the user can approve, reject, or modify each.
- **Closing beats deleting — and git history is the archive.** This system has no archive folder because it doesn't need one: every committed version of every file is recoverable forever. So a finished or abandoned project gets a dated closing line at the top of its `context.md` and stays put; a superseded note stays where it is (it's history); only true clutter — duplicates, empty scaffolds, orphans — gets deleted, via `git rm`, with each deletion named and individually approved, never folded silently into a batch.
- **Record the outcome.** After applying approved changes: one line in CLAUDE.md § Version, a memory note in `Memory/` (this note is also how the session close ritual knows when the audit last ran), then commit and push.
- **Keep CLAUDE.md slim.** When in doubt between adding to CLAUDE.md and creating a reference file, prefer the reference file.

---

*Skill version: 1.0 — part of the seed. This file is also the model for any new skill: frontmatter triggers, a stated purpose, a procedure, explicit write rules, and a version line.*
