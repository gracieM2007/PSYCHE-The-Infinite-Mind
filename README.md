# 🧠 PSYCHE: The Infinite Mind

> *An immersive, minimalist HTML5 Canvas experience exploring the vast expanse of human consciousness.*

[![Live Demo on Render](https://img.shields.io/badge/Render-Live%20Demo-00f2ff?style=for-the-badge&logo=render&logoColor=white)](https://psyche-the-infinite-mind.onrender.com)
[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/gracieM2007/PSYCHE-The-Infinite-Mind)

[![HTML5 Canvas](https://img.shields.io/badge/Canvas-HTML5-orange.svg)](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)
[![JavaScript](https://img.shields.io/badge/Language-ES6%2B%20JavaScript-yellow.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](#license)
[![Device Support](https://img.shields.io/badge/Platform-Desktop%20%7C%20Mobile-brightgreen.svg)](#controls)

---

## 🌐 Live Demo & Instant Deployment

- ⚡ **Play Live on Render**: **[https://psyche-the-infinite-mind.onrender.com](https://psyche-the-infinite-mind.onrender.com)**
- 🚀 **Deploy Your Own Copy**: Click the button below to deploy your own instance to Render in 1 click:

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/gracieM2007/PSYCHE-The-Infinite-Mind)

---

## 🌌 Overview

**PSYCHE: The Infinite Mind** is a visually stunning, ambient arcade web game built using native HTML5 Canvas 2D and ES6 JavaScript. Set within a glowing, interactive neural network, players pilot a core consciousness orb through abstract mindscapes, absorbing glowing thoughts while managing neural stress and evading hostile mental entities.

Designed with a modern glassmorphic UI overlay, dynamic time-dilation mechanics, responsive physics, and high-contrast glowing visual effects, **PSYCHE** delivers both intense arcade survival and relaxing meditative gameplay.

---

## ✨ Features

- **🎮 Dual Game Modes**:
  - **Initiate Survival**: A high-stakes race for higher expansion scores. Evade relentless, tracking neural threats; manage your **Neural Stress** meter before experiencing a **SYSTEM CRASH**.
  - **Zen State**: A soothing, meditative exploration mode with continuous RGB dynamic spectrum shifting, non-lethal threat impacts (bullet-time slowdowns), and zero game-over pressure.
- **⚡ Dynamic Physics & Visual Effects**:
  - Velocity-based squash & stretch core animations.
  - Motion trail effects and pulsing halo rings.
  - Matrix-style time dilation (slow-motion) upon hit impact or threat collision.
  - Screen shake and particle bursts for visceral feedback.
- **🧬 Interactive Neural Canvas**:
  - Dynamic neural synapses connect background nodes directly to your player core in real-time based on distance.
  - Color-shifting biomes that evolve every 1,000 points of Consciousness score.
  - Edge wrapping allowing seamless movement across screen boundaries.
- **🏆 Vision Board & High Score System**:
  - Integrated achievement slots unlocked at key score milestones:
    - 🌌 **500 Consciousness**
    - 🧬 **1500 Consciousness**
    - 💎 **3000 Consciousness**
  - Persistent high scores saved locally via browser `localStorage`.
- **📱 Universal Compatibility**:
  - Works seamlessly across all screen sizes with auto-resizing canvas.
  - Full support for both **Keyboard Navigation** and **Multi-touch / Gesture Controls**.

---

## 🕹️ Controls

| Platform | Action | Input |
| :--- | :--- | :--- |
| **Desktop** | Move Up | `W` or `Up Arrow` |
| **Desktop** | Move Down | `S` or `Down Arrow` |
| **Desktop** | Move Left | `A` or `Left Arrow` |
| **Desktop** | Move Right | `D` or `Right Arrow` |
| **Mobile / Touch** | Move Directionally | `Touch & Drag` anywhere on canvas |

---

## 🚀 Quick Start & Hosting

Because **PSYCHE** is built with zero external framework dependencies or build scripts, getting started takes seconds:

### 1. Play Online (Render)
Visit **[https://psyche-the-infinite-mind.onrender.com](https://psyche-the-infinite-mind.onrender.com)** to play directly in your browser.

### 2. Direct Local Open
Simply open [`index.html`](file:///c:/Users/DELL/OneDrive/Desktop/PSYCHE%20The%20Infinite%20Mind/index.html) or [`home.html`](file:///c:/Users/DELL/OneDrive/Desktop/PSYCHE%20The%20Infinite%20Mind/home.html) directly in any browser (Chrome, Edge, Firefox, Safari).

### 3. Local HTTP Server
Using Python:
```bash
python -m http.server 8000
# Open http://localhost:8000 in your browser
```

Using Node.js (`npx serve`):
```bash
npx serve .
# Open http://localhost:3000
```

---

## 🛠️ Tech Stack & Architecture

- **Rendering**: Pure HTML5 `<canvas>` using 2D Context API.
- **Styling**: CSS3 custom variables (`:root`), Glassmorphism (`backdrop-filter: blur()`), flexbox layout, ambient radial gradients.
- **Typography**: System font stack featuring modern geometric sans-serifs (`Inter`, `-apple-system`, `Segoe UI`).
- **Engine Architecture**:
  - Object-Oriented class structures (`Player`, `Thought`, `Threat`, `Particle`).
  - Delta time-scaled physics update loops driven by `requestAnimationFrame`.
  - Screen wrap boundaries, elastic friction algorithms, vector math collision detection.
  - Web Storage API integration (`localStorage.getItem('psyche_highscore')`).

---

## 📂 File Structure

```
PSYCHE The Infinite Mind/
├── index.html       # Primary static web server entry point
├── home.html        # Game application HTML5 source
├── render.yaml      # Render static site blueprint configuration
└── README.md        # Documentation with Live Demo & Render Deploy Button
```

---

## 🎨 Game Concepts & Entities

1. **Player Core**: The focal point of awareness. Responds to player direction with smooth velocity acceleration and friction decay.
2. **Thoughts (Collectibles)**: Pulsing golden/cyan energy orbs. Gathering thoughts awards **+50 Consciousness**, spawns particle effects, and advances biome progression.
3. **Neural Threats**: Hostile, segmented red organisms that actively track the core player in Survival Mode. Impacting a threat increases stress by 25%.
4. **Neural Stress Meter**: Displays system instability. At 100% capacity, the mind suffers a `SYSTEM CRASH`.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE). Feel free to modify, expand, and share!
