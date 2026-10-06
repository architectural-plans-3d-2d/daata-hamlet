# Daata Hamlet Residence - 3D viewer

Interactive 3D model of the ground floor (REV-04), with both stair options (L and U).
Works on phones: drag to turn, pinch to zoom, tap a room for its size and area.

## Put it online with GitHub Pages
1. Create a new public repository on github.com, for example `daata-hamlet-3d`.
2. Upload the three files in this folder: `index.html`, `DH-GF-L.glb`, `DH-GF-U.glb`
   (Add file > Upload files > Commit).
3. Settings > Pages > Source: "Deploy from a branch", branch `main`, folder `/ (root)` > Save.
4. After a minute the viewer is live at `https://<your-username>.github.io/daata-hamlet-3d/`.

To update the model later, regenerate the .glb files (`DH_STAIR=L python build_3d.py blend`) and upload them again.
