# Fairway Nine — Visual Asset Pack v1.0

This pack is designed for **Vibe Apps / Microsoft Power Apps Canvas** to replace primitive generated vector art with a coherent premium 2.5D golf-game visual language.

## Recommended use
- Treat these files as the **canonical visual assets**. Do not recreate the golfer, trees, course props, or HUD art from circles/rectangles.
- Keep procedural **world geometry and physics** in code, but skin the world with these assets.
- Use the golfer pose PNGs as animation keyframes/states. Crossfade or interpolate position/scale/rotation between states rather than redrawing the character.
- Use tree PNGs as world sprites: scale by camera depth, vary size/flip, depth-sort, add dynamic ground shadow, and fade distant instances.
- Terrain tiles are texture references for fairway/rough/green/fringe/sand/path surfaces. Apply them inside perspective course geometry rather than as flat screen bands.
- Use mountains, hills, sky, and clubhouse as layered parallax scenery.
- Use effect assets only when the corresponding gameplay event occurs.
- Putting graphics must stay attached to actual green slope/aim physics.

## Key folders
`01_golfer` swing/putting poses and avatar reference
`02_equipment` clubs, balls, tees, flags/cup
`03_terrain` surface textures
`04_course_elements` bunkers, water, rocks, vegetation, bridge/fence
`05_trees` ten tree/shrub families
`06_backgrounds` parallax layers
`07_effects` tracer/impact/divot/sand/water/shadow
`08_putting` aim/break/slope/cup/target/contour graphics
`09_ui` HUD/control/minimap atlases and example composition

## Important
The source boards in `00_reference` define the intended overall art direction. The production crops are intentionally modular so the course can remain procedural.
