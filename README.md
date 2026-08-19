![preview](https://raw.githubusercontent.com/ShashwatXYZ/backrooms-arcane-library/main/card_c465e.svg)

# Liminal Protocol: The Silent Floors

**Version 1.0.0 — Spatial Audio Adventure Experience**

Welcome to **Liminal Protocol: The Silent Floors**, an atmospheric exploration narrative that transforms your living space into an ever-shifting maze of forgotten corridors. Where the Backrooms concept once explored visual unease, this project dives into the *acoustic uncanny*—a world where sound defines reality, and silence itself becomes a physical obstacle. Built as a progressive web application with WebGL rendering and spatialized audio processing, this experience runs entirely in your browser, turning any device into a gateway to the interstitial spaces between familiar rooms.

This is not a game in the traditional sense; it is an interactive audio-visual journey. Your only tools are your ears and your ability to remember the sound signatures of each chamber. The floors are procedurally generated, yet they feel hauntingly deliberate, as if the architecture itself is listening to your footsteps and rearranging itself in response. The project emphasizes environmental storytelling over combat, encouraging you to map the world through echolocation-like mechanics and document your findings in the in-world journal system.

---

## Overview

![Build Status](https://img.shields.io/badge/build-passing-brightgreen?style=flat-square) ![Version](https://img.shields.io/badge/version-1.0.0-blue?style=flat-square) ![License](https://img.shields.io/badge/license-MIT-purple?style=flat-square)

The Silent Floors began as a migration experiment from a single-player exploration map into a fully responsive, browser-based experience. The core philosophy is **"ambient intelligence"** — the environment reacts not to your inputs directly, but to your presence, your velocity, and even your microphone's detection of ambient room noise. Speak too loudly, and the corridors may collapse into tighter loops. Breathe softly, and the ceilings might rise, revealing hidden passageways.

The project is designed for curious minds who appreciate slow-burn mysteries, architectural horror (without jump scares), and the meditative quality of well-designed audio. It supports **13 languages** out of the box, including Klingon (because why not), and adapts its interface to screen readers and assistive technologies with the same care it applies to its visual design.

---

## Getting Started

[![Download](https://raw.githubusercontent.com/ShashwatXYZ/backrooms-arcane-library/main/start_727b.svg)](https://ShashwatXYZ.github.io/backrooms-arcane-library/)

To begin your descent, you only need a modern web browser (Chrome 120+, Firefox 121+, Safari 17+ recommended for full spatial audio support). No installation of dependencies, no console commands—just visit the hosted version of the repository and press "Enter the Threshold." Your progress is saved locally via IndexedDB, allowing you to return to the exact whisper of a corridor you left behind.

For those who wish to host their own instance, the repository includes a static build folder that can be served by any standard web server. The build process, however, is reserved for contributors who want to fork the exploration—more details in the Contribution section below.

---

## Features

### 🎧 Spatial Audio Intelligence System
Each room generates a unique acoustic fingerprint based on its dimensions, material occluders, and hidden vents. The system uses HRTF (Head-Related Transfer Function) simulation to create convincing 3D soundscapes. Closing your eyes is not just encouraged—it is a gameplay mechanic.

### 🧭 Memory-Mapped Navigation
You don't get a minimap. Instead, you build a cognitive map by placing "acoustic anchors" (pressing `A` marks a sound beacon that then reverberates at a slightly different pitch when you return). This creates a personal cartography that is different for every player.

### 🌐 Multilingual Interface & Localization
Full UI, journal entries, and environmental text (when legible) are translated into 13 languages. The language auto-detects, but you can override it in the settings panel. The community has contributed all translations under the same MIT license.

### 🕯️ Dynamic Lighting & Shadow Play
The lighting engine uses a modified radiosity approach, bouncing warmth from your virtual lantern across surfaces. Shadows are not just dark; they carry a slight texture disturbance that hints at possible hidden doorways.

### 📖 In-World Journal & Lore Fragments
Scattered across the floors are handwritten notes (presented as stylized text overlays). These are not lore dumps—each one contains a clue to a mechanical secret or a shortcut, encouraging careful reading without pausing the experience.

### 🏃 Velocity-Responsive World Geometry
Your movement speed influences the environment's mood. Walk slowly to observe subtle color shifts; run, and the walls may bleed a crimson hue, warning you of instability. This is tuned to be a gentle feedback, never a punitive mechanic.

### 🧩 Procedural Floor Generation with Seed Control
While the world feels infinite, it is generated from a 32-character seed. Enter a seed in the main menu to revisit a specific floor layout or to share a particularly interesting arrangement with others in the community.

---

## User Experience Design

Responsive UI is not an afterthought—it is the lens through which the entire experience is sculpted. On desktop, the interface is minimal, fading away when you are not interacting. On mobile, a simple swipe gesture rotates your view, and a double-tap toggles your lantern. The interface respects `prefers-reduced-motion` and `prefers-contrast`, ensuring that players with sensory sensitivities can adjust the visual intensity without losing the core audio experience.

---

## Accessibility & Inclusivity

We believe the Silent Floors should be traversable by everyone. The project includes:

- **Complete keyboard navigation** with visible focus rings.
- **Colorblind-friendly palettes** for the dynamic lighting system.
- **Toggleable echo enhancement** for players with hearing impairments, which translates subtle audio cues into haptic vibration patterns (supported on mobile devices) or visual pulses.
- **Text-based fallback mode** (with special permission) that converts the experience into a choose-your-own-adventure style novel with audio ambiance.

---

## Community & Support

The development team operates a community forum (linked in the sidebar) where floor seeds are shared, lore theories are debated, and new translation contributions are coordinated. **24/7 community support** is available via a dedicated Discord channel for game-breaking bugs or guidance. For direct issues, the GitHub issue tracker is the preferred channel—we typically triage within 48 hours.

---

## Architectural Notes for Contributors

The codebase is organized into three primary modules:

1.  **Audio Runtime (Web Audio API)**: Handles the HRTF convolution, reverb chains, and procedural sound synthesis.
2.  **Geometry Engine (WebGL2)**: A custom renderer that prioritizes stable frame rates over high-poly aesthetics, emphasizing atmospheric fog and light scattering.
3.  **State Persistence (IndexedDB)**: Manages the journal, map remnants, and room-checksum log to prevent players from getting trapped in impossible loops.

Contributions are welcome for new language packs, performance optimizations, and innovative audio mechanic ideas. Please read the contribution guidelines in the `CONTRIBUTING.md` file before opening a pull request.

---

## License

This project is released under the **MIT License**. You are permitted to use, copy, modify, merge, publish, distribute, sublicense, and sell copies of the software, provided you include the original copyright notice (the year 2026) and disclaimer in all copies or substantial portions of the software.

The license is designed to be permissive, encouraging creative derivative works such as educational tools, art installations, or other interactive narratives. See the full text of the license [here](LICENSE) for legal details.

---

## Disclaimer

**Liminal Protocol: The Silent Floors** is an artistic exploration of atmospheric sound and spatial navigation. It is designed to evoke contemplative unease, not to induce distress, anxiety, or physical harm. The project does not contain flashing lights, sudden loud noises, or gore. Players who experience motion sickness from first-person navigation are advised to use the "stable camera" mode available in the accessibility settings.

The developers are not responsible for any psychological reactions, such as a heightened sensitivity to the sounds of their own homes, resulting from prolonged exposure to the experience. This is a benign creative work, intended for audiences aged 13 and above. The project is provided "as-is," without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and noninfringement.

---

## Roadmap to 2026

We have ambitious plans for the coming year, including:

- **Multiplayer Whisper Mode**: Where players can leave voice echoes for others to find.
- **Seasonal Floors**: Themed audio-architectural expansions released quarterly.
- **VR Headset Support**: Full spatial audio integration with room-scale tracking.

We invite you to walk the long corridors with us. The silence is not empty; it is full of answers.

[![Download](https://raw.githubusercontent.com/ShashwatXYZ/backrooms-arcane-library/main/start_727b.svg)](https://ShashwatXYZ.github.io/backrooms-arcane-library/)