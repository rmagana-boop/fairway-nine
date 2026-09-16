# Canvas/Vibe Integration Notes

- Prefer SVG files for dynamic overlays because they scale without blur.
- Use transparent PNGs for golfer/tree/prop sprites.
- Use terrain tiles as fills/textures clipped to procedural world polygons; never stretch one tile over the whole viewport.
- Use the `golfer_pose_atlas_reference.png` and `tree_atlas_reference.png` only as reference/fallback; individual PNGs are the preferred runtime assets.
- Camera depth: scale sprites by projected depth, then depth-sort. Fade distant layers slightly toward sky blue.
- Putting overlays should be transformed onto the green plane and computed from actual slope/pace data.
