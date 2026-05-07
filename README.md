# Bonnie's Quest

A single-file, browser-based cinematic cozy mystery adventure inspired by classic point-and-click games like King's Quest.

## Current features

- Title screen introducing the larger Hollow Oak Estate mystery
- Three explorable rooms: Main Antique Shop, Back Storage Room, and Upstairs Office
- Classic point-and-click Bonnie movement with walkable floor limits, object approach points, smooth facing, and idle/walking poses
- Mabel dialogue interactions with branching choices, clue reveals, and deliberate misdirection
- Missing antique collector Evelyn Blackwood and a hidden family secret tied to Mabel's Antiques
- Reference-inspired cinematic one-screen layout with an immersive left room scene, polished right sidebar, and bottom action/evidence panels
- Cinematic room transitions, typewriter-style narration, and soft camera zoom effects when clues are discovered
- Ambient generated antique-shop music, suspense tones in important rooms, optional mute button, and generated sound effects
- Asset-based illustrated backgrounds and character sprites for the antique shop, storage room, upstairs office, Bonnie, and Mabel, with warm lighting, shadows, rugs, clocks, shelves, cabinets, framed photos, music boxes, and antique clutter
- Visible glowing hotspot rings, many examine objects and hidden clue surfaces, short hover descriptions, and smooth Bonnie walk-to-object movement
- Quest Notes journal that updates automatically as Bonnie discovers real clues and red herrings
- Inventory for collected clues
- Investigation Board that visually connects Evelyn Blackwood, Hollow Oak Estate, the music box, torn photograph, and hidden symbol
- Upstairs Office locked-drawer puzzle unlocked by the Brass Key
- Hidden wall safe with a four-digit code-breaking puzzle built from clues across multiple rooms
- Timed atmospheric lightning, power flicker, and hidden hallway shadow event
- Browser save/load system using local storage
- Fixed-width centered desktop layout that keeps the full scene, slim side panels, inventory, quest notes, and room navigation visible without horizontal or vertical scrolling on standard desktop monitors

## How to run

Open `index.html` in any modern web browser.

For a local development server, run:

```bash
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

> Note: Browser audio starts after the first player interaction, which keeps the game compatible with modern autoplay rules. Saved games are stored only in the current browser with local storage.
