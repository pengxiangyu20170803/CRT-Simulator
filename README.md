# CRT-Simulator

# README.md

---

# 🚇 Chongqing Rail Transit (CRT) Driving Simulator 2026

**A full-featured, single‑file 3D driving simulator for Chongqing’s metro network, built with Three.js.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Three.js](https://img.shields.io/badge/Three.js-r160-blue)](https://threejs.org/)
[![Status](https://img.shields.io/badge/status-stable-brightgreen)]()
[![Data](https://img.shields.io/badge/data-2026.08-informational)]()

---

## 🌟 Overview

**CRT Simulator 2026** is an immersive, browser‑based driving simulation for the Chongqing Rail Transit network. It leverages Three.js to create a realistic 3D environment with procedural terrain, dynamic weather, and a full physics‑based train model.

**Key highlights:**
- 🗺️ **Full network coverage** – all 14 operational lines as of August 2026 (1, 2, 3, 4, 5, 6, 9, 10, 18, Loop, Expo, Airport, Jiangtiao, and Bishan–Tongliang lines).
- 🏙️ **Famous landmarks** – Liziba “train-through-building”, multiple Yangtze/Jialing river bridges, and the steepest 45‰ gradient at Tongyuanju.
- 🎮 **Authentic driving experience** – ATO (automatic) / manual driving with ATP overspeed protection, emergency brake, and realistic door controls.
- 🌦️ **Dynamic environment** – day/night cycle, clear/fog/rain weather, and a procedural audio engine (traction, wheel‑rail, braking, horn).
- 🔊 **Chinese voice announcements** – station arrival/departure announcements using the Web Speech API.
- 📊 **Performance scoring** – stop precision, ride comfort, punctuality, and rule compliance, with a final star rating.

---

## 🕹️ Controls

| Key               | Action                           |
|-------------------|----------------------------------|
| `W` / `↑`         | Increase traction (throttle)     |
| `S` / `↓`         | Increase braking                 |
| `A` / `D`         | Release handle (coast)           |
| `Space`           | Emergency brake                  |
| `R`               | Release emergency brake          |
| `Q`               | Open left doors                  |
| `E`               | Close doors                      |
| `C`               | Toggle ATO / manual              |
| `H` (hold)        | Horn                             |
| `L`               | Toggle headlights                |
| `V`               | Cycle camera views               |
| `1` / `2` / `3`   | Weather: clear / fog / rain      |
| `T`               | Cycle time of day                |
| `P`               | Pause / resume                   |
| `F`               | Toggle fullscreen                |
| `M`               | Toggle left/right panels         |

You can also drag the **traction/brake levers** on the HUD, or use the on‑screen buttons (especially for touch devices).

---

## 🛠️ Technology Stack

- **3D Engine** – [Three.js](https://threejs.org/) r160
- **Physics** – custom train dynamics with jerk‑limited acceleration, gradient resistance, and ATP look‑ahead.
- **Audio** – WebAudio synthesizer (no external sound files required).
- **Voice** – Web Speech API (Chinese Mandarin).
- **Data** – station coordinates, line profiles, and historical facts compiled from public sources (accurate as of August 2026).

---

## 📁 Project Structure

Since this is a **single‑file application**, all code is contained in `index.html`.  
The main components are:

```plaintext
index.html                 # Full application (HTML + CSS + JavaScript)
README.md                  # This file
