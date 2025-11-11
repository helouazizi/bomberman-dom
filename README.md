# 💣 Bomberman DOM – Multiplayer Edition

A **multiplayer Bomberman-style game** built entirely using my own **custom mini-framework** (without Canvas or WebGL).  
This project focuses on performance, real-time synchronization, and multiplayer gameplay using **WebSockets**.

---

## 🎯 Objectives

The goal of this project is to build a **real-time multiplayer Bomberman game** that runs smoothly at **60 FPS**, where **2 to 4 players** compete to be the last one standing.  
Each player starts in a different corner of the map, places bombs, destroys blocks, collects power-ups, and battles others until only one remains.

---

## 🕹️ Game Overview

### 👥 Players
- Supports **2 to 4 players**.
- Each player starts in a **different corner** of the map.
- Each player has **3 lives**.
- The last surviving player **wins** the match.

### 🧱 Map
- The **entire map** is visible to all players.
- **Walls** are fixed and indestructible.
- **Blocks** are randomly generated and can be destroyed with bombs.
- **Power-ups** can appear after destroying blocks.
- Starting areas are safe zones — players can escape their own bomb explosions.

### 💥 Power-ups
When a block is destroyed, a random power-up may appear:

| Power-up | Effect |
|-----------|---------|
| 💣 **Bomb** | Increases the number of bombs a player can drop simultaneously by +1 |
| 🔥 **Flame** | Increases the explosion range by +1 block in all directions |
| ⚡ **Speed** | Increases the player's movement speed |

---

## 💬 Multiplayer & Chat

The multiplayer system and chat are powered by **WebSockets**.

### Connection Flow:
1. Players enter a **nickname** on the login screen.  
2. They are redirected to a **waiting room** with a **player counter (0–4)**.  
3. Game starts when:
   - At least **2 players** join and **10 seconds** pass after the 20-second mark, **or**
   - **4 players** join before 20 seconds.  
4. Players can **chat in real-time** during gameplay.

---

## ⚙️ Performance Requirements

Performance is a **core aspect** of this project:

- Game must run **at least 60 FPS** at all times.
- Use of **`requestAnimationFrame`** is mandatory.
- **No frame drops** allowed.
- Real-time updates and animations must remain **smooth and synchronized**.
- Use of **developer tools (Chrome/Firefox)** for performance measurement and debugging.

---

## 🧩 Technologies Used

| Technology | Purpose |
|-------------|----------|
| **HTML / CSS / JavaScript (Vanilla)** | Core game logic and UI |
| **Custom DOM Framework** | Rendering and element management (built in a previous project) |
| **WebSockets** | Real-time multiplayer synchronization and chat |
| **requestAnimationFrame** | Game loop and animations |
| **SVG / DOM elements** | Game visuals and map rendering (no Canvas or WebGL) |

---

## 🚀 Game Flow

1. **Login Page:**  
   Player enters nickname → joins waiting room.  

2. **Waiting Room:**  
   Displays a live **player counter (2–4)** and a **countdown** timer.  

3. **Game Start:**  
   All players spawn on the map corners. The game begins once the timer finishes.  

4. **Gameplay:**  
   - Move around the map.  
   - Drop bombs and avoid explosions.  
   - Collect power-ups to gain advantages.  
   - Lose a life if caught in an explosion.  
   - Game ends when only one player remains alive.  

5. **End Game:**  
   Display winner and option to play again.  

---

## 🔧 Developer Notes

- Built **without Canvas or WebGL**.  
- Uses **DOM manipulation only** via a custom framework.  
- Focused on **performance, synchronization, and smooth animation**.  
- Real-time communication handled via **WebSockets**.  
- FPS and performance can be monitored using browser **developer tools**.

---

## 📈 Learning Outcomes

This project helped me gain deep understanding of:

- ⚙️ `requestAnimationFrame` and game loop optimization  
- ⏱️ Animation performance and frame rate measurement  
- 🔄 Event loop and asynchronous execution  
- 🌐 WebSocket real-time communication  
- 🧩 Framework architecture and DOM rendering optimization  
- 💬 Synchronization between multiple players and clients  

---

## 🏁 Future Improvements

- Add **multiple map layouts**  
- Introduce **AI players (bots)**  
- Add **sound effects** and **explosion animations**  
- Improve **UI design** with custom skins  
- Implement **leaderboards** and **match history**

---

## 👨‍💻 Author

**Developed by:** [Your Name]  
🎓 Zone01 Oujda  
💬 Contact: [Your Email or Portfolio Link]  

---


---

## 🧠 Concepts Reinforced

- **Performance-first programming**  
- **Real-time multiplayer architecture**  
- **DOM-based rendering and updates**  
- **Client synchronization via WebSockets**  
- **Game state management**  

---

## 🕹️ “The last one standing wins!”

💣 Have fun playing, building, and learning from the **Bomberman DOM Multiplayer** project!


