# THE SIX — Draft Day

Premium browser-based draft control room for THE SIX by God Syndicate.

## Current build

- Broadcast view
- Host Console
- Admin Control
- Captain Control login demo
- Start Draft gate
- 10-second stress-test clock
- Automatic turn advancement at 00:00
- Balanced multi-team order with no back-to-back team turns
- Player categories: Vanguard / Duelist / Strategist / Flex
- Player Reserve unlocks after Round 1
- Draft / Next / Reset controls
- Face-down THE SIX card back
- 3D card reveal
- Placeholder player-card pool
- Team roster status

## Local test

Run a static server from the repository root:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Captain demo access

- T01 / SIX-101
- T02 / SIX-202
- T03 / SIX-303
- T04 / SIX-404

## Important architecture note

This repository is the production front-end foundation. The current demo state is browser-local so the interaction model can be stress-tested safely. A real tournament with multiple captains in different browsers will need a shared realtime backend and authenticated roles; that should be added before Draft Day rather than faking multiplayer with localStorage.

## Asset replacement

Put finished Player Card PNG/SVG files in `cards/` using IDs such as `P001.svg`, `P002.svg`, etc. The current build includes P001 and stress-test placeholders. Replace those assets without changing the UI code.
