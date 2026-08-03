# Cooja Positioner v2026 - browser-based geo-scenario editor 2026

> **Cooja Positioner runs entirely in the browser and helps you craft Cooja-ready and multi-simulator mobility layouts from real-world geography, including on-device editing and exports aimed at everyday WSN and IoT toolchains.**

[![Platform](https://img.shields.io/badge/Platform-web%20browser-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/henry-wagner1964/cooja-geo-positioner?style=flat-square)](https://github.com/henry-wagner1964/cooja-geo-positioner)

---

<p align="center">
  <a href="https://henry-wagner1964.github.io/cooja-geo-positioner/">
    <img src="https://img.shields.io/badge/Download-Cooja%20Positioner%20Latest-brightgreen?style=for-the-badge" alt="Download Cooja Positioner">
  </a>
</p>

> **[Direct Download - Cooja Positioner v2026](https://henry-wagner1964.github.io/cooja-geo-positioner/)**

---

[Download Latest Build](https://henry-wagner1964.github.io/cooja-geo-positioner/)

---

## What is Cooja Positioner?

Cooja Positioner is a map-first web editor for turning geographic ideas into position and mobility inputs your simulators can consume. It targets researchers and engineers who use Cooja or related WSN/IoT stacks and want to place nodes, sketch motion, and handle coordinates visually instead of maintaining a separate desktop utility.

All editing stays in the client. You can compose point and polygon layouts, mix fixed and moving nodes, and attach timed waypoints in a single session. The same workspace covers WGS84, ECEF, and ENU conversions and helps you bridge Cooja position files with mobility traces for ns-2, ns-3, and INET/OMNeT++.

---

## What you can do

- Edit full scenarios in-browser on the client
- Author layouts on a map with points and polygons
- Place both static and mobile nodes
- Build motion paths from waypoints and timestamps
- Choose a custom WGS84 origin for geo-based work
- Convert coordinates along the WGS84 to ECEF to ENU path
- Write Cooja `positions.dat` exports
- Produce mobility files for ns-2, ns-3, and INET/OMNeT++
- Step backward and forward through edits with undo/redo
- Select and adjust multiple nodes together
- Bring existing Cooja position data back into the editor

---

## Getting it running

Because Cooja Positioner is a browser application, day-to-day use does not require a classic installer.

For a local checkout:

1. Clone or download this repository.
2. Serve the project with any browser-friendly web server, or open the published build.
3. Start the app in your browser and create or load a scenario.

Example:

- `git clone https://github.com/henry-wagner1964/cooja-geo-positioner.git
- open the web app from your local server or from the published build

---

## How to work with it

A common path looks like this:

1. Launch the editor in the browser.
2. Establish or tweak the WGS84 origin for the scene.
3. Drop points, polygons, static nodes, and mobile nodes onto the map.
4. When motion matters, attach waypoints and timestamps.
5. Refine with undo, redo, and multi-select as needed.
6. Export either a Cooja position file or mobility output for another simulator.

Supported export destinations include:

- Cooja `positions.dat`
- ns-2 mobility files
- ns-3 mobility files
- INET/OMNeT++ mobility files

---

## Scenario settings

Configuration lives mainly inside the editor as you build. The geographic origin that drives coordinate conversion is the central knob.

You will typically control:

- WGS84 origin
- imported position data
- whether nodes are static or mobile
- waypoint timing
- which export format to emit

For scenarios you plan to reuse, record the origin and coordinate conventions next to the files you export.

---

## Requirements

- Modern web browser
- JavaScript turned on
- Either the repo files or the published build available
- Local storage or workspace capacity for saved exports

Suggested setup:

- Up-to-date desktop browser
- Wider display for comfortable map editing
- Working knowledge of Cooja, WSN/IoT setups, or mobility file formats

---

## FAQ

**Where do I obtain the newest build?**  
Follow the download link near the top, or open the published build directly.

**Is a local install mandatory for editing?**  
No. The workflow is meant to run inside a web browser.

**Can Cooja position files be loaded again?**  
Yes. You can import existing Cooja position data and keep editing.

**Are mobile nodes part of the model?**  
Yes. Mobile nodes plus waypoints and timestamps are included.

**How do I change the geographic reference point?**  
Set a custom WGS84 origin before you convert or export.

**Exports look wrong in my simulator—what next?**  
Confirm format choice, origin, and coordinate assumptions, then compare the file with what your target simulator expects.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
