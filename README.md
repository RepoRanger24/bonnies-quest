# Bonnie's Quest

A single-file, browser-based cinematic cozy mystery adventure inspired by classic point-and-click games like King's Quest.

## Current features

- Title screen introducing the larger Hollow Oak Estate mystery
- Three explorable rooms: Main Antique Shop, Back Storage Room, and Upstairs Office
- Classic point-and-click Bonnie movement with walkable floor limits, object approach points, smooth facing, and idle/walking poses
- Expanded Mabel dialogue interactions with branching choices, clue reveals, deliberate misdirection, the missing heirloom, the old town fire, and the secret ledger
- Missing antique collector Evelyn Blackwood and a hidden family secret tied to Mabel's Antiques
- Reference-inspired cinematic one-screen layout with an immersive left room scene, polished right sidebar, and bottom action/evidence panels
- Cinematic room transitions, typewriter-style narration, and soft camera zoom effects when clues are discovered
- Ambient generated antique-shop music, rain bed, ticking clocks, creaking wood, soft room tone, suspense tones in important rooms, optional mute button, and generated sound effects
- Image-based adventure room architecture: all three existing rooms now use cinematic full-scene art layers instead of relying on CSS-drawn furniture
- Realistic cinematic visual pass with local photographic-style antique-shop room plates, semi-realistic Bonnie/Mabel character assets, subtle dust motes, warm volumetric light, window-limited rain streaks, vignette grading, and dark wood/brass UI styling
- Invisible point-and-click hotspot regions layered over the room art, with labels and subtle glints appearing only on hover, keyboard focus, or Bonnie proximity
- Subtle hover/focus glow rings, object-name tooltips, short hover descriptions, smooth Bonnie walk-to-object movement, and gentle camera drift
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

## How to run

Open `index.html` in any modern web browser.

For a local development server, run:

```bash
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

> Note: Browser audio starts after the first player interaction, which keeps the game compatible with modern autoplay rules. Saved games are stored only in the current browser with local storage.
