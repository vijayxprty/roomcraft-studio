# Roomcraft Studio
Free, browser-local 2D and 3D concept planner for homes and shops. No account, backend, API key or paid dependencies.

## Run
Serve `dist` with any static web server, e.g. `python3 -m http.server 8080 --directory dist`, then visit http://localhost:8080. Opening index.html directly is not supported because ES modules require HTTP.

## Features
- Home, shop and blank starters; searchable library of 33 procedural furniture and fixture assets.
- Drag furniture onto the 2D plan; draw rectangular rooms and straight axis-aligned walls; edit dimensions, positions, colours and rotation.
- Named levels with editable elevation, including basement, ground, upper floors and rooftop; selected or stacked 3D views.
- Orbit and seven camera presets, including ceiling/bottom; optional ceilings.
- PNG current view, ZIP with seven 3D angles and every floor plan plus project JSON, WebM orbit video where MediaRecorder is supported.
- Local autosave, editable JSON import/export, undo/redo and metric/imperial display.
- Vendored Three.js (MIT). Fonts are optional Google Fonts with local fallbacks.

## Hosting on GitHub Pages
Push this repository to GitHub. In Settings → Pages choose GitHub Actions. The included workflow publishes `dist` when the main branch changes. No build needed. The `.openai` folder is only for the optional Sites deployment and is not needed for GitHub Pages.

## Scope and limits
This is a concept planner, not architectural CAD. Room walls use a dollhouse presentation (two full walls and two low walls). Doors/windows are standalone assets and do not boolean-cut wall openings. Rooms are rectangular; custom walls can be combined. Furniture is procedural, not photorealistic. No structural, code compliance, electrical, plumbing or staircase clearance validation. Exports reflect the current geometry and visibility options; bottom/ceiling inspection hides floor slabs and shows the ceiling undersides. Videos use the active visible tab and browser capabilities. Projects stay in the visitor's own browser; no shared accounts, cloud synchronization or server storage. Local storage can be cleared by the browser, so download JSON backups. No commercial cost guarantee is made for third-party hosting limits.

## License
App source: MIT, see LICENSE. Three.js license: dist/vendor/THREE-LICENSE.txt.
