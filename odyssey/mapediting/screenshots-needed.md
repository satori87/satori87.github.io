# Screenshots Needed for Odyssey Map Making Guide

All screenshots should be at least 800px wide. Save as PNG in the `img/` directory.

---

## index.html (1 screenshot)

### `img/ingame-finished-map.png`
**An in-game view of a finished Odyssey map.** Should show a nice-looking area with visible floor tiles, textured walls, object sprites (trees/barrels), and lighting. A good showcase of what a completed map looks like in 3D.

---

## getting-started.html (3 screenshots)

### `img/tiled-download-page.png`
**The Tiled download page at mapeditor.org.** Show the main download page with the platform options (Windows/Mac/Linux). Alternatively, just show the Tiled application window freshly opened.

### `img/tiled-interface-labeled.png`
**The Tiled editor interface with all major panels labeled.** Open an existing Odyssey map (like testmap or testmap2). Label/annotate the four key areas:
- **Map View** (center)
- **Layers panel** (top-right)
- **Tilesets panel** (bottom-right)
- **Properties panel** (left)

This is the most important screenshot in the tutorial. Use arrows or boxes to highlight each panel.

### `img/tiled-project-open.png`
**Tiled with the Odyssey project open.** Open `assets/tiled/odyssey-dungeon.tiled-project` and show the Project panel listing the map files. Should show how the project gives access to all maps and tilesets.

---

## creating-a-map.html (3 screenshots)

### `img/tiled-new-map-dialog.png`
**The "New Map" dialog in Tiled with correct settings.** Go to File > New > New Map and show the dialog with these settings highlighted/circled:
- Orientation: Orthogonal
- Tile layer format: CSV
- Tile render order: Right Down
- Tile size: 32 x 32 px

### `img/tiled-layers-panel.png`
**The Layers panel showing a well-organized map.** Show the Layers panel (top-right) with a map that has a good set of layers: Floor, Walls, Objects, Doors, Ceiling (tile layers) and Warps, Spawns, Properties (object layers). Both tile layer and object layer icons should be visible.

### `img/tiled-first-room.png`
**A simple first room in Tiled.** Show a 16x16 map with:
- Floor tiles filling the interior area
- Wall tiles forming the room perimeter
- A gap in the walls for a doorway
This should look like a basic room that a beginner would create as their first map.

---

## tile-layers.html (7 screenshots)

### `img/layer-floor.png`
**The Floor layer in Tiled.** Show the Floor tile layer selected, with brick or stone floor tiles painted across a room interior. The Layers panel should show "Floor" highlighted.

### `img/layer-floor2.png`
**The Floor2 overlay layer.** Show Floor2 with carpet or rug tiles placed on top of the base floor. Ideally show both the Tiled view and a small in-game view showing the carpet rendered on the ground.

### `img/layer-walls.png`
**The Walls layer.** Show wall tiles forming room boundaries with visible gaps for doorways. The Layers panel should show "Walls" selected. Good to show a room with clear wall layout.

### `img/layer-walls2.png`
**The Walls2 decoration layer.** Show Walls2 tiles (torches, shelf decorations, signs) placed on wall positions. If possible, also show the in-game result with decorations visible on the walls.

### `img/layer-objects.png`
**The Objects layer with sprites.** Show trees, barrels, furniture, or other doodad sprites placed on the Objects layer. In-game view showing the billboard sprites facing the camera would be great to include.

### `img/layer-doors.png`
**The Doors layer.** Show door tiles placed in wall gaps. If possible, include an in-game view showing a door in both open and closed states.

### `img/layer-ceiling.png`
**The Ceiling layer with height property.** Show the Ceiling tile layer selected, with the Properties panel visible on the left showing the custom `height` property set to a value like 2. The ceiling tiles should be painted across the indoor area.

---

## object-layers.html (9 screenshots)

### `img/layer-warps.png`
**A Warp zone in Tiled.** Show the Warps object layer with a rectangle drawn across a doorway or map edge. The Properties panel should display the `map`, `x`, `y` (and optionally `dir`) properties on the selected warp rectangle.

### `img/layer-spawns.png`
**A Spawn zone in Tiled.** Show the Spawns layer with one or more spawner rectangles. The Properties panel should show `SPAWN_ID`, `SPAWN_COUNT`, and `SPAWN_DELAY` on the selected spawner.

### `img/layer-nm.png`
**A No-Monster zone in Tiled.** Show the NM layer with rectangles drawn around a safe area (like a town center or near NPCs). No properties needed on the objects, just the rectangles.

### `img/layer-keep.png`
**A Keep zone in Tiled.** Show the Keep layer with a rectangle covering a guild hall safe area. Similar to NM but specifically for a guild building context.

### `img/layer-locks.png`
**A Lock zone overlapping a door.** Show the Locks layer with a rectangle aligned to a door tile position. The Properties panel should display the `lock` property (e.g., set to `"guild"` or a key ID). Make sure the rectangle clearly overlaps the door.

### `img/layer-tp.png`
**A Touchplate zone in Tiled.** Show the TP layer with a rectangle drawn near the floor (the pressure plate area). The Properties panel should display `x` and `y` properties. Ideally show the locked door that the touchplate points to elsewhere on the map (maybe with an arrow annotation).

### `img/layer-bootmap.png`
**A Bootmap zone in Tiled.** Show the Bootmap layer with a rectangle covering a dungeon area. The Properties panel should show `map`, `x`, and `y` properties.

### `img/layer-items.png`
**Item spawns in Tiled.** Show the Items layer with small objects/points placed on the map. The Properties panel should show `item_id` and `qty` on a selected item. Show a few different items (weapon, gold, potion) if possible.

### `img/layer-wallheight.png`
**A WallHeight override zone.** Show the WallHeight object layer with a rectangle and its `height` property set to 2 or 3. If possible, show the in-game result with taller walls in that area.

---

## map-properties.html (1 screenshot)

### `img/layer-properties.png`
**A Properties object with all settings.** Show a Properties layer object selected, with the Properties panel displaying several properties: `name`, `indoors`, `pk` or `friendly`, `ambient`, `cantattackmonsters`, and `music`. This should be a clear view of how to configure map settings.

---

## advanced.html (5 screenshots)

### `img/advanced-roofs.png`
**The Roof system in Tiled and in-game.** Show both:
1. Tiled view with the Roof tile layer (painted with roof texture tiles) and the Roof object layer (rectangle with `roof_dir`, `roof_angle`, `hip` properties visible)
2. In-game view of the generated 3D roof

Bonus: Show both a hip roof and a gable roof side by side for comparison.

### `img/advanced-wallheight.png`
**Variable wall heights.** Show:
1. Tiled view with a WallHeight rectangle (height=2 or 3)
2. In-game view with the noticeably taller walls in that region compared to normal height-1 walls nearby

### `img/advanced-lights.png`
**Point lights in Tiled and in-game.** Show:
1. Tiled view with Lights object layer and light point objects with `intensity`, `color`, and `flicker` properties
2. In-game view of a dark room illuminated by warm torch lights

### `img/advanced-fx.png`
**Particle effects placement.** Show:
1. Tiled view with FX object layer and effect placements with `fx` property
2. In-game view showing the particle effects active (fire, smoke, etc.)

### `img/advanced-walls2-dir.png`
**Walls2 directional control.** Show:
1. Tiled view with the Walls2 tile layer (torch tiles) and the Walls2 object layer with a `dir` property rectangle
2. In-game view showing how the torch decoration only appears on the specified face direction

---

## coordinate-reference.html (2 screenshots)

### `img/coords-tiled-system.png`
**Tiled coordinate display.** Show the Tiled editor with the mouse hovering over a tile, with the coordinate readout visible in the status bar at the bottom. Annotate or highlight where the X,Y tile coordinates are displayed. Label the origin (0,0) at the top-left corner.

### `img/coords-visual-comparison.png`
**Tiled vs in-game coordinate comparison.** Side-by-side:
- Left: Tiled map view with a few tile positions labeled (e.g., "Tiled (5, 2)")
- Right: In-game 3D view of the same area with the corresponding world positions labeled
Shows how the Y axis flips between the two systems.

---

## Summary

| Page | Count | Filenames |
|------|-------|-----------|
| index.html | 1 | ingame-finished-map |
| getting-started.html | 3 | tiled-download-page, tiled-interface-labeled, tiled-project-open |
| creating-a-map.html | 3 | tiled-new-map-dialog, tiled-layers-panel, tiled-first-room |
| tile-layers.html | 7 | layer-floor, layer-floor2, layer-walls, layer-walls2, layer-objects, layer-doors, layer-ceiling |
| object-layers.html | 9 | layer-warps, layer-spawns, layer-nm, layer-keep, layer-locks, layer-tp, layer-bootmap, layer-items, layer-wallheight |
| map-properties.html | 1 | layer-properties |
| advanced.html | 5 | advanced-roofs, advanced-wallheight, advanced-lights, advanced-fx, advanced-walls2-dir |
| coordinate-reference.html | 2 | coords-tiled-system, coords-visual-comparison |
| **Total** | **31** | |
