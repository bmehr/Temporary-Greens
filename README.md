# 🛹 Temporary Greens ⛳️

> An arcade skater meets technical 3D driving range simulation built for the web.

**Temporary Greens** puts you in the sneakers of a beverage-sipping skater with an iron slung across his back, cruising down the cart path on his way to hit balls at the driving range. Avoid course hazards on your commute, then dial in your club selection, read the wind, and aim for the pins (or hit the ball picker cart) in a cel-shaded 3D driving range.

---

## 🎮 Play Directly in Your Browser

This game is designed as a zero-dependency, single-file web app optimized for both desktop browsers and mobile touch screens:

- **Live URL:** `https://<your-username>.github.io/<repo-name>/`

---

## ✨ Features

### Phase 1: The Commute (2D Side-Scroller)
- **Authentic Rubber-Hose Character Art:** Hand-crafted vector silhouette matching the original *Temporary Greens* character (backwards cap, drink in hand, slung iron, ripped jeans, and kicked skateboard deck).
- **Smooth Skate Mechanics:**
  - **Ollie:** Pop over stray golf ball baskets, traffic cones, and carts.
  - **Duck:** Slide low under hanging willow branches and course signage.
  - **Push:** Kick for extra speed down the cart path.
- **Dynamic Golf Course Hazards:** Multiple randomized ground and overhead obstacles.
- **Audio Synthesis:** Built-in Web Audio API sound effects for rolling wheels, pops, landings, and crashes.

### Phase 2: The Driving Range (3D Sim)
- **Cel-Shaded / Ink Aesthetic:** 3D fairway powered by [Three.js](https://threejs.org/) maintaining the high-contrast comic-strip visual identity.
- **Aerodynamic Ball Flight Model:** Realistic loft, speed, backspin (Magnus effect lift), and side-spin hooks/slices.
- **Club Bag:**
  - `1W` (Driver)
  - `3W` (3-Wood)
  - `5I` (5-Iron)
  - `7I` (7-Iron)
  - `9I` (9-Iron)
  - `PW` (Pitching Wedge)
- **Environmental Factors:** Dynamic wind vectors (speed & compass direction) affecting ball flight and carry.
- **Target Greens & Moving Targets:**
  - Concentric circular target greens at 50, 100, 150, 200, 250, and 300 yards.
  - An animated range ball picker cart patrolling the fairway (hitting it scores a 500-point direct-hit bonus!).
- **Classic 3-Click Swing Gauge:**
  1. Click 1: Start power gauge
  2. Click 2: Lock power
  3. Click 3: Snap timing (dead-center for straight shots, edges create draws/fades/slices)
- **Dynamic Tracer Camera:** Follow camera that tracks the ball through the sky with an illuminated shot tracer.

---

## 🕹️ Controls

### Desktop Controls

| Action | Phase 1 (Skate Run) | Phase 2 (Driving Range) |
| :--- | :--- | :--- |
| **Ollie / Jump** | `Space`, `W`, or `↑` | — |
| **Duck / Slide** | `S` or `↓` (Hold) | — |
| **Push / Boost** | `D` or `→` | — |
| **Swing / Meter** | — | `Space` or Click **Hit Ball** |
| **Club Select** | — | Click club pill buttons (`1W` - `PW`) |

### Mobile Controls
- **Phase 1:** On-screen arcade buttons for **DUCK**, **PUSH**, and **OLLIE**.
- **Phase 2:** Responsive touch buttons for club selection and swing execution.

---

## 🚀 Setting Up on GitHub Pages

1. **Fork or clone** this repository to your GitHub account:
   ```bash
   git clone https://github.com/<your-username>/temporary-greens.git
   cd temporary-greens
   ```
2. Make sure the primary game file is named `index.html` in the root folder.
3. Push to your `main` (or `master`) branch:
   ```bash
   git add .
   git commit -m "Initial Temporary Greens commit"
   git push origin main
   ```
4. In your GitHub repository:
   - Go to **Settings** > **Pages** (in the left-hand sidebar).
   - Under **Build and deployment** > **Source**, choose **Deploy from a branch**.
   - Select `main` (or `master`) and `/ (root)`.
   - Click **Save**.
5. Wait a few moments, and your game will be live at:
   `https://<your-username>.github.io/<repo-name>/`

---

## 🛠️ Tech Stack

- **HTML5 Canvas & 2D Context:** Custom vector rendering and procedural rigging for the skater.
- **Three.js (r128):** 3D fairway environment, lighting, meshes, and ball camera tracking.
- **Tailwind CSS (CDN):** Responsive UI, overlays, HUD, and mobile controls.
- **Web Audio API:** Zero-asset procedural audio generation (synthesized road rumble, clicks, strikes, and chimes).

---

## 📄 License

MIT License. See [LICENSE](LICENSE) for details.