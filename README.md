# The Single Horse Model

An interactive, Flatland-inspired thought experiment: one connected four-dimensional octopus-horse, roughly sixty million horse-shaped tentacles, and the three-dimensional cross-sections we call horses.

**[Open the website](https://amontesinos.github.io/single-horse-model/)**

The revised model uses cross-sections, replacing the earlier shadow/projection model. The hand-through-paper analogy explains why separate intersections can belong to one connected object. Octopus arm control and different fingerprints inspire the behavioral and variation analogies; the page distinguishes those analogies from biological evidence.

## Controls

- Switch between the horse creature and fingers through paper.
- Move the slice from outside the object, through separate branches, to the shared body.
- Reveal or hide the connecting structure.
- Compare varied coats/builds or finger widths with matching samples.
- Animate local horse behavior at a fixed fourth-dimensional coordinate.
- Select a horse to highlight its corresponding branch.
- Drag the herd to orbit; arrow keys work when the canvas is focused.
- Reset the lab or download a complete offline HTML copy.

## Geometry

The procedural horse consists of convex 3D mesh components. Each branch T_i is defined by a continuous family of 3D horse profiles P_i(w):

    T_i = { (x, y, z, w) : (x, y, z) belongs to P_i(w), 0 <= w <= 1 }

At a chosen coordinate s, the lab renders the intersection T_i with w = s. Profiles grow from tips, remain at separate locations through the middle range, then converge in position, scale, build, orientation, and local movement to a common core at s = 1. Consequently the connected 4D union has disconnected 3D sections at intermediate coordinates. Six example branches represent the proposed millions.

The left illustration is a schematic of connections, not a literal 4D view. The right panel renders the actual 3D profiles. Animation changes ordinary time while leaving w fixed; w is an extra spatial coordinate, not time. Hand mode uses five idealized finger branches that converge into one rounded palm section.

## Running and deployment

Open `index.html` in a browser. All styles, geometry, and scripts are included; no build step, runtime dependencies, or network requests are required. External research references open only when selected.

GitHub Pages serves the repository root on `main`. `.nojekyll` serves the static files directly.

## Validation

JavaScript syntax and geometric invariants are checked: no intersection before the tips, six disjoint horse sections and five finger sections at the default slice, coincident branches at the shared core, finite coordinates across 808 slice/time/variation configurations, continuous slice boundaries, and distinct smooth local animation. Browser checks cover desktop and 390px layouts, mode switching, slider endpoints, variation, connection visibility, horse selection, animation, keyboard orbit, reset, and offline download.

## Sources and scope

The page links the UN's horse-population estimate, primary research on octopus arm control and chemotactile sensing, and Abbott's *Flatland* (1884). This is a constructed geometric thought experiment, not empirical evidence that real horses are one organism. The fingerprint analogy illustrates variation within a whole; it does not explain genetic differences between horses.
