# Forge3D — Browser 3D Game Studio

A mobile-friendly starter 3D scene editor built with HTML, CSS, JavaScript modules and Three.js.

## Run it

Three.js modules are loaded from jsDelivr, so an internet connection is required. Because browsers restrict ES modules on `file://`, serve this folder from a local or hosted web server.

### Quick local server

If Python is installed:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

On Android, you can upload the folder to a static hosting provider (for example GitHub Pages, Netlify, or Cloudflare Pages) and open the published URL. Keep `index.html`, `styles.css`, and `app.js` together in the same folder.

## Features

- Three.js real-time 3D viewport with orbit, pan and zoom
- Create cube, sphere, cylinder, plane, cone and torus primitives
- Move, rotate and scale with TransformControls (W/E/R shortcuts)
- Scene hierarchy and object inspector
- Position, rotation, scale, color, roughness, metalness and wireframe controls
- Add point lights and cameras
- Import GLB, GLTF, OBJ, STL, FBX and common image textures
- Save/open editable `.forge3d` project JSON files
- Export the current scene as GLB
- JavaScript script editor with `.js` download (scripts are stored, not executed)
- Preview mode, grid/axes toggles, shadow toggle and responsive mobile layout

## Notes / current limitations

This is a functional starter editor, not a full Unity/Unreal replacement. The timeline is currently a UI placeholder; there is no animation authoring, physics simulation, terrain sculpting, multiplayer, asset marketplace, or runtime game packaging yet. Imported external model assets are included in GLB export, but the `.forge3d` project file currently stores editable primitive/object transforms and basic material properties rather than embedding imported model binaries. Imported image textures are also not embedded in project JSON.
