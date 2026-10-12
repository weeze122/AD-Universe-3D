# A&D Universe V2 — Sports City

New playable browser prototype built using your original Node/Express/WebSocket server.

## Start on your PC
1. Install Node.js 18 or newer.
2. Open this folder in a terminal.
3. Run `npm install` then `npm start`.
4. Go to http://localhost:3000 in Chrome or Edge.

Requires internet to load Three.js from jsDelivr. To publish online, upload **the whole folder** to GitHub (including `public/index.html`), then create a Render Web Service using `npm install` and `npm start`. `render.yaml` is included.

## Controls
- 1 city, 2 basketball, 3 football.
- WASD move; Shift sprint; mouse drag rotate; V change first-person/third-person/broadcast camera.
- Basketball: hold and release Space to shoot with timing meter; Q/E/R/T passes to teammates.
- Football: Space advances carrier, Q/E/R/T/Y/U throw to marked receivers, F tackle (placeholder).
- Receiver buttons appear over friendly AI players.
- Room/name inputs at top right connect to same server and room.

## What's implemented / limitations
- City with roads, towers, street trees and building windows.
- Basketball arena with tiered stands, ceiling lights, hoop, backboards, court lines, and 5 blue versus 5 red slots including your player, simplified AI motion and shots.
- Football stadium with yard lines, end zones, goalposts, stands, lights, 11 blue versus 11 red slots including your player, rudimentary AI motion, passes, tackle proximity and touchdown scoring.
- Three camera modes, running/sprint motion, live WebSocket rooms from original server.
- These are **visual/gameplay prototypes**: AI runs basic patterns; there is no true playbook, full rules engine, offensive/defensive decision intelligence, official game clock logic, collision engine, photorealistic players, or accurate online synchronized ball/team gameplay. Remote WebSocket positions are exchanged but other human avatars are not yet rendered; the AI matches currently simulate independently for each client. No production multiplayer matches or matchmaking. The original server's scoring rules remain simplified.
