# A&D Universe — 3D Online Prototype

Playable original 3D browser multiplayer proof-of-concept with a connected city, basketball shooting, football scoring, room codes, avatars, and room chat. This is **not** photorealistic or a finished AAA sports game. Basketball and football use simplified scoring mechanics, not complete sports rules or teams.

## Run locally

1. Install Node.js 18 or newer.
2. Open a terminal in this folder.
3. Run `npm install`.
4. Run `npm start`.
5. Open http://localhost:3000 in your browser. Open another window to test multiplayer.

Internet is needed for the Three.js module from jsDelivr. The client connects over WebSocket to the same host as the webpage.

## Host online

1. Upload these files to a GitHub repository (keep `public/index.html` under public).
2. In Render, create a **Web Service** from that repository, environment `Node`, build command `npm install`, start command `npm start`.
3. Open the Render site URL with a friend, join using the same room code.

Render and GitHub policies and costs may change. This is not a static-only Netlify site: WebSockets require the Node server. Use appropriate supervision/account support when an online service requires an adult.

## Controls

WASD / arrows: move; Shift: sprint; E: enter nearby arena; Space: shoot / score; ESC: city; mouse drag: orbit camera; mouse wheel: zoom; mobile: directional pad/action button.

## Notes

- 3D avatars are simple geometric placeholders, not realistic character models.
- Multiplayer sends movements and scoring results through the Node WebSocket server. Gameplay physics are simple, and not fully authoritative or cheat-proof.
- Online chat has basic length filtering but no moderation, account verification, or persistent records. Only share room codes with people you trust.
- Player scores are per connection, not saved to a database.
- Later milestones: realistic character assets, driving physics, full team sports, matchmaking, collision, server-authoritative simulations, character creation, accounts, moderation.
