# FAHEEM AI Studio 🎬✨
> **AI Video Reverse-Engineering & Structured Prompt DNA Extraction**

FAHEEM AI Studio is a professional, dark-mode SaaS application engineered with a **"Liquid Glass" Glassmorphism** design language. It reverse-engineers chronological video frames to reconstruct deep, cinematic generation prompts and structured visual DNA vectors.

---

## 💎 Design System & Aesthetic (Liquid Glass)
- **Liquid Glass Skeuomorphism**: Multi-layered inner reflections, top specular light highlights, and iridescent edge refractions inspired by modern translucent 3D UI concepts.
- **Pill Geometry**: Pill-shaped action buttons, floating capsules, and smooth input controls (`border-radius: 9999px`).
- **Dynamic Lighting**: Ambient mesh orbs with floating cosmic gradients over a deep obsidian canvas (`#06080e`).
- **Tactile Feedback**: Specular gleam sweeps, micro-depressions on click, and responsive status tags.

---

## ⚡ Core Pipeline & Architecture

```
                               ┌──────────────────────────────────────────────────────────┐
                               │                    CLIENT BROWSER                        │
┌──────────────┐   Upload/Drop │ 1. Ingest Video File (MP4, WebM, MOV)                    │
│ Video Source │──────────────>│ 2. Extract Duration, Dimensions, Aspect Ratio, FPS       │
└──────────────┘               │ 3. Extract 8-16 Evenly Distributed Frames (HTML5 Canvas) │
                               └────────────────────────────┬─────────────────────────────┘
                                                            │ Frames + Metadata Payload
                                                            ▼
                               ┌──────────────────────────────────────────────────────────┐
                               │                     NODE.JS SERVER                       │
                               │  /server/ai/providers/ Architecture                      │
                               │  ├─ BaseAIProvider (Contract & Schema Validation)       │
                               │  ├─ GeminiProvider (@google/genai & REST Fallback)       │
                               │  └─ ProviderManager (Registry & Runtime Config)          │
                               └────────────────────────────┬─────────────────────────────┘
                                                            │
                                                            ▼
                               ┌──────────────────────────────────────────────────────────┐
                               │              OUTPUT & PRESENTATION LAYER                 │
                               │  1. ⚖️ Forensic Disclaimer (Observable Reconstructions)  │
                               │  2. 📜 Reconstructed Master Prompt (Sora/Runway/MJ/Kling)│
                               │  3. 🧬 8 Structured DNA Vectors with Individual Copy     │
                               │  4. ⏱️ Chronological Scene-by-Scene Timeline             │
                               │  5. 💾 Download Full DNA Dossier (.txt)                  │
                               └──────────────────────────────────────────────────────────┘
```

---

## 🛡️ Security & Privacy Principles
- **Zero Client-Side Exposure**: API keys reside exclusively in server-side environment variables (`.env`) or secure in-memory server session. Keys are never transmitted to the browser.
- **Client-Side Media Efficiency**: Video decoding and frame capture occur completely inside the client's browser using HTML5 Canvas. The full video file is never transmitted to third parties; only selected compressed analytical frames are processed.
- **Objective Observables Only**: Adheres to the strict rule of never claiming to recover hidden author prompts. Master prompts are explicitly designated as *Reconstructed Master Prompts*.
- **No Faked Responses**: When `GEMINI_API_KEY` is not present, the system cleanly operates in Local Processing Mode and presents the informative notification: `"AI analysis is not configured yet."`

---

## 🚀 Getting Started

### 1. Installation
```bash
git clone <repo-url>
cd Antigravity
npm install
```

### 2. Configure Environment
Copy `.env.example` to `.env`:
```bash
cp .env.example .env
```

Edit `.env` to configure your Gemini API Key:
```env
PORT=3000
GEMINI_API_KEY=AIzaSy...
GEMINI_MODEL=gemini-2.5-flash
```
*(Leave `GEMINI_API_KEY` empty to test Local Processing mode and the AI fallback banner).*

### 3. Launch Server
```bash
npm start
```
Open **[http://localhost:3000](http://localhost:3000)** in your browser.

---

## 🧩 Key Features & Controls
- **In-Browser Demo Video Synthesizer**: Click **Demo Clip** in the top bar to procedurally generate a 4-second cyberpunk sci-fi video directly in the browser via Canvas & MediaRecorder.
- **Density Control**: Extract 8, 12, or 16 frames evenly distributed across the video timeline.
- **Frame Lightbox**: Click any frame in the Frame Gallery to zoom in and inspect fine details and timestamps.
- **One-Click Section Copying**: Individual copy buttons for all 8 DNA vectors with animated checkmark feedback.
- **Format Formatter**: Toggle target prompt syntax for **Runway Gen-3**, **Midjourney v6.1**, **Sora**, **Kling AI**, or **Luma Dream Machine**.
- **Download Master Prompt (.txt)**: Export a clean analysis dossier with metadata, master prompt, observable DNA, and scene chronology.
- **New Analysis Reset**: Reset the entire workspace instantaneously without a full page reload.

---

## 📜 Structured DNA Schema
| Vector | Description |
|---|---|
| **Characters & Subjects** | Physical attributes, expressions, attire, and postures |
| **Environment & Setting** | Architectural context, depth planes, weather, and world atmosphere |
| **Key Objects & Props** | Hero objects, surface materials, interactions, and placements |
| **Actions & Kinematics** | Physical motions, speed vectors, trajectories, and pacing |
| **Camera & Optics** | Shot scale, focal length, depth of field, angles, and camera tracking moves |
| **Lighting & Radiance** | Key/fill ratios, color temperature, volumetric rays, and shadow hardness |
| **Visual Style & Medium** | Medium, art direction, texture/grain, and hex color grading swatches |
| **Audio & Acoustics** | Strictly observable sonic markers (silent if visual-only) |
| **Chronological Timeline** | Scene cuts, duration bounds, camera choreography, and visual cues |
| **Master Prompt** | Comprehensive generation prompt formatted for modern video models |
