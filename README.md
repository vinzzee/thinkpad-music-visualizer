Here is a sleek, professional `README.md` tailored specifically for your ThinkPad-inspired audio visualizer. It captures the minimalist, high-contrast aesthetic of the code and includes clear setup instructions.

---

# 🔴 ThinkPad Audio Visualizer

A sleek, lightweight, client-side web audio visualizer inspired by the iconic **IBM/Lenovo ThinkPad** aesthetic. Designed with a dark high-contrast theme, glassmorphism UI elements, and glowing TrackPoint-red accents (`#E60012`), this application renders real-time audio spectrum visualizations and interactive floating geometry directly in your browser.

---

## ⚡ Features

* **Multiple Audio Sources:**
* **System Audio Capture:** Visualizes live loopback audio directly from your system or browser tabs via `getDisplayMedia`.
* **Microphone Input:** Live audio visualization via your device's mic input.
* **Local File Upload:** Upload and visualize local audio files (`.mp3`, `.wav`, `.flac`, etc.) with continuous playback loop.


* **Minimalist Canvas Visualizer:**
* **Radial Spectrum Core:** 64-bar circular frequency spectrum anchored at the screen center with highlighted TrackPoint red index markers.
* **Reactive Floating Geometry:** Dynamic floating artifacts (wireframe squares, crosshairs, concentric rings, and glowing red TrackPoint nodes) that pulse, scale, and rotate based on specific frequency bands.


* **Customizable Settings UI:**
* Floating **Glassmorphism Panel** with real-time parameter tuning.
* Adjust **Response Time (Smoothing)** via `analyser.smoothingTimeConstant`.
* Scale **Reaction Intensity** dynamically.


* **Zero Dependencies:** Built entirely with raw HTML5, CSS3 (Flexbox/Grid/Backdrop Filters), and pure Vanilla JavaScript using the **Web Audio API** and **HTML5 Canvas**. No frameworks, no external dependencies.

---

## 🚀 Quick Start

Since this is a standalone HTML application, no build process or package installation is required.

### 1. Run Locally

1. Clone or download this repository:
```bash
git clone https://github.com/your-username/thinkpad-audio-visualizer.git

```


2. Open `index.html` (or `thinkpad-music-visualizerg.html`) directly in any modern web browser (Chrome, Edge, Brave, Firefox, or Safari).

### 2. Using System Audio (Loopback)

1. Open the UI controls by clicking the **gear icon** in the bottom-left corner.
2. Click **System Audio (Loopback)**.
3. In the browser popup, select the tab, window, or entire screen you want to capture, and **make sure to check the "Share Audio" checkbox**.

---

## 🛠️ Built With

* **HTML5 Canvas** - High-performance 2D dynamic rendering.
* **Web Audio API** - `AudioContext`, `AnalyserNode`, and real-time Fast Fourier Transform (FFT) frequency data extraction.
* **CSS Glassmorphism** - modern UI layer built using `backdrop-filter: blur()`.

---

## ⚙️ Configuration & Controls

| Control | Description | Range / Options |
| --- | --- | --- |
| **Response Time** | Adjusts audio smoothing; higher values create smoother movements, lower values react instantly to spikes. | `0.10` – `0.95` |
| **Reaction Intensity** | Multiplier for bar heights and geometric artifact scaling/speed. | `0.5x` – `4.0x` |
| **System Audio** | Captures desktop/browser sound output. | Native Browser Stream |
| **Microphone** | Captures audio from default input device. | `getUserMedia` Stream |
| **Upload File** | Load an audio file for local playback. | Any browser-supported audio format |

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.
