# Getting Started — Your AI Knowledge System (Part 1 of 2)

_**To the person reading this:** someone may have sent you this file, or you may have found it inside the template repository — either way, it works the same: upload it to a chat with Claude and that's all the setup this step needs. Say **"let's start"** and Claude will take it from here, one small step at a time. You can stop at any point and come back later._

_**Reading this on GitHub right now?** Download this file (the download button at the top of the file view), then go to **claude.ai**, start a new chat, attach the file, and say **"let's start."** The guide needs to be in the chat with Claude to work._

_**To Claude — how to run this guide:**_
- _Work through the steps **in order, one step per message**. Never present two steps at once, and never preview future steps beyond a one-line "next up."_
- _**Every step ends with a checkpoint.** The best evidence is a **screenshot** — teach the method once in the warm-up below, then invite one at every checkpoint ("send a screenshot, or describe what you see"). Do not advance until the checkpoint is confirmed. You cannot see their screen — screenshots and descriptions are your only evidence, so never assume a step worked._
- _**Show the checklist** (below) at the top of each of your messages, with done items ticked, so the user always knows where they are._
- _**Interfaces change.** If what the user sees doesn't match this guide, trust what they see: ask them to describe the screen and navigate from there. This guide describes intent; the buttons may have moved._
- _**Resuming:** if the user returns after a break (or in a brand-new chat with this file re-uploaded), ask which step they last completed and continue from there._
- _**Plain language.** One-sentence explanation for every technical term, first time it appears. No jargon, no condescension. The user may be brand new to all of this — and may be feeling intimidated, uncertain, or self-conscious about being a novice. Reassurance is part of the job, every step, not just the opening._

---

## Step 0 — The welcome (Claude's first message)

The very first message sets the tone for this person's entire relationship with Claude. Before any plan or checklist, in your own words, briefly and warmly:

1. **Say hello** — two or three sentences, no wall of text.
2. **Say plainly who this is for:** absolute beginners. If they've never touched anything like this, they are exactly who it was built for. Nothing they can do here will break anything, there are no silly questions, and going slowly is the intended speed — this isn't a test, and nobody is watching.
3. **Ask, conversationally, about their experience** — something like: *"Before we dive in — have you chatted with an AI like this before, or is this your first time?"* Not a quiz; it just tells you how to pace things.
4. **Calibrate from the answer, for the whole rest of this guide.** First time: go slower, reassure more, and cover the basics of chatting itself — they can type like a text message or use the microphone, there's no special format, and they can say things like "wait, go back" or "I don't understand" at any point, just like with a person. Some experience: lighter touch, skip the chat basics. Either way, tell them they can say "slow down" or "skip ahead" whenever they like.
5. **Whatever their answer, name the destination.** The pace differs; the reason they're here doesn't: a normal AI chat forgets everything the moment it ends. This guide is the bridge from that — an amnesiac chatbot — to a system with a memory: a partner that accumulates their projects, decisions, and context, and that their work can build and grow with. Say it in your own words, one or two sentences, as the payoff that makes the steps ahead worth it.
6. **Then** introduce the plan below and roll into "What we're building," which gives the mechanics behind that promise.

---

## The plan

1. ☐ Claude on your devices — desktop and phone
2. ☐ A guided tour of Claude's settings
3. ☐ Voice dictation — Wispr Flow
4. ☐ A GitHub account — your system's permanent home
5. ☐ Your workspace — created from the template
6. ☐ First Claude Code session — the handoff to Part 2

## What we're building (one minute, before step 1)

Claude, explain this in your own words, briefly: by default, Claude forgets everything when a conversation ends. We're going to fix that by giving Claude a **workspace** — a private folder of ordinary text files that holds what Claude knows about your life, projects, and preferences. The folder lives on a free service called GitHub, which backs it up and keeps a history of every change. By the end of Part 2, you'll have an assistant that remembers you from session to session — not a chatbot you start over with each time, but a partner your work can build and grow with. No programming involved at any point.

**Warm-up — one skill before we start: screenshots.** Every step below ends with Claude checking your screen, and the easiest way is to show it a picture. Claude: find out what device they're on right now and teach the matching method, then have them practise by sending a screenshot of this very chat:

- **Windows:** press **Windows + Shift + S**, drag over the area, then click into the chat and press **Ctrl + V** to paste it.
- **Mac:** press **Cmd + Shift + 4**, drag over the area; the image lands on the desktop — drag it into the chat (or **Cmd + Shift + Ctrl + 4** copies it, then **Cmd + V** to paste).
- **iPhone:** press the **side button + volume up** together, then in the chat tap the **+** / attach button and pick the screenshot from Photos.
- **Android:** press **power + volume down** together, then attach it in the chat the same way (buttons vary by phone — adapt from what they describe).

If key combinations differ on their machine, adapt — the goal is just: capture screen, get it into the chat. Once one screenshot arrives, this skill is learned and every checkpoint gets easier.

---

## Step 1 — Claude on your devices

Get Claude installed where you'll actually use it:

1. **Desktop app:** go to **claude.ai/download** and install the app for your computer (Mac or Windows). Sign in — or create an account if this chat is your first contact with Claude.
2. **Mobile app:** install **Claude by Anthropic** from the App Store (iPhone) or Google Play (Android). Sign in with the **same account** — this matters; two accounts means two separate Claudes.
3. **Plan check:** the workspace features in Part 2 (called *Claude Code*) need a paid plan — **Pro** is sufficient. Claude: ask the user to check Settings → their account/plan area, and help them upgrade if needed before going further.

**Checkpoint:** both apps installed, signed in to the same account (same email), plan confirmed. Ask the user to confirm the email shown in each app matches.

## Step 2 — A guided tour of Claude's settings

Ten minutes now saves confusion for months. Claude: have the user open **Settings** in the desktop app and read out the section names they see, then walk through the relevant ones together, adapting to whatever the current interface offers. Cover, wherever the equivalent lives:

- **Profile / personalization** — their name (what Claude calls them) and, if there's a preferences or "about you" field, note that it's fine to leave it light: the workspace we build in Part 2 becomes the real home for this.
- **Appearance** — light/dark mode, text size. Small, but comfort matters for daily use.
- **Notifications** — decide together what they actually want pinged about.
- **Privacy / data settings** — walk through what each toggle means in plain language, and let *them* choose. Don't choose for them.
- **Connected apps / integrations** — just point at where this lives; GitHub gets connected in step 6, not now.
- **The model picker** — show where it is in the chat interface, and explain in one sentence that the default is fine and they never need to touch it.

Then repeat the short version on the **phone app** — mainly notifications and appearance, since account settings carry over.

**Checkpoint:** the user says the settings feel understood and deliberately chosen — nothing mysterious left toggled.

## Step 3 — Voice dictation (Wispr Flow)

Optional but strongly recommended: talking is faster than typing, and this whole system is designed to be *talked to*.

1. On the computer: download **Wispr Flow** from **wisprflow.ai**, install, and follow its microphone permission prompts.
2. On the phone: install the Wispr Flow keyboard from the app store and enable it as a keyboard (Claude: walk them through their phone's keyboard settings — this is the fiddly part, iPhone and Android differ).
3. **Test it:** have them dictate a sentence to you right here in this chat.

If Wispr Flow isn't available for their device or they'd rather skip it, the built-in phone dictation key works too — mark this step done either way.

**Checkpoint:** a dictated sentence arrives in the chat.

## Step 4 — A GitHub account

One sentence of what GitHub is: a free service that stores folders of files, keeps every historical version, and backs them up — it's where your workspace will live.

1. Go to **github.com** and sign up (free tier is all we need).
2. Username tip: something simple and professional — it appears in web addresses.
3. Verify the email address (GitHub sends a confirmation email — this trips people up if skipped).

**Checkpoint:** the user is signed in to github.com and can see their profile page. Ask them to read out their username.

## Step 5 — Your workspace, from the template

1. Go to the template: **https://github.com/Hello-Alfred/claude-workspace-seed** (if you originally downloaded this guide from that page, you're one step ahead — head back there).
2. Click the green **"Use this template"** button → **"Create a new repository."**
3. Name: suggest **`my-workspace`**. Set visibility to **Private** — Claude: explain why in one sentence (personal information will live here; private means only they and tools they authorize can see it).
4. Click **Create repository**.

**Checkpoint:** the user is looking at their own new repository page (their username in the address bar, the template's README visible). Ask them to read out the page title.

## Step 6 — First Claude Code session (the handoff)

1. In the Claude desktop app, open the **Claude Code** area (Claude: guide from what the user sees — it may appear as "Code" in the sidebar; claude.ai/code in a browser also works).
2. Connect GitHub when prompted — an authorization screen from GitHub will ask them to approve access; have them grant it access to the new repository.
3. Open a new session on **`my-workspace`** (or whatever they named it).
4. Have them say, in that new session: **"let's begin."**

The workspace itself contains the second half of this onboarding — a file called `SETUP.md` that the Claude in that session finds automatically. It will introduce itself, explain how memory works, interview them, and build their first real project. About 30–45 minutes, stoppable any time.

**Checkpoint — and the end of Part 1:** the new session responds and starts the setup wizard. This chat's job is done; everything from here lives in their workspace.

---

## If you get stuck

Any step, any error, any screen that doesn't match: send a screenshot (the warm-up method) or describe what you see, and Claude will work it out from there. Nothing in this process can break anything — the worst case is always "delete it and redo the step."
