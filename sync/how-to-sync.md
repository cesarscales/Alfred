# HOW TO KEEP ALL THREE ALFREDS IN SYNC

## The System
This repo (cesarscales/alfred on GitHub) is the single source of truth.
All three devices read from and write to this same repo.

---

## Desktop (Windows) — Claude Code
1. Open Claude Code in the Alfred project folder
2. Run: git pull origin main
3. Work with Alfred — he'll read all files automatically
4. When done: git add . && git commit -m "update [what changed]" && git push

## MacBook — Claude Code
1. First time: git clone https://github.com/cesarscales/alfred
2. Every session: git pull origin main
3. Same workflow as desktop — Claude Code reads files automatically
4. Push changes when done: git push

## Mobile — claude.ai Projects
1. On desktop or MacBook, open: _alfred-brain/mobile-sync.md
2. Copy the latest CLAUDE.md + any relevant status files
3. Paste into the Alfred project in claude.ai
4. Mobile Alfred is now current

---

## When to Sync
- Before any important conversation: pull latest
- After any important decision or update: commit + push
- Before switching devices: always push first

---

## File Structure
Alfred/
├── CLAUDE.md                          ← Master context (read this first)
├── _alfred-brain/
│   └── mobile-sync.md                 ← Mobile paste template
├── cesarcscales/
│   └── clients/
│       └── vaquero-x/
│           └── status.md
├── cnc-lawn-care/
│   ├── creatives/                     ← Store creative briefs here
│   └── campaigns/
│       └── launch-may22.md            ← CNC launch checklist
└── sync/
    └── how-to-sync.md                 ← This file
