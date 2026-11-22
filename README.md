<div align="center">

# 🕶️ EDWIN

**Real-Time Autonomous Vision & Agentic Swarm OSINT Platform**  
*The father of JARVIS: From live optical feed to comprehensive intelligence dossiers in seconds.*

[![License: MIT](https://img.shields.io/badge/License-MIT-emerald.svg)](LICENSE)
[![Python: 3.11+](https://img.shields.io/badge/Python-3.11+-3776AB.svg?logo=python&logoColor=white)](https://python.org)
[![Next.js: 16](https://img.shields.io/badge/Next.js-16-black.svg?logo=next.js&logoColor=white)](https://nextjs.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.116+-009688.svg?logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![TypeScript](https://img.shields.io/badge/TypeScript-5+-3178C6.svg?logo=typescript&logoColor=white)](https://www.typescriptlang.org)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-CSS-38B2AC.svg?logo=tailwind-css&logoColor=white)](https://tailwindcss.com)

[Architecture](#-architecture) • [Supported Glasses](#-supported-smart-glasses--hardware) • [Features](#-core-capabilities) • [Quick Start](#-quick-start) • [Environment](#-configuration) • [Disclaimer](#-ethical--legal-disclaimer)

</div>

---

## ⚡ Overview

**EDWIN** transforms smart eyewear—including **Ray-Ban Meta** and **Oakley Meta** smart glasses—or live video streams into an autonomous reconnaissance engine. When a subject appears in your field of view, EDWIN extracts facial biometrics, dispatches a parallel swarm of browser agents to research their background across the open web, and projects an interactive, military-grade corkboard dossier in real time.

```
[ Meta Ray-Ban / Oakley Meta / Video Stream ] ──► [ MediaPipe + ArcFace Biometrics ]
                                                                 │
                                                                 ▼
                                                     [ Reverse Visual Search ]
                                                                 │
                  ┌──────────────────────────────┴──────────────────────────────┐
                  ▼                                                             ▼
      [ Exa Fast Enrichment ]                                      [ Browser-Use Agent Swarm ]
   (News, Articles, Profiles)                                     (LinkedIn, X, GitHub, Web)
                  │                                                             │
                  └──────────────────────────────┬──────────────────────────────┘
                                                 ▼
                                   [ Claude / Gemini Synthesis ]
                                                 │
                                                 ▼
                                [ Reactive Tactical Corkboard HUD ]
```

---

## 👓 Supported Smart Glasses & Hardware

EDWIN is engineered for seamless wearable optical capture across the Meta / EssilorLuxottica smart glasses ecosystem:

* 🕶️ **Ray-Ban Meta Smart Glasses** *(Wayfarer, Headliner, Skyler)*: Native streaming integration for real-time video frames and audio transcription.
* 🏃 **Oakley Meta Smart Glasses**: Performance sports optics compatibility for dynamic, on-the-move field intelligence gathering.
* 📱 **Mobile & RTSP Streams**: Connect any phone camera or wearable rig via WebRTC/RTSP or Telegram photo intake bot.
* 💻 **Webcam & Local Video**: Run local simulations using any standard USB webcam or pre-recorded evaluation footage.

---

## 🚀 Core Capabilities

* **Hardware & Stream Ingestion:** Ingests live RTSP/WebRTC streams from Ray-Ban Meta and Oakley Meta smart glasses, mobile cameras, or Telegram intake bots.
* **Neural Face Embeddings:** High-speed face detection via MediaPipe coupled with ArcFace-style feature embeddings and reverse-image correlation.
* **Autonomous Swarm Reconnaissance:** Spawns headless Browser-Use sessions across LinkedIn, X (Twitter), Google, and public registries simultaneously.
* **Dual-Tier Intelligence Synthesis:** Synthesizes structured dossiers using Claude 3.5 Sonnet with automated fallback to Gemini 2.0 Flash.
* **Tactical Corkboard UI:** A high-framerate Next.js interface with physics-based pushpin nodes, dynamic red-string connection graphs, and live agent feeds.
* **Graceful Degradation:** Runs locally even if specific cloud APIs are unconfigured.

---

## 🛠️ Tech Stack

| Component | Technology |
| :--- | :--- |
| **Frontend** | Next.js 16 (App Router), Framer Motion, Tailwind CSS, Lucide Icons |
| **Backend** | FastAPI (Python 3.11+), Pydantic v2, Uvicorn |
| **Real-Time Data** | Convex (reactive sync) + In-memory local fallback |
| **Computer Vision** | MediaPipe, OpenCV, ArcFace (insightface) |
| **Agent Swarm** | Browser Use Cloud / Chromium Automation |
| **Fast Search** | Exa API |
| **LLM Synthesis** | Anthropic Claude 3.5 Sonnet & Google Gemini Flash |

---

## 🏁 Quick Start

### Prerequisites
* **Python 3.11+**
* **Node.js 20+**
* `uv` or `pip`

### 1. Clone & Setup
```bash
git clone https://github.com/ATLURI0001/EDWIN.git
cd EDWIN
cp .env.example .env
```

### 2. Launch Backend
```bash
cd backend
python -m venv .venv
# Windows:
.venv\Scripts\Activate.ps1
# Linux/macOS:
# source .venv/bin/activate

pip install -e .
uvicorn main:app --reload --port 8000
```
Verify health: `http://localhost:8000/api/health`

### 3. Launch Frontend
```bash
cd ../frontend
npm install
npm run dev
```
Open **[http://localhost:3000](http://localhost:3000)** in your browser.

---

## 🔐 Configuration

Populate your `.env` file with the keys you wish to enable (missing keys degrade gracefully):

| Key | Description |
| :--- | :--- |
| `ANTHROPIC_API_KEY` | Primary dossier synthesis model (Claude) |
| `GEMINI_API_KEY` | Secondary synthesis fallback & audio transcription |
| `BROWSER_USE_API_KEY` | Cloud agent swarm orchestration |
| `EXA_API_KEY` | Fast OSINT entity resolution |
| `NEXT_PUBLIC_CONVEX_URL` | Multi-tab real-time state synchronization |
| `TELEGRAM_BOT_TOKEN` | Remote photo intake via Telegram |

---

## ⚖️ Ethical & Legal Disclaimer

EDWIN is intended **strictly for academic research, privacy auditing, and authorized demonstrations**. Users are solely responsible for compliance with local wiretapping, consent, and biometric privacy laws (e.g., GDPR, CCPA, BIPA). Never record or profile individuals without explicit authorization.

---

## 📄 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for details.