# Bonnie's Quest

A single-file, browser-based cozy mystery adventure inspired by classic point-and-click games like King's Quest.

## Current features

- Title screen with intro story text and a Start Quest button
- Three explorable rooms: Main Antique Shop, Back Storage Room, and Upstairs Office
- CSS-painted cozy antique shop visuals with richer wood and wall textures
- Ambient generated antique-shop music with an optional mute button
- Subtle generated sound effects for drawer opening, paper pickup, clock ticking, and footsteps between rooms
- Hover glow effects and short hover descriptions for clickable objects
- Inventory for collected clues
- Quest Notes journal that updates automatically as Bonnie discovers clues
- Upstairs Office locked-drawer puzzle unlocked by the Brass Key
- Drawer reveal containing an old handwritten letter, a strange symbol, and a clue about The Hollow Oak Estate
- Dust particles floating through light beams and subtle flickering lights
- A misleading clue/red herring and a hidden hotspot for careful explorers
- Responsive desktop-friendly design

## How to run

Open `index.html` in any modern web browser.

For a local development server, run:

```bash
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

> Note: Browser audio starts after the first player interaction, which keeps the game compatible with modern autoplay rules.
