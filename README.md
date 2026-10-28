# Hyperforge V1

**Draw it. Solve it. Race it.**

Hyperforge V1 is a self-contained browser-based futuristic hover-racing game and track maker. Draw a circuit in 2D, let the solver turn it into a banked 3D raceway, add race modules and scenery, choose a pilot, then race the result directly in your browser.

Everything runs from a single HTML file with no installation, build system, external assets, or game engine required.

![Hyperforge V1 race](assets/mobile-race-01.png)

## Features

- **Draw your own circuits** — sketch a closed route and convert it into a playable 3D track.
- **Automatic 3D track solving** — banking, elevation, slopes, bridges and separated crossings are generated from the route.
- **START + PIT module** — a combined starting grid, red-light gantry and pit lane/service area.
- **Boost tunnels** — place boost sections around the course and trigger them while racing.
- **Up to 10 racers** — choose from ten alien, robot and creature pilots with brightly coloured dart-style hovercraft.
- **Arcade opponent AI** — rivals use individual racing lines, lane movement and passing behaviour instead of staying in a fixed formation.
- **Low-hover handling** — craft sit close to the surface and visibly follow banked track edges.
- **Damage and shields** — barrier contact and craft collisions affect the race, with pit-lane shield charging.
- **Custom track appearance** — choose road, shoulder and edge treatments.
- **Deep-space scenery** — planets, moons, stars, nebulae, asteroid belts and other sky options.
- **Keyboard, touch and controller support** — designed to work on desktop and mobile.
- **Save and load projects** — export editable Hyperforge project JSON files and continue later.
- **16-shot Track Tour** — automatically creates a single PNG contact sheet with cinematic cameras placed around a virtual lap, including the red-light starting grid, pit lane, boost tunnels, banks, crossings, high/low points and other useful track locations.
- **Track sketch reference** — the original 2D route is included underneath the Track Tour collage.

## Screenshots

### Racing

| Mobile race view | Race HUD |
| --- | --- |
| ![Mobile race](assets/mobile-race-01.png) | ![Race HUD](assets/mobile-race-02.png) |

### Pilots

![Pilot selection](assets/pilot-selection.png)

### 16-shot Track Tour

![Track tour example 1](assets/track-tour-01.png)

![Track tour example 2](assets/track-tour-02.png)

![Track tour example 3](assets/track-tour-03.png)

![Track tour example 4](assets/track-tour-04.png)

## How to run

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Draw a track, or use one of the ready-made examples.
4. Press **Build & check track**.
5. Add optional race pieces and customise the look.
6. Choose a pilot and start racing.

No local server is required for normal use.

## Basic controls

### Desktop

- **A / D** or **Left / Right arrows** — drive and steer.
- **Space** — drift / brake.
- **B** — boost while inside a boost tunnel.
- **P** — toggle pit assist.

### Touch

Use the large **LEFT**, **RIGHT**, **DRIFT / BRAKE** and **BOOST** controls beneath the race view.

### Controller

Hyperforge includes gamepad support and rebinding controls inside the game. The default layout uses shoulder/trigger or D-pad controls for steering, with face buttons for drift and boost.

## Track-building workflow

Hyperforge is organised into a simple five-step flow:

1. **Draw** — create the route and elevation zones.
2. **Solve** — turn the sketch into valid 3D race geometry.
3. **Race pieces** — add the combined START + PIT module and boost tunnels.
4. **Look** — customise track materials and the space environment.
5. **Play Game** — select a pilot, choose the race grid and race the course.

The maker also includes undo/redo, example tracks, save/load project support and geometry checks intended to catch invalid or overly sharp track designs before racing.

## 16-shot Track Tour

The Track Tour runs a virtual lap without normal race physics and captures sixteen distinct 3D locations around the course. It prioritises useful features such as:

- the full starting grid beneath red lights;
- the selected planet behind the start when possible;
- pit lane;
- boost tunnels;
- steep banks;
- bridges/crossings;
- highest and lowest track sections;
- steep climbs and descents;
- sharp bends;
- additional well-spaced trackside viewpoints.

The final PNG also includes the original track sketch as a route-plan reference.

## Project format

Saved courses are exported as editable JSON project files. They retain track geometry/settings so a design can be loaded back into Hyperforge and modified later.

## Browser support

A current desktop or mobile browser with Canvas and WebGL support is recommended.

## Status

**Hyperforge V1** is an experimental hobby project. Feedback, bug reports and unusual track designs are welcome — especially around handling, opponent AI, track solving, mobile controls and camera placement.

## Licence

Hyperforge V1 is released under the **MIT License**. See [LICENSE](LICENSE).
