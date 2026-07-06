# 🌊 AuraFlow3 - Procedural Water Sound Engine

**A real-time, toggleable water sound synthesizer built with the Web Audio API.  
Sculpt organic, bubbling streams and transform them into resonant, musical drones with a single click.**

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](#)
[![Web Audio API](https://img.shields.io/badge/Web%20Audio-API-blueviolet?style=flat)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

![Screenshot](screenshot.png) <!-- Replace with an actual screenshot of the interface -->

---

## 📖 Overview

**Procedural Water Sound Engine** is a standalone HTML/JavaScript web application that generates an endless, evolving water texture using brown noise, dynamic bubbles, and subtle modulation.  

In **Normal** mode you hear a believable stream – complete with surging lows and popping bubbles.  
Switch to **Resonant** mode, and the same chaotic water is routed through a bank of **high‑Q bandpass filters tuned to a C‑major chord**, transforming it into a shimmering, musical instrument.

All seven advanced audio techniques (noise‑based bubbles, sub‑bass, flow LFO, feedback delay, cascaded filters, pre‑saturation, and Q modulation) can be **individually toggled on/off in real time**, giving you complete control over the sound’s character.

Two live visualizers (oscilloscope + frequency spectrum) provide instant feedback, making the engine perfect for sound design, meditation aids, game prototyping, or simply exploring procedural audio.

---

## ✨ Features

### 💧 Realism Layer
| Feature | Description |
|--------|-------------|
| **Noise‑Based Bubbles** | Filtered noise bursts with ascending pitch envelope – mimics authentic bubble pops and gurgles, replacing sterile sine waves. |
| **Flow LFO Modulation** | A slow, random low‑frequency oscillator sweeps the water’s low‑pass cutoff, creating a natural, surging stream movement. |
| **Sub‑Bass Rumble** | A second brown noise layer, aggressively low‑passed at ~100 Hz, adds weight and underwater pressure. |

### 🔮 Resonance Layer (Resonant Mode)
| Feature | Description |
|--------|-------------|
| **Feedback Delay (C4‑tuned)** | A short delay line (period of C4, ~3.82 ms) with feedback creates shimmering, comb‑filtered overtones that reinforce the root pitch. |
| **Cascaded Bandpass Filters** | Two resonant bandpass filters per chord note provide a much steeper, vocal/formant‑like resonance peak compared to a single filter. |
| **Pre‑Filter Soft Saturation** | A tanh‑based waveshaper adds subtle harmonic excitement, giving the resonant filters more to “grab onto”. |
| **Q Modulation (Breathing)** | Independent LFOs slowly vary the resonance (Q) of each filter, making the chord feel organic and alive. |

### 🖥️ User Interface
- 🎛 **Toggle switches** for every feature – no page reloads, no restarts.  
- 📊 **Real‑time oscilloscope and frequency spectrum** with distinct color themes (blue for Normal, purple for Resonant).  
- 🟢 **Live status indicator** and clear play/stop controls.  
- 🧩 Responsive design – works on desktop and modern mobile browsers.

---

## 🗺️ Roadmap

✅ **Implemented**
- Realistic water generation (brown noise + dynamic bubbles)
- All seven toggleable audio processing modules
- Live visual feedback with canvas visualizers
- Seamless mode switching without audio glitches

🔮 **Planned (Next Releases)**
- **Additional chord presets** – minor, suspended, and user‑definable frequency sets
- **Reverb module** – simple convolution or algorithmic reverb for spacious ambiences
- **Parameter sliders** – fine‑tune filter Q, bubble density, LFO rates, and feedback amount
- **MIDI/OSC control** – trigger mode changes and toggle switches externally
- **Audio export** – record the output directly to a WAV file
- **Mobile performance optimizations** – reduce CPU load on lower‑end devices
- **Preset save/load** – store your favourite toggle combinations

---

## 🚀 Getting Started

### Running the Engine
1. **Clone or download** this repository.
2. Open the `index.html` file in a modern browser (Chrome, Firefox, Edge, Safari).
3. Click **🌊 Normal Water** or **✨ Resonant Water** to start the engine.
4. Toggle any feature – changes are applied instantly while the sound is playing.

No build tools, frameworks, or external dependencies required.

### Browser Support
- Any browser that supports the **Web Audio API** (all major browsers since ~2015).
- For the best experience, use the latest version of Chrome or Firefox.

---

## 🤝 Contributing

Contributions are welcome!  
If you have ideas for new features, improvements, or bug fixes, please open an issue first to discuss your proposal.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 🙏 Acknowledgments

- Inspired by procedural audio techniques and the incredible power of the Web Audio API.
- Built with vanilla JavaScript – no libraries, no compromises.

---

*Made with 💧 and 🎵 by [Your Name/Username]*
