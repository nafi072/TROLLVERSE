# TROLLVERSE: Don't Trust the Level

An original, self-contained browser platformer prototype designed for desktop and mobile browsers.

## Included
- `index.html` — complete game (HTML, CSS, JavaScript, original canvas-drawn visuals)
- `README.md` — these instructions
- `_headers` — lightweight security/cache headers for Cloudflare Pages

## Run locally
Open `index.html` in a modern browser. No build step, npm, API key, or external asset is required.

## Deploy to Cloudflare Pages (free)
1. Create a GitHub repository for the game.
2. Upload `index.html`, `README.md`, and `_headers` to the repository root (not inside another nested folder).
3. In Cloudflare, open **Workers & Pages → Create → Pages → Connect to Git**.
4. Choose the repository.
5. For a static HTML site, choose **None** for framework preset, leave the build command blank, and use `/` as the build output directory if the setup screen asks for it.
6. Deploy. Cloudflare will provide a `*.pages.dev` address.

## Controls
- Left / Right arrow keys or A / D: move
- Space / Up arrow or W: jump
- R: restart level
- Esc: return to menu
- Mobile: on-screen directional and jump buttons

## What's new in v2
- **30 levels** in 3 worlds: The Unwelcome (1-10), The Wobbling Wilds (11-20), The Final Joke (21-30)
- New mechanics: crumbling platforms, spring pads, patrolling enemies, vanishing floors, moving ferries, a door that runs away, and trap doors
- Fixed: a JavaScript syntax error in level 9 that could stop the whole game from loading
- Fixed: moving platforms can now be stood on; game no longer crashes when browser storage is blocked
- Added coyote-time (forgiving jumps) and a levels-unlock flow for all 30 levels

## Notes
This is an initial playable version with thirty original levels across three worlds. It saves level unlocks, cleared levels, death count, and best clear time in the browser's local storage on that device. Local-storage progress does not sync between devices. The project is intentionally asset-free and does not copy source code or artwork from the games that inspired it.
