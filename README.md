
# Wacky Tube Battle 🎈🥊

> "The QWOP of Inflatable Fighting Games."

A chaos-driven physics fighting game where you control an inflatable tube man. Built entirely in vanilla JavaScript with no external game engines.

## 🎮 How to Play
The goal is simple: **Slap the other tube man.**

1.  **Controls:** The screen is split into two touch zones.
    * **Hold Left:** Activates the left fan (pushes you Right).
    * **Hold Right:** Activates the right fan (pushes you Left).
    * **Alternate:** Tap rhythmically to build momentum and flail your arms.
2.  **Combat:**
    * **Headshots:** Hitting the opponent's head deals critical damage.
    * **Wind Up:** You must build velocity to hurt the enemy. Gentle touches won't do damage.

## 🛠 Tech Stack
* **Engine:** Custom 2D Verlet Integration (Constraint Solver).
* **Rendering:** HTML5 Canvas API.
* **Input:** Pointer Events API (Mouse & Touch unified).
* **Dependencies:** ZERO. None.

## 🏗 Setup
1.  Clone the repo.
2.  Open \`index.html\` in any modern browser.
3.  That's it. No build step required.

## 💡 The Physics Behind It
The game uses a **Point-Stick system**:
1.  **Points:** Invisible dots that have mass and respond to gravity/wind.
2.  **Sticks:** Rigid constraints that keep points at fixed distances.
3.  **The "Tube":** A spine of 14 points connected by sticks.
4.  **The "Wind":** A variable force vector applied to the spine points, simulating air pressure from the base fan.

## 📱 Mobile Optimization
The game uses a fixed-width gap logic for spawning characters, ensuring that whether you are on an iPhone Mini or an iPad Pro, the enemy is always within slapping range.
