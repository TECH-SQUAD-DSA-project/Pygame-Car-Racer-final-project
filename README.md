# 🏎️ Racing Game Project by TECH SQUAD

Welcome to our Pygame Racing Game Series! This repository contains four progressively complex racing game projects, each building upon the previous. These projects explore Pygame fundamentals, AI path-following, collision mechanics, and level-based gameplay progression.

---

## 📦 Project 1: Basic Track Drawing

### 📌 Overview
This project sets the foundation by displaying the racetrack and background using Pygame. It handles window creation, image loading, and initial rendering.

### 🛠️ Features
- Loads images: grass, track, finish line, track borders.
- Displays all images centered and scaled appropriately.
- Establishes `WIDTH`, `HEIGHT`, and frame rate (FPS).

### 📚 Key Learning
- Using `pygame.image.load()` and `blit()`.
- Managing layers: track above grass, borders on top, etc.
- Resizing and scaling images.

### 🐞 Glitches / Limitations
- Static screen — no interaction.
- No car, movement, or AI yet.

### ✅Strengths:
- Nice use of OOP with abstract car and player-specific car.
- Smooth rotation + acceleration logic.
- Clean drawing and frame handling with clock.tick(FPS).

---

## 🚗 Project 2: Player Car Movement

### 📌 Overview
This project adds a **player-controlled car**. You can now drive using the `W`, `A`, `S`, `D` keys and see real-time movement with rotation.

### 🛠️ Features
- Adds `AbstractCar` and `PlayerCar` classes.
- Implements rotation and velocity.
- Physics-like movement using `math.cos/sin` and angles.

### 📚 Key Learning
- Creating custom classes with inheritance.
- Managing movement with acceleration and friction.
- Rotating surfaces and blitting with angle.

### 🐞 Glitches / Issues Faced
- No collision — you can drive off the track.
- No AI or goal — just drive freely.

---

## 🧠 Project 3: AI Car + Collision Detection

### 📌 Overview
The game now has an **AI car** that follows a pre-defined path. Collision detection is introduced using Pygame masks, adding gameplay challenge.

### 🛠️ Features
- `ComputerCar` follows a hardcoded path using angle calculation.
- Both cars detect collisions with the track border using masks.
- Player car "bounces" on collision.

### 📚 Key Learning
- Using `pygame.mask.from_surface()` and `mask.overlap()` for pixel-perfect collision.
- Controlling AI with `calculate_angle()` toward waypoints.

### 🐞 Glitches / Issues Faced
- AI sometimes misses path points at sharp turns.
- No win/loss conditions — the game doesn't end.

---

## 🏁 Project 4: Levels, Timer, and Game Loop

### 📌 Overview
This version introduces **levels**, a **timer**, and **win/lose mechanics**. The AI gets faster each level, and you must finish first to progress.

### 🛠️ Features
- `GameInfo` class manages levels and timers.
- Game pauses at the start of each level waiting for user input.
- AI speed increases slightly with each level.
- Messages shown for losing, winning, and starting.

### 📚 Key Learning
- Managing game state (levels, wins, resets).
- Blocking loops for user input (e.g. wait for key press).
- Scaling difficulty with level progression.

### 🐞 Glitches / Issues Faced
- AI still uses the same path for every level.
- If the player or AI gets stuck, the game doesn’t end.
- No saving progress — everything resets on game restart.

---

Thanks for checking out our Racing Game projects! 🎮

Feel free to fork and extend any version — maybe add laps, boost items, or smarter AI!

