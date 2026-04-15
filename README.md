# 🛸 NEON RAIDER: REGENESIS

**Neon Raider: Regenesis** is a high-octane, single-file survival shooter built with the HTML5 Canvas API. Defend your core against an endless onslaught of geometric space-junk and hostile interceptors in a glowing, 360-degree synthwave battlefield.

![Play Now](https://www.newsignlabs.in/portfolio/web/neon-raider-html5-game)
---

## 🕹️ Gameplay & Controls

You are the pilot of a **Starforce Interceptor** stationed at a fixed defensive point. Threats converge from the periphery of deep space. Your mission: survive as long as possible.

* **Aim:** Move your mouse/touch to rotate the ship 360°.
* **Fire:** Click or Tap to engage neon disruptor beams.
* **Move:** Use `WASD` or `Arrow Keys` for micro-maneuvers to dodge incoming collisions.

### 💎 Power-Ups & Entities

| Type | Visual | Effect |
| :--- | :--- | :--- |
| **Energy Core** | 🟡 Gold Square | Activates **Triple-Shot** spread for 6 seconds. |
| **Repair Kit** | 🟢 Green Hexagon | Instantly restores **Hull Integrity to 100%**. |
| **Enemy Junk** | 💗 Pink Octagon | Standard threat. Destroy for points. |

---

## 🛠️ Technical Architecture

This project serves as a case study in **Zero-Asset Game Development**. It contains no external PNGs, JPEGs, or sound libraries—everything is rendered procedurally via code.

### Key Features:
* **Radial Spawning Logic:** Obstacles utilize polar coordinates to spawn outside the viewport and calculate trajectories toward the screen center using `Math.atan2`.
* **Procedural Vector Sprites:** The spaceship is drawn using mathematical paths (`lineTo`, `bezierCurveTo`) rather than static images, allowing for infinite scaling without pixelation.
* **Efficient Entity Management:** An automated "Clean-Up" loop filters arrays to remove off-screen bullets and destroyed particles, maintaining a consistent 60 FPS.
* **Neon Aesthetics:** Heavy use of `shadowBlur` and `CanvasGradients` to mimic the "bloom" effect of 80s arcade monitors.

---

## 🚀 How to Run

Because the game is contained within a single HTML file, deployment is instant:

1.  **Download** the `index.html` file from this repository.
2.  **Open** it in any modern web browser (Chrome, Firefox, Safari, Edge).
3.  **Deploy to GitHub Pages:** * Push the file to a repository.
    * Go to **Settings > Pages**.
    * Select the branch and click **Save**. Your game is now live!

---

## 📜 Development Case Study

The core engine was developed with a focus on **Edge Reading Engineering**:
* **Collision Detection:** Uses Euclidean distance formulas rather than bounding boxes for "pixel-perfect" circular hit detection.
* **Particle Physics:** On destruction, entities shatter into a "Particle System" where each fragment has its own velocity, gravity-drag, and alpha-decay properties.

---

## 📄 License

This project is open-source and available for free. Feel free to fork, mod, and expand the Neon universe!

---

*Developed with 💖 by ![Newsign Labs](www.newsignlabs.in).*
