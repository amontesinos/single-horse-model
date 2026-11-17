# The Single Horse Model

A self-contained, offline-capable HTML presentation illustrating a four-dimensional horse-shaped extrusion and its three-dimensional orthographic projection.

Open `index.html` in a browser. No dependencies or network requests are required for the interactive model. The external Flatland reference opens only when selected.

## Controls

- Scrub the rotation slider or use Play rotation.
- Choose the x–w, y–w, or z–w rotation plane.
- Drag horizontally to orbit (mouse users can also drag vertically); arrow keys work when the canvas is focused.
- Switch between the horse and a tesseract.
- Select a projection specimen to inspect its angle.
- Download HTML creates a portable copy of the complete page.

## Geometry

The horse is a union of convex 3D meshes. Each is extended over w ∈ [−0.58, +0.58], rotated in 4D, and projected by dropping w. The projected solid is the union of the 3D convex hulls of each component's projected endpoint vertices. The source diagram uses an oblique projection to reveal the fourth direction.

This is a geometric thought experiment, not empirical evidence that real horses share a single higher-dimensional source. It distinguishes projections from cross-sections and documents the limits of the analogy.

## Editing and deployment

The entire app is in `index.html`; no build step is needed. GitHub Pages serves the root of the `main` branch. `.nojekyll` ensures the files are served directly.

The page includes a Download HTML button for saving an offline copy.

## Validation

JavaScript syntax checked. Geometry checked across all three rotation planes at −90°, −65°, −35°, 0°, 35°, 65°, and 90°: finite vertices, convex outward faces, closed manifold meshes, Euler characteristic, the zero-angle projection identity, and tesseract endpoint bounds. A tesseract has 16 vertices and 32 edges. Desktop and 390px phone layouts, shape selection, specimen selection, animation, rotation planes, keyboard orbit, reset, and HTML download were inspected in a browser.
