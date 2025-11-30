# 🎮 KORBLOX: Roblox Baseplate Simulator (Multiplayer)

A browser-based 3D simulation of a classic Roblox baseplate, built using **Three.js** and enabled for **real-time multiplayer** using the **Firebase Realtime Database**.

## ✨ Features

* **Real-time Multiplayer:** Players in separate browser tabs or on different computers see each other's custom avatars move instantly.
* **Roblox-style Character:** A fully articulated block-style avatar with walking animations.
* **Physics:** Basic gravity and ground collision detection.
* **First-Person Building:** Switch to First-Person view and use the Left Mouse Button (LMB) to place blocks on a grid.
* **Controls:** Classic WASD movement, jumping, and running.

## 🕹️ How to Play

### Controls
| Key | Action |
| :--- | :--- |
| **W/A/S/D** | Move Forward, Left, Backward, Right |
| **SHIFT** | Run (Hold) |
| **SPACE** | Jump |
| **C** | Toggle Camera View (Third-Person / First-Person) |
| **I / O** | Zoom Camera In / Out (in Third-Person) |
| **LMB (Click)** | Place Block (in First-Person mode) |

### Multiplayer Instructions
1.  Open the live game URL in your browser.
2.  Share the same URL with a friend.
3.  When both of you are playing, you will see each other's avatars moving in real-time!

## 💻 Technical Stack

* **3D Rendering:** [**Three.js**](https://threejs.org/) (JavaScript library)
* **Styling:** [**Tailwind CSS**](https://tailwindcss.com/) (Used for the UI panel)
* **Real-Time Data:** [**Firebase Realtime Database**](https://firebase.google.com/docs/database) (Used for player synchronization)
* **Hosting:** **GitHub Pages** (Static web hosting)

## ⚙️ Setup and Configuration

This project is a single-file application (`index.html`) that works out of the box after deployment.

### Firebase Connection

The multiplayer capability is powered by a connection to a live Firebase project. The configuration keys are embedded directly in the `index.html` file:

```javascript
// Your web app's Firebase configuration
const firebaseConfig = {
    apiKey: "AIzaSyAIrLIjpvfqtLl7BNHHkWQ6QUh1L93Mys8",
    authDomain: "testroblox-495d6.firebaseapp.com",
    projectId: "testroblox-495d6",
    // ... other keys
};
