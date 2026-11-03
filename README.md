# 🪁 Patangbaazi: Lapet Re Lapet! (2D Kite Battle)

[![HTML5 Canvas](https://img.shields.io/badge/Canvas-HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-v3.0-38B2AC?style=flat&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Web Audio API](https://img.shields.io/badge/Web_Audio_API-Synthesized_BGM-blue)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> An addictive, nostalgic 2D Indian rooftop kite battle arcade game inspired by the festivities of Makar Sankranti and Uttarayan! Fly your diamond *patang*, engage in intense thread clashes against neighborhood rivals, dodge flying pigeons, and scream **"लपेट रे लपेट!"** across the mohalla!

---

## 🎮 Live Demo & Gameplay Preview

- **Play in Browser**: Simply open `index.html` in any web browser on desktop or mobile.
- **Controls**: Intuitive touchpad/finger direct gliding + dedicated two-thumb **KHINCH!** and **DHEEL** action buttons.

---

## ✨ Features

- **🪁 Realistic Aerodynamic Kite Physics**:
  - Authentic diamond kite anatomy featuring the central wooden bamboo spine (*Thadda*), curved tension bow (*Kampa*), and dynamic waving ribbon tail (*Poonchh*).
  - Catenary string bending rendering originating from the rooftop kid's charkhi (spool).

- **✂️ Deep "Khinch" & "Dheel" Clash Mechanics**:
  - **KHINCH! (⚡ Pull Attack)**: Rapid upward slicing attack to sever rival strings.
  - **DHEEL (💨 String Release)**: Relieves string friction by ~60% and catches wind currents to slip out of dangerous tangles.

- **🗣️ Desi Rooftop Voice Shouts (Web Speech API)**:
  - Shouts authentic Hindi rooftop slogans:
    - Slicing a rival kite: **"लपेट रे लपेट!"** (*Lapet Re Lapet!*)
    - Giving Dheel: **"ढील दे दे रे!"** (*Dheel de de re!*)
  - Interactive rooftop comic speech bubbles displayed directly on screen.

- **🎵 Procedural Makar Sankranti Folk Theme Song**:
  - 100% synthesized using the **Web Audio API** (no external audio files required).
  - Festive Indian pentatonic folk melody (*Raga Bhupali / Bilawal*) backed by energetic syncopated **Dholak ("धिन-ता")** percussion beats at a preset 75% master volume mix.

- **🏙️ Rooftop Rivals & Sky Hazards**:
  - Battle iconic neighborhood rivals: **Pinku**, **Sharma Ji**, **Bunty**, and **Guddu Bhaiya**.
  - Dodge flocking pigeons (**🕊️ Kabootar**) that damage and snap your *manja*.
  - Collect air-dropped parachutes:
    - 🔥 **Bareilly Ka Manja**: Ultra-sharp glass-coated string for instant cuts.
    - 🧆 **Tilgul Laddoo**: Repairs +35% Manja Life.
    - 💨 **Tez Hawa Boost**: High-speed velocity burst.

- **📱 Fully Responsive & Mobile-First**:
  - Touchpad glide & mobile screen swipe controls.
  - Corner-aligned, thumb-accessible arcade action buttons.

---

## 🕹️ Controls Guide

| Action | Laptop / Desktop | Mobile / Touchscreen |
| :--- | :--- | :--- |
| **Steer Kite** | Mouse glide / Trackpad drag / `W` `A` `S` `D` / Arrow Keys | Tap & drag finger anywhere on screen |
| **KHINCH (Attack)** | `Space` or Click **KHINCH** (Bottom Left) | Tap **⚡ KHINCH!** (Bottom Left) |
| **DHEEL (Defense)**| `Shift` or Click **DHEEL** (Bottom Right) | Tap **💨 DHEEL** (Bottom Right) |
| **Toggle Music** | Click `🎵 SONG: ON/OFF` in top bar | Tap `🎵 SONG: ON/OFF` |
| **Toggle Voice** | Click `🗣️ VOICE: ON/OFF` in top bar | Tap `🗣️ VOICE: ON/OFF` |
| **Mute Sound** | Click `🔊 / 🔇` in top bar | Tap `🔊 / 🔇` |

---

## 📖 Rules of Engagement

1. **How to Cut Rival Kites:**
   - Move your kite into the vicinity of an opponent's kite until sparks (`⚡`) appear.
   - Press and hold **KHINCH!** to rapidly deplete their string health.
   - When their meter hits 0: **"लपेट रे लपेट!"** — their kite tumbles down to the colony below and your cut score increases.

2. **How to Protect Your Manja:**
   - Your kite starts with **100% Manja Life**.
   - If trapped in a losing angle, tap **DHEEL** to slip away with the wind.
   - Avoid collision with flying pigeons (kabootar), which deliver an instant 18% string integrity penalty.
   - Collect floating **Tilgul Laddoos** to repair damaged string.

---

## 🚀 How to Run Locally in VS Code

### 1. Prerequisites
- [Visual Studio Code](https://code.visualstudio.com/)
- Any modern web browser (Google Chrome, Brave, Edge, or Safari)

### 2. Setup Steps
1. Clone or download this repository:
   ```bash
   git clone https://github.com/your-username/patangbaazi-kite-battle.git
   cd patangbaazi-kite-battle
   ```
2. Open the project folder in VS Code:
   ```bash
   code .
   ```
3. Run the game:
   - **Method A (Easiest)**: Double-click `desi_auto_game.html` (or `index.html`) to open it directly in your browser.
   - **Method B (Live Server)**:
     1. Install the **Live Server** extension (`ms-vscode.live-server`) in VS Code.
     2. Right-click the `.html` file and click **"Open with Live Server"**.

> **Note on Browser Audio**: Browsers require a user interaction before playing sound. Click the **"UDAO PATANG!"** button on the start screen to initialize the synthesized dholak song, cutting SFX, and speech synthesis.

---

## 🛠️ Tech Stack & Architecture

- **Single-File Architecture**: Clean, standalone code combining HTML, Tailwind CSS, and vanilla JavaScript without bundler dependencies.
- **Rendering Engine**: HTML5 2D Canvas rendering at 60 FPS using `requestAnimationFrame`.
- **Audio Synthesizer**: Web Audio API (`AudioContext`, `OscillatorNode`, `GainNode`) for procedural sound synthesis and procedural BGM loops.
- **Voice System**: Web Speech API (`SpeechSynthesisUtterance`) with automatic `hi-IN` Hindi / Indian accent locale detection.
- **Persistence**: Browser `localStorage` for tracking high scores and personal records across sessions.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and share!

---

<p align="center">
  Made with ❤️ for Indian kite lovers & street festival enthusiasts.<br>
  <b>लपेट रे लपेट! 🪁</b>
</p>
