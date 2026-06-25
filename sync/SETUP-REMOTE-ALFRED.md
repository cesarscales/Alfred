# ACTION ITEM — GET REMOTE/MACBOOK ALFRED TO PARITY WITH DESKTOP ALFRED
Priority: HIGH — the gap is costing real time. Logged Tue 2026-06-16.

## THE PROBLEM
Remote Alfred (MacBook / claude.ai web instance) is NOT up to date with Desktop
Alfred. Every time Cesar asks Remote Alfred for something, half the answers are
"I can't access that from here." This is costing time we don't have with ads
going live this week.

Examples of what Remote Alfred CANNOT currently do that Desktop can:
- Read the `cesarscales/head-quarters` repo (where Vaquero X creatives live)
- Access Stripe / pull or create invoices (e.g. Tomicheal $100 invoice)
- See the Obsidian brain / HQ content
- ElevenLabs voice (HQ back-and-forth)
- Agent routing (Zenith, Vortex, Nexus, Stratos, Aurelius)

## THE GOAL
Make Remote Alfred function as close to Desktop Alfred as possible so Cesar can
work from his phone / MacBook without hitting dead ends.

## WHAT NEEDS TO HAPPEN (to do at desktop)
1. **Repo scope** — add `cesarscales/head-quarters` to the remote session's
   allowed repositories so Remote Alfred can see creatives + previews.
2. **Push the Obsidian brain** into the shared repo (or mirror the key notes)
   so Remote Alfred reads the same source of truth, not a stale skeleton.
3. **Stripe access** — decide how Remote Alfred gets payment visibility
   (connect a Stripe MCP/integration, or log invoice links into the repo).
4. **Document what stays Desktop-only** — ElevenLabs/HQ voice and agent routing
   likely can't be replicated remotely; note that so expectations are clear.
5. **Confirm sync cadence** — Desktop must push after every important change so
   Remote stays current (this is the root cause of the drift).

## NOTE ON REALISTIC LIMITS
Remote and Desktop are separate Claude instances — they don't share live memory,
only this git repo. Full 1:1 parity isn't possible for tools that require local
machine access. But repo scope + pushed brain + Stripe visibility closes ~90%
of the gap that's actually costing time.
