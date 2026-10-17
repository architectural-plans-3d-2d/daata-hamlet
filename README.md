# Daata Hamlet Residence - 3D viewer

Interactive 3D model of the house: ground floor (REV-04), second floor (REV-01), roof and mumty,
with both stair options (L and U).
Works on phones: drag to turn, pinch to zoom, tap a room for its size and area.

- **Floor switch:** Ground / Second / Whole house. In Ground and Second, the walls are cut at the slider height.
- **Viewpoints:** whole house, street view, the ground-floor rooms, and the second-floor lounge, TV lounge + balcony and master bedroom.
- **Open/Close car gate:** slides the 11'-3" gate into its wall pocket.

Files: `index.html`, `DH-L.glb` (L stair), `DH-U.glb` (U stair).
Live at https://architectural-plans-3d-2d.github.io/daata-hamlet/

To update the model, regenerate the .glb files (`DH_STAIR=L python build_3d.py blend`, then `U`) and push them.
