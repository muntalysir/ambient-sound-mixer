# 🎧 Ambient Sound Mixer

A sleek, professional ambient soundscape generator built with **Object-Oriented JavaScript** and **Tailwind CSS**. Create your own focus or relaxation environments by mixing multiple nature and urban sounds, adjusting individual volumes, and saving custom "atmospheres" to your browser.

## ✨ Features

- **Multilayered Mixing:** Play and blend multiple high-quality audio tracks (Rain, Birds, Cafe, etc.) simultaneously.
- **Individual Volume Control:** Dedicated sliders for every sound with real-time visual feedback.
- **Master Control:** A global Play/Pause and Master Volume slider to manage the entire mix instantly.
- **Custom Presets:** Save your favorite sound combinations to `localStorage` and reload them anytime.
- **Sleep Timer:** Integrated countdown timer (5, 15, 30, 60 min) to automatically stop audio and help you drift off.
- **Responsive UI:** A modern, glassmorphism design built with Tailwind CSS, optimized for mobile and desktop.

## 🚀 Tech Stack

- **HTML5 & CSS3:** Semantic structure and custom animations.
- **Tailwind CSS:** Utility-first styling with backdrop-blur and gradient effects.
- **Vanilla JavaScript (ES6+):** Organized using a clean Class-based architecture:
  - `AmbientMixer` (app.js): The main controller and event orchestrator.
  - `SoundManager`: Handles audio loading, play/pause states, and volume logic.
  - `UI`: Manages DOM rendering, icon toggling, and progress bar updates.
  - `Timer`: Handles the countdown logic and automatic audio cutoff.
  - `PresetManager`: Handles data persistence using `localStorage`.

## 🛠️ How to Run Locally

### Prerequisites

Because this project uses **ES6 Modules** (`import`/`export`), you must run it through a local web server to avoid browser security (CORS) errors.

### Launching the App

1.  **Clone the repository:**

    ```bash
    git clone [https://github.com/your-username/ambient-mixer.git](https://github.com/muntalysir/ambient-sound-mixer)
    cd ambient-mixer
    ```

2.  **Launch a Local Server:**
    - **VS Code:** Install the **Live Server** extension. Right-click `index.html` and select **"Open with Live Server"**.

## 📂 Project Structure

```text
├── index.html          # Main application structure
├── css/
│   └── styles.css      # Custom styles, animations, and Tailwind overrides
├── src/
│   ├── app.js          # Entry point & AmbientMixer initialization
│   ├── soundManager.js # Logic for audio elements and playback
│   ├── ui.js           # Logic for DOM updates and rendering
│   ├── timer.js        # Sleep timer and countdown logic
│   ├── presetManager.js # LocalStorage saving/loading functionality
│   └── soundData.js    # Configuration for sounds, icons, and colors
├── audio/              # .mp3 sound files
└── README.md           # Project documentation
```
