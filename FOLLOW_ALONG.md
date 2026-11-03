# AI Agents & Vibe Coding — Follow Along

**Conference:** All Things Open 2026  
**Session:** AI Agents & Vibe Coding Extended Workshop  
**Instructor:** Mark Hinkle (Peripety Labs / All Things AI)  
**When:** Monday, October 19, 2026 · 9:00 am – 5:30 pm  
**Where:** Ballroom A · Raleigh Atlantic Union Bank Convention Center  
**Official page:** https://2026.allthingsopen.org/ai-agents-vibe-coding

**Session GitHub repo:** https://github.com/TysonK5/vibe_1.git  
**Session deploy target:** [Vercel team `my-own-team16`](https://vercel.com/new?teamSlug=my-own-team16)  
Import `TysonK5/vibe_1` on that Vercel page when you are ready to deploy.

Use this file as the working notes for the day. Fill in the blanks as you go. Point your coding assistant at this file and say:

> Read FOLLOW_ALONG.md. Tell me which checkpoint I am on, then help me complete the next one.

Keep **this notes repo** separate from the two class projects. Course materials are the textbook. Your website and game each get their own folder, GitHub repo, and Vercel project.

---

## Goal for the day

Leave with:

1. A working, deployed website URL
2. A playable, deployed browser game URL
3. GitHub history that shows what the agent changed
4. A repeatable loop: **prompt → generate → check → commit → review → deploy → repeat**

---

## Accounts and folders

| Item | Your answer |
| --- | --- |
| Chatbot / coding assistant | Grok Build (this workspace) |
| GitHub username | `TysonK5` |
| Session GitHub repo | https://github.com/TysonK5/vibe_1.git |
| Vercel team | `my-own-team16` (session target) |
| Vercel import page | https://vercel.com/new?teamSlug=my-own-team16 |
| Website folder | `my-first-site/` |
| Website GitHub URL | https://github.com/TysonK5/vibe_1.git |
| Website Vercel URL | |
| Game folder | `games/alien-tic-tac-toe/` |
| Game GitHub URL | https://github.com/TysonK5/vibe_1.git |
| Game Vercel URL | |
| Playtest partner | |

### Create before (or during) setup

```text
vibe_confer_1/                 ← this notes project
  FOLLOW_ALONG.md
  my-first-site/               ← Project 1 files
  my-first-game/               ← Project 2 files
```

### Required accounts (free)

- [x] [GitHub](https://github.com) — `TysonK5/vibe_1`
- [x] [Vercel](https://vercel.com) — signed in; team `my-own-team16`
- [ ] [v0](https://v0.dev) — available through the Vercel account

Stop before deploying during setup. First production deploy happens in class after you have checked the files.

---

## The loop you will run all day

```text
Idea  →  Brief  →  Small build  →  Open it  →  Check it
      →  Commit  →  Pull request / review  →  Deploy
      →  Look at the live URL  →  Next instruction
```

GitHub is the audit trail. Vercel is the live URL. The agent types. You direct, check, and decide what ships.

---

## Morning — Foundations

Workshop programming: **9:00 am – 1:00 pm**  
Lunch: **1:00 – 1:30 pm** (lightning talks / featured sessions are optional)

### 1. How software gets built (SDLC)

Plain-language version of the professional loop.

| Stage | What it means here | Notes |
| --- | --- | --- |
| Idea | One sentence for who it is for and what they can do | |
| Brief | Observable checks, not “make it look nice” | |
| Build | Smallest complete version | |
| Test | Open the actual page / play the actual round | |
| Save | Commit so you can roll back | |
| Review | Read the diff. Say no when the agent drifted | |
| Deploy | Push → Vercel gives a URL | |
| Maintain | Next change is another small loop | |

**Checkpoint:** You can explain why GitHub and Vercel exist even if you never write the code yourself.

- [ ] Done

### 2. Source control for the agent era

Agents produce a lot of files fast. GitHub is how you know what happened.

| Term | Meaning | Your example from today |
| --- | --- | --- |
| Repository | The project’s saved history | |
| Commit | A named snapshot of files | |
| Diff | What changed in this snapshot | |
| Branch | A line of work | |
| Pull request | The checkpoint where a human stays in charge | |
| Rollback | Return to a previous snapshot | |

**Hands-on**

- [x] Session GitHub repo: https://github.com/TysonK5/vibe_1.git
- [x] Owner: `TysonK5`
- [ ] Push this workspace to `origin` so Vercel can import it

### 3. Connect Vercel and deploy a starter

Import new projects here: https://vercel.com/new?teamSlug=my-own-team16

- [x] Sign in to Vercel — team `my-own-team16`
- [ ] Confirm `TysonK5/vibe_1` appears in the import list
- [ ] Import it when the instructor says to (first deploy is production)
- [ ] Open the live URL on laptop
- [ ] Open the same URL on a phone if you can

**What I actually saw:**

```
Live URL:
What loaded:
Anything broken:
```

---

## Afternoon — Build

Workshop programming: **1:15 – 2:15 pm**, then **2:30 – 4:30 pm**  
Monday social: 5:30 pm at Jimmy V’s (optional)

### 4. Vibe coding with v0

v0 turns a plain-English description into working front-end code. You still check the result.

**Starter prompt (paste into v0, then adapt):**

```text
Build a single-page website for [audience].
Title: [heading].
Sections: [2–3 section names].
Primary button: [label] that [exact behavior: open this URL / scroll to this section].
Style in three words: [e.g. calm, high-contrast, playful].
Keep it one HTML page plus CSS. No login, no database, no paid APIs.
Make the main action work on a phone-sized screen.
```

- [ ] Generated a first version
- [ ] Downloaded or copied the files into `my-first-site/`
- [ ] Opened `index.html` locally in the browser

**What worked / what drifted:**

```

```

### 5. Agent development loop

For every change, run this:

1. One focused request (“change X, preserve Y, I will check Z”)
2. Agent generates files
3. You open the files and try Z
4. Commit only if Z passed
5. Deploy
6. Repeat the check on the live URL

**Focused change template:**

```text
For this audience, change ____________.
Preserve ____________.
I will check it by ____________.
```

Change 1:

```
Request:
Observed:
Commit:
```

Change 2:

```
Request:
Observed:
Commit:
```

### 6. Reading what the agent wrote

- [ ] Open a commit or pull request
- [ ] Find one change you asked for
- [ ] Find one change you did **not** ask for (if any)
- [ ] Keep, revert, or rewrite that extra change

**When to say no:** extra pages, logins, databases, APIs, fake content you cannot stand behind, or a broken main button.

---

## Project 1 — Simple website

**Target:** one page, clear heading, two or three sections, one working primary action.  
**Repo:** `my-first-site`  
**Stack:** static HTML / CSS / JS is enough.

Starter themes from the class materials: personal intro, event, hobby, community, fictional business, dream restaurant, dream product, pet, or an All Things AI fan page.

### Brief

| Question | My answer |
| --- | --- |
| Working title | |
| Who is this for? | |
| Main heading | |
| Two or three sections | |
| Button / link label | |
| Exact destination or behavior | |
| Style in three words | |
| Out of scope for v1 | |

**One-sentence outcome:** A visitor can ____________________________________.

### Completion checks

Use only **Passed**, **Failed**, or **Not tested**. A chatbot claim is not a check. A local pass does not count as a published pass.

| ID | Try this | Expected | Local | Live |
| --- | --- | --- | --- | --- |
| W1 | Ask a partner what the page is for | They can say it in one sentence | | |
| W2 | Read heading and sections | Content matches the brief | | |
| W3 | Use the primary button / link | Stated destination or behavior happens | | |
| W4 | Follow each nav link | Each one goes where the label says | | |
| W5 | Phone-sized view | Heading, sections, and button still usable | | |

- [ ] Files saved in `my-first-site/`
- [ ] Pushed to GitHub
- [ ] Deployed on Vercel
- [ ] Live URL recorded at the top of this file

---

## Project 2 — Browser game

**Target:** a short start → play → result → restart loop.  
**Repo:** `my-first-game` (separate from the website).  
**Choices from class:**

1. **Alien Tic-Tac-Toe** (featured) — pick a square, fight an alien; win to claim X, lose and the alien claims O
2. **Five-question quiz**
3. **One-button space dodger**

Arcade reference: https://staging.allthingsai.org/arcade

Keep accounts, databases, multiplayer, global leaderboards, and paid APIs out of v1.

### Brief

| Question | My answer |
| --- | --- |
| Title and theme | Alien Tic-Tac-Toe — solo board + short alien battles |
| Which recipe | Featured: Alien Tic-Tac-Toe |
| Player goal | Get three X marks in a row, column, or diagonal |
| Main action | Click an empty square, then pick Shield / Blast / Dodge |
| How a round ends | X line (you win), O line (aliens win), or full board with no line (draw) |
| Round length | Nine battles at most; each battle is 2–3 exchanges |
| Out of scope | Timers, sound, logins, random alien moves, extra art packs |

**One-sentence game:** The player fights for each square to earn X marks before the aliens complete a line of O.

### Rules the partner should understand before you build

| Situation | What happens | Check |
| --- | --- | --- |
| Before play | Instructions and Start are clear | |
| Start | One new round begins | |
| Play | Main control does the stated thing | |
| Round ends | Result is readable | |
| Restart | Score / board / lives reset | |

### Playtest (two minutes, no coaching)

| Prompt | Observation |
| --- | --- |
| Where did they hesitate? | |
| Which rule surprised them? | |
| What broke? | |
| Would they play again? | |
| First fix | |

- [x] Playable locally — `games/alien-tic-tac-toe/index.html` (linked from the ATO homepage)
- [ ] Partner completed a round and restarted
- [ ] Pushed to GitHub
- [ ] Deployed on Vercel
- [ ] Live URL recorded at the top of this file

**Game prompt starter:**

```text
Build a browser game: [title].
Recipe: [Alien Tic-Tac-Toe / quiz / space dodger].
One round: start → play → result → restart.
Main control: [click square / answer / hold or tap].
Win / lose / draw must be visible on screen.
No login, no server, no leaderboard.
Single HTML/CSS/JS page is fine.
After a round, Play again must reset all round state.
```

---

## Wrap-up — take this back to work

| Question | Notes |
| --- | --- |
| What will I automate next? | |
| Where does an agent still need a human checkpoint? | |
| What should never auto-deploy? | |
| Who on my team reviews diffs? | |

**Demonstration checklist**

- [ ] Show the website’s main action on the live URL
- [ ] Complete a game round and restart on the live URL
- [ ] Point at a GitHub commit / PR that the agent made
- [ ] Name one thing you rejected

**One assumption I corrected:**

```

```

---

## Copy-paste prompts for this workspace

**Start / resume**

```text
Read FOLLOW_ALONG.md. Summarize which checkboxes are done.
Ask me only for the next missing answer, then complete that checkpoint.
Do not mix my-first-site and my-first-game files.
```

**Website increment**

```text
Read FOLLOW_ALONG.md Project 1. The brief and checks are the spec.
Make the smallest change that satisfies the next Failed or empty check.
Preserve everything that already Passed. I will open index.html and try it.
```

**Game increment**

```text
Read FOLLOW_ALONG.md Project 2. Keep the start → play → result → restart loop.
Implement or fix only: [one behavior].
Do not add login, storage, or extra screens unless the brief already has them.
```

**Review the agent’s work**

```text
Show me a short diff summary: what I asked for, what you changed,
and anything extra you added. Stop if a completion check would fail.
```

---

## Links

| Resource | URL |
| --- | --- |
| Workshop page | https://2026.allthingsopen.org/ai-agents-vibe-coding |
| GitHub | https://github.com |
| Vercel | https://vercel.com |
| v0 | https://v0.dev |
| Course repo (if you have access) | https://github.com/mrhinkle/Vibe-Coding-for-Non-Technical-Professionals |
| All Things AI Arcade | https://staging.allthingsai.org/arcade |

Course repo is often private. If GitHub returns 404, use the instructor’s copy or keep working from this file.

---

## Live notes (dump anything from the room)

```
Time / topic:


Quote / demo to remember:


Error I hit:


Fix that worked:
```
