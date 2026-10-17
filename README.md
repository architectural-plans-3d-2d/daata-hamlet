# Daata Hamlet Residence - 3D viewer

Interactive 3D model of the house: ground floor (REV-04), second floor (REV-01), roof and mumty,
with both stair options (L and U).
Works on phones: drag to turn, pinch to zoom, tap a room for its size and area.

- **Floor switch:** Ground / Second / Whole house. In Ground and Second, the walls are cut at the slider height.
- **Viewpoints:** whole house, street view, the ground-floor rooms, and the second-floor lounge, TV lounge + balcony and master bedroom.
- **Open/Close car gate:** slides the 11'-3" gate into its wall pocket.

Two pages:
- `index.html` - the 3D model viewer (ground / second floor / whole house, cut-plane, viewpoints).
- `earth.html` - the same model dropped onto a 3D globe over real satellite imagery
  (CesiumJS + free Esri World Imagery, no API key). Open it, paste the plot's
  latitude/longitude, and drag **Heading** to line the house up with the image.
  Note: the free satellite imagery softens when zoomed in to house scale - that is a
  limitation of the free imagery, not the model. (Google's sharper Photorealistic 3D
  Tiles are a paid Maps Platform product and would need a billed API key.)

Files: `index.html`, `earth.html`, `DH-L.glb` (L stair), `DH-U.glb` (U stair). The models are meshopt-compressed (~270 KB each) for phones.
Live at https://architectural-plans-3d-2d.github.io/daata-hamlet/

To update the model, regenerate the .glb files (`DH_STAIR=L python build_3d.py blend`, then `U`) and push them.
