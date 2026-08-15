# THE SIX — Draft Day

Production direction for the recurring THE SIX competitive draft event presented by God Syndicate.

## Live project
GitHub repository: https://github.com/MrGoKuuu/the-six-draft

## Draft rules implemented in the current web build
- Minimum 4 teams, scalable to 6.
- Draft starts only after Admin Control is unlocked and START DRAFT is pressed.
- Stress-test timer: 10 seconds. Tournament presets: 30, 60, 90 seconds.
- A completed pick immediately advances the turn.
- Timer expiry automatically advances the turn.
- Rotating pick order avoids the traditional snake boundary double-pick advantage.
- Player Reserve unlocks after Round 1.
- Reserved players are protected from other teams.
- A reserve skips the reserving team in the next round and gives that team the last compensation position in the following round.
- Only the authenticated captain who owns the current turn, or Admin, can draft.
- Captain Control can privately reveal cards while scouting.
- Player View is intentionally removed from the current product direction.

## Access
- Admin access is entered through Admin Access and is protected by the private test code 1290.
- Captain test codes are stored in the demo build and must be moved server-side before production.

## Assets
The project includes the supplied THE SIX card back, supplied P001 player card artwork, and supplied Team Card reference visual. Additional production assets can be added as the player pool grows.

## Current development mode
The current repository is a front-end shared site deployed from `main`/`root`. The next production milestone is server-backed real-time draft state so multiple captains and the broadcast view share one authoritative session.
