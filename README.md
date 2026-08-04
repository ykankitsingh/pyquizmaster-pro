<div align="center">

# 🧠 PyQuizMaster Pro

<img src="https://readme-typing-svg.demolab.com?font=Poppins&weight=600&size=26&duration=3000&pause=1000&color=4CAF50&center=true&vCenter=true&width=750&lines=Lightweight+Browser-Based+Quiz+Engine;Zero+External+Dependencies+%26+Native+APIs;Real-Time+Scoring+%26+Local+Persistence" alt="PyQuizMaster Pro Typing SVG" />

### 🚀 *A lightweight, interactive browser-based quiz application built with zero external dependencies, native Web Audio, and canvas particles*

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License](https://img.shields.io/badge/License-MIT-4CAF50?style=for-the-badge&logo=opensourceinitiative&logoColor=white)](LICENSE)

---

**Test your knowledge with real-time scoring, custom configurations, and native audio feedback! 🎯**

[📖 About](#-about-the-project) • [✨ Features](#-features) • [🏗️ Architecture](#-system-architecture) • [🛠️ Tech Stack](#️-technology-stack) • [🚀 Quick Start](#-getting-started)

</div>

---

## 📖 About the Project

**PyQuizMaster Pro** is a robust, self-contained educational web application designed to deliver an engaging quiz experience right inside any modern browser. 

By leveraging native web technologies like the **Web Audio API** for sound effects and **HTML5 Canvas** for particle/confetti visual feedback, it operates with absolute zero external dependencies, libraries, or build pipelines.

> [!NOTE]  
> **🎯 Mission:** To build high-performance, zero-overhead interactive web apps that require zero installation and run instantly anywhere.

---

## ✨ Features

<div align="center">

| Feature | Description |
|---------|-------------|
| 🟢 **Zero Externalities** | 100% self-contained code using native Web APIs (Web Audio & Canvas) |
| ⚡ **Interactive Gameplay** | Instant feedback, custom countdown timers, and responsive layout |
| 🎛️ **Custom Configuration** | Filter questions by topic and adjust quiz length dynamically |
| 💾 **Local Persistence** | Tracks your top scores directly in the browser via `localStorage` |
| 🎵 **Web Audio Feedback** | Procedurally generated sound effects for correct and incorrect answers |
| 🎉 **Canvas Visuals** | Native particle and confetti systems triggered upon completion |

</div>

---

## 🏗️ System Architecture

```mermaid
flowchart TB
    subgraph ClientLayer["🌐 User Browser Layer"]
        Browser["Modern Web Browser<br/>(Chrome / Firefox / Safari / Edge)"]
        HTML["index.html<br/>(Semantic Layout & Containers)"]
    end

    subgraph StylingLayer["🎨 Styling Engine"]
        CSS["Styles & Tokens<br/>(Responsive Flexbox / Grid & Modern Themes)"]
    end

    subgraph EngineLayer["⚡ Application Logic Layer"]
        App["JavaScript Engine<br/>(Quiz State Machine, Timer & Event Controller)"]
        Audio["Web Audio API<br/>(Native Sound Generator)"]
        Canvas["HTML5 Canvas<br/>(Particle & Confetti System)"]
    end

    subgraph StorageLayer["💾 Persistence Layer"]
        Storage[("Browser LocalStorage<br/>(High Scores & User History)")]
    end

    Browser --> HTML
    HTML --> CSS
    HTML --> App
    App --> Audio
    App --> Canvas
    App --> Storage

    style ClientLayer fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px
    style StylingLayer fill:#f9fbe7,stroke:#9e9d24,stroke-width:2px
    style EngineLayer fill:#e0f2f1,stroke:#00695c,stroke-width:2px
    style StorageLayer fill:#f1f8e9,stroke:#558b2f,stroke-width:2px
