# Bonnie's Quest

A single-file, browser-based cinematic cozy mystery adventure inspired by classic point-and-click games like King's Quest.

## Current features

- Title screen introducing the larger Hollow Oak Estate mystery
- Three explorable rooms: Main Antique Shop, Back Storage Room, and Upstairs Office
- Classic point-and-click Bonnie movement with walkable floor limits, object approach points, smooth facing, and idle/walking poses
- Expanded Mabel dialogue interactions with branching choices, clue reveals, deliberate misdirection, the missing heirloom, the old town fire, and the secret ledger
- Missing antique collector Evelyn Blackwood and a hidden family secret tied to Mabel's Antiques
- Reference-inspired cinematic one-screen layout with an immersive left room scene, polished right sidebar, and bottom action/evidence panels
- Clean room transitions and typewriter-style narration without camera zoom or dark grading over the photographs
- Ambient generated antique-shop music, rain bed, ticking clocks, creaking wood, soft room tone, suspense tones in important rooms, optional mute button, and generated sound effects
- Image-based adventure room architecture: all three rooms prefer uploaded realistic room plates and keep generated CSS furniture only as a missing-asset fallback
- Realistic photographic clarity pass that layers Bonnie, Mabel, clue props, and invisible interaction zones over the room photographs without artificial fog, rain overlays, blur filters, or dark masking
- Invisible point-and-click hotspot regions layered over the room art, with labels and subtle glints appearing only on hover, keyboard focus, or Bonnie proximity
- Subtle hover/focus glow rings, object-name tooltips, short hover descriptions, and smooth Bonnie walk-to-object movement without shifting the imported room plates
- More realistic high-detail Bonnie sprite with improved proportions, face shading, room-matched shadowing, idle breathing, and smoother walking animation over the static room background
- Quest Notes journal that updates automatically as Bonnie discovers real clues, multi-step object interactions, final-compartment evidence, and red herrings
- Inventory for collected clues with selectable inspection, item-on-hotspot use, and item combination puzzles
- Inventory combinations and item-on-object puzzle chains including old key + receipt + music box, torn photograph + hidden symbol, old key + office drawer, and lantern + dark storage corner
- Investigation Board that visually connects Evelyn Blackwood, Hollow Oak Estate, the music box, torn photograph, and hidden symbol
- Upstairs Office locked-drawer puzzle unlocked by the Old Key
- Hidden wall safe with a four-digit code-breaking puzzle built from clues across multiple rooms
- Deeper puzzle chain with a locked drawer, lamp-revealed message, antique clock cipher, hidden wall safe, and final wall compartment containing Evelyn's secret ledger
- Timed atmospheric lightning, power flicker, and hidden hallway shadow event
- Browser save/load system using local storage
- Fixed-width centered desktop layout that keeps the full scene, slim side panels, inventory, quest notes, and room navigation visible without horizontal or vertical scrolling on standard desktop monitors

## Asset folders

Game assets are organized by purpose so future replacements are easier to maintain:

- `assets/backgrounds/` — room plates and background fallback art
- `assets/props/` — collectible objects and character sprites
- `assets/ui/` — interface portraits, markers, and other UI artwork
- `assets/audio/` — music, ambience, and sound-effect files

## Using organized asset folders and uploaded realistic room images

Place the provided antique room images in `assets/backgrounds/` using these filenames so the game loads them as the actual in-game environments without generating replacement room art:

- `assets/backgrounds/main-antique-shop.webp` (or `.jpg` / `.png`)
- `assets/backgrounds/storage-room.webp` (or `.jpg` / `.png`)
- `assets/backgrounds/upstairs-office.webp` (or `.jpg` / `.png`)

The browser automatically uses the first matching realistic plate it can load. Bonnie, Mabel, prop callouts, invisible hotspots, and interaction zones are layered on top of those backgrounds while preserving the photographic room clarity. The existing SVG room art remains only as a development fallback if the uploaded images are not present.

## How to run

Open `index.html` in any modern web browser.

For a local development server, run:

```bash
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

> Note: Browser audio starts after the first player interaction, which keeps the game compatible with modern autoplay rules. Saved games are stored only in the current browser with local storage.
