# Daata Hamlet Residence - 3D viewer

Interactive 3D model of the ground floor (REV-04), with both stair options (L and U).
Works on phones: drag to turn, pinch to zoom, tap a room for its size and area.

Two pages:
- `index.html` - the standalone 3D model viewer (plan view, cut-plane, viewpoints).
- `earth.html` - the same model dropped onto a 3D globe over real satellite imagery
  (CesiumJS + free Esri World Imagery, no API key). Open it, paste the plot's
  latitude/longitude, and drag **Heading** to line the house up with the image.
  Note: the free satellite imagery softens when zoomed in to house scale - that is a
  limitation of the free imagery, not the model. (Google's sharper Photorealistic 3D
  Tiles are a paid Maps Platform product and would need a billed API key.)

## Put it online with GitHub Pages
1. Create a new public repository on github.com, for example `daata-hamlet-3d`.
2. Upload the three files in this folder: `index.html`, `DH-GF-L.glb`, `DH-GF-U.glb`
   (Add file > Upload files > Commit).
3. Settings > Pages > Source: "Deploy from a branch", branch `main`, folder `/ (root)` > Save.
4. After a minute the viewer is live at `https://<your-username>.github.io/daata-hamlet-3d/`.

To update the model later, regenerate the .glb files (`DH_STAIR=L python build_3d.py blend`) and upload them again.
