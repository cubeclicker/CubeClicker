# CubeClicker

A high-performance, browser-based 3D clicker and idle game engineered using **Three.js**, **Tailwind CSS**, and **Firebase Firestore**. Built with a modular architecture, the application features real-time cloud persistence, dynamic physics-based animations, and a responsive reactive UI.

---

## Architecture & Technical Stack

* **Rendering Engine:** [Three.js](https://threejs.org/) (WebGL-based 3D graphics renderer handling lighting, meshes, grid helpers, and camera transformations).
* **Cloud Database:** Firebase Firestore (real-time data synchronization and persistent user scores via anonymous or token-based authentication).
* **Styling:** Tailwind CSS (utility-first styling for the asynchronous UI layout and modal overlays).
* **Core Logic:** Vanilla ES6+ JavaScript implementing custom spring-back physics, dynamic gravitational acceleration scaling, and state management.

---

## Features

* **3D Physics & Visual Feedback:** Every click triggers a smooth physics-based jump calculation, dynamic camera tracking, color shifts, and recoil impulses.
* **Real-Time Cloud Synchronization:** User progress and click counts are automatically synchronized and persisted using Firebase Firestore document snapshots.
* **Achievement & Rank Systems:** A progressive tier system ranging from *Recruit* to *Death Lord*, complete with unlockable milestone badges and dynamic notification toasts.
* **Cheat Code Integration:** Hidden input mechanics allowing easter eggs and developer testing (`HACKRBAND`).

---

## Project Structure

```text
├── index.html          # Complete single-file application containing markup, styling, Three.js logic, and Firebase integration
└── README.md           # Professional project documentation

```

---

## Getting Started

### Prerequisites

To run this project locally, you only need a modern web browser and a local development server (due to ES6 module imports and Firebase security policies).

### Installation & Execution

1. Clone the repository or copy the code into an `index.html` file.
2. Serve the file using a local static server (e.g., [VS Code Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) or Python's built-in server):
```bash
python3 -m http.server 8000

```


3. Open your browser and navigate to `http://localhost:8000`.

---

## Configuration

Firebase credentials and project configurations are dynamically injected via `__firebase_config` and `__app_id` globals if hosted within an integrated platform, or can be supplied directly in the initialization routine.

---

## License

This project is licensed under the [MIT License](https://www.google.com/search?q=LICENSE).
