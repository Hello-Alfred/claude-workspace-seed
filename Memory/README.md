# Memory/ — session memory notes

This folder is how work survives between sessions. At the close of a working session, Claude writes one short note here recording what happened. "Where were we?" at the start of a session = Claude reads the two or three most recent notes.

## Note shape

**Filename:** `YYYY-MM-DD-HH-MM-short-topic.md` (date and 24h time of writing; topic is 2–5 hyphenated lowercase words).

```markdown
---
status: complete | partial
date: YYYY-MM-DD
---

# [Session topic in plain language]

**Outcome:** 1–2 sentences, declarative — what is now true, not what was discussed.
("Greenhouse project scaffolded; materials list drafted." Not "we talked about the greenhouse.")

**Files touched:** filenames only. Omit if none.

**Open loops:** anything raised but not resolved, one per line. Omit if none.
```

## Rules

- **`status: partial`** means the session stopped mid-work — the Outcome says exactly where, and Open loops say what's next.
- **Append only.** Never edit a past note; write a new one. The newest note on a topic governs.
- **Pointers, not content.** The note names the files that changed; the files themselves are the source of truth.
- Audit result notes also live here — the session close ritual reads the newest one to know when the audit last ran.
