# STATUS — Halal Da Nang GrabFood Launch

> Live project heartbeat. Source of truth for menu/pricing = `SOT.md`.
> Visual assets = Drive `1. Duong Dang / Halal Da Nang` (Banners / Products).

Updated: 2026-06-17

---

## Roles
- **Chat 1 (this) — Orchestrator:** holds strategy, hands briefs to Chats 2 & 3.
- **Chat 2 — Image Studio:** generates banners (16:9) & product shots (1:1).
- **Chat 3 — GrabFood Integrator:** field-by-field portal data entry.
- Sessions are isolated; the user is the bridge between chats.

## Working rules
- Minimal structure: 2 git files + 3 Drive folders. No sprawl.
- **Every write/edit needs user approval first.**
- Drive scope = `Halal Da Nang` only. Nothing else in Drive is touched.
- One step at a time; nothing advances until images + portal config confirmed.

---

## Progress

| Step | Scope | Image (Chat 2) | Portal (Chat 3) | State |
|------|-------|----------------|-----------------|-------|
| 1 | Noodle Bar | Hero banner + 1:1 noodle | Category + modifier framework | In flight |
| 2 | Burgers & Chicken Mains | briefed (5 tiles) | briefed (6 items + sauce modifier) | Pending build |
| 3 | Salads & Finger Foods | — | — | Not started |
| 4 | Drinks & Desserts | — | — | Not started |

## Tooling confirmed
- Canva: WORKS (generates real design candidates; stock photos — needs real food shots dropped in for product tiles).
- Drive: connected, scoped to `Halal Da Nang`.
- Git repo: this branch holds STATUS.md + SOT.md.

---

## Open decisions (blocking)
1. **3 phantom-ingredient items** — see SOT.md §3. Shrimp ×3, Schnitzel, Fish & Chips. Need source-or-rework call.
2. **Canva test tile** — 4 candidates generated for Big Hamburger Cheese; awaiting user pick.

## Next action
- User to resolve ingredient gaps + pick Canva candidate, then release Step 2 portal build.
