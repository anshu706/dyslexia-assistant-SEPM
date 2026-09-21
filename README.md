<div align="center">

<img src="https://img.shields.io/badge/Version-1.0.0-6366F1?style=flat-square" alt="Version" />
<img src="https://img.shields.io/badge/PWA-Enabled-10B981?style=flat-square&logo=googlechrome&logoColor=white" alt="PWA" />
<img src="https://img.shields.io/badge/Accessibility-WCAG%202.1%20AAA-4F46E5?style=flat-square" alt="WCAG AAA" />
<img src="https://img.shields.io/badge/License-MIT-F59E0B?style=flat-square" alt="License" />
<img src="https://img.shields.io/badge/JavaScript-Vanilla%20ES6-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="Vanilla JS" />

<br /><br />

# 📖 Dyslexia Assistant

**A premium, distraction-free reading environment built specifically for dyslexic students and professionals.**

Upload any document, listen to it read aloud, apply accessibility overlays, and take annotated notes — all from a beautiful offline-capable web app.

<br />

[Features](#-features) · [Getting Started](#-getting-started) · [Usage Guide](#-usage-guide) · [Accessibility](#-accessibility) · [Tech Stack](#-tech-stack) · [Roadmap](#-roadmap)

</div>

---

## ✨ Features

| Category | Feature | Description |
|---|---|---|
| 📤 **Upload** | Multi-format Documents | Upload PDF, DOCX, or TXT — text is extracted client-side with no server needed |
| 📤 **Upload** | Paste Text | Directly paste or type text into the reader |
| 🎵 **Audio** | Text-to-Speech | Natural voice playback via Web Speech API with real-time word highlighting |
| 🎵 **Audio** | Voice Controls | Adjust speed (0.5×–2×), pitch, and select from all available system voices |
| 🎵 **Audio** | Indian English Voice | Automatic preference for `en-IN` voices when available |
| 👁️ **Reading** | Bionic Reading Mode | Bold word-prefix anchors for faster, guided eye movement |
| 📏 **Reading** | Focus Ruler | A position-tracking horizontal ruler overlay to guide line-by-line reading |
| 🎨 **Accessibility** | Irlen Colour Tints | Five overlay tints — Sepia, Soft Yellow, Mint, Soft Blue, Rose — to reduce visual stress |
| 🅰️ **Accessibility** | Dyslexia Fonts | Switch between OpenDyslexic, Atkinson Hyperlegible, or system font |
| 🅰️ **Accessibility** | Reading Typography | Fine-tune font size, line height, and letter spacing |
| 🔍 **Tools** | In-document Search | Instant keyword highlighting within the loaded document |
| 📖 **Tools** | Word Dictionary | Double-click any word for definitions, phonetics, examples, synonyms, and audio pronunciation |
| 🖍️ **Tools** | Colour Highlights | Select and highlight text in 5 colours; highlights persist per document |
| 📝 **Tools** | Notes | Create, edit, and delete notes for any document via a polished modal interface |
| ⭐ **Tools** | Bookmarks | Save named bookmarks per document |
| 📥 **Export** | Markdown Export | Download notes and highlights as `.md` files |
| 📊 **Stats** | Reading Analytics | Track sessions, words read, time spent, and reading streak |
| 👤 **Auth** | Local Auth | Register, login, update profile, and change password — all stored locally |
| 🌙 **UI** | Dark / Light / Auto Theme | System-aware theming with manual override |
| 📱 **UI** | Fully Responsive | Glassmorphism design optimised for mobile, tablet, and desktop |
| ⚡ **PWA** | Offline Support | Service Worker caches all assets for full offline usage |

---

## 🚀 Getting Started

### Prerequisites

- Any modern browser: **Chrome 90+**, **Edge 90+**, **Firefox 90+**, or **Safari 15+**
- No build step, no npm install, no backend — it is pure HTML/CSS/JS

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/YOUR-USERNAME/dyslexia-assistant.git
cd dyslexia-assistant

# 2. Open directly in your browser
start index.html           # Windows
open index.html            # macOS
xdg-open index.html        # Linux

# — or — serve with any static server
npx http-server -p 8080 .
python -m http.server 8080
```

### Install as a PWA (optional)

1. Open the app in Chrome or Edge
2. Click the **install icon** in the address bar (or the browser menu)
3. The app installs to your desktop / home screen and works fully offline

---

## 📚 Usage Guide

### 1. Sign In / Guest Mode

On first load you will see the authentication overlay. You can:
- **Create an account** (stored in your browser's localStorage)
- **Sign in** to restore your profile and settings
- **Continue as guest** to use all features without an account

### 2. Upload a Document

From the **Home** tab:
- Click the upload area or drag-and-drop a **PDF**, **DOCX**, or **TXT** file (max 10 MB)
- Or click **✏️ Paste Text Instead** to type / paste content directly

### 3. Read with Text-to-Speech

In the **Reader** tab:
- Press ▶ to play, ⏸ to pause, and ⏹ to stop
- Adjust **Speed**, **Pitch**, and **Voice** from the toolbar
- The currently spoken word is highlighted in the text in real time

### 4. Accessibility Overlays

| Control | How to use |
|---|---|
| **Bionic Reading** | Click the 👁️ button in the toolbar |
| **Focus Ruler** | Click the 📏 button; the ruler follows your mouse |
| **Colour Tint** | Click any coloured dot in the toolbar row |
| **Font / Spacing** | Go to the ⚙️ Settings tab |

### 5. Annotate

| Tool | How to use |
|---|---|
| **Highlight** | Select text → click 🖊 Highlight in the pop-up |
| **Dictionary** | Double-click any single word |
| **Note** | Click 📝 → fill in the modal → Save Note |
| **Bookmark** | Click ⭐ → name it → Save Bookmark |

### 6. Export

Open the sidebar (🖍 button) → **Highlights** or **Notes** panel → click the export button to download a formatted Markdown file.

### 7. Statistics

Navigate to the **📊 Statistics** tab to see your total sessions, words read, time spent, and current reading streak.

---

## ♿ Accessibility

This project targets **WCAG 2.1 Level AAA** and is built around the needs of dyslexic readers:

| Consideration | Implementation |
|---|---|
| **Dyslexia fonts** | OpenDyslexic (bottom-weighted letterforms) and Atkinson Hyperlegible (high character distinction) |
| **Irlen Syndrome** | Five colour overlay tints — scientifically chosen to reduce contrast-sensitivity issues |
| **Bionic Reading** | Bold prefixes anchor eye movement and reduce letter-tracking errors |
| **Focus Ruler** | Horizontal ruler eliminates line-skip errors during reading |
| **Typography control** | User-adjustable font size (px), line height (1–3), and letter spacing (em) |
| **High Contrast Mode** | One-click high contrast toggle |
| **Screen reader** | Semantic HTML5, ARIA roles, labels, and `aria-live` regions for notifications |
| **Keyboard navigation** | Full tab-order support; Enter key submits modals |
| **TTS** | Real-time word highlighting synchronised with speech playback |

---

## 🧩 Tech Stack

| Layer | Technology |
|---|---|
| **Structure** | HTML5 (semantic elements, ARIA) |
| **Styling** | Vanilla CSS3 — custom properties, glassmorphism, `@font-face`, media queries |
| **Logic** | Vanilla JavaScript (ES6 classes, async/await, Web APIs) |
| **TTS** | [Web Speech API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API) |
| **PDF parsing** | [PDF.js 3.11](https://mozilla.github.io/pdf.js/) — Mozilla's client-side PDF renderer |
| **DOCX parsing** | [JSZip 3.10](https://stuk.github.io/jszip/) — ZIP extraction + XML parsing |
| **Dictionary** | [Free Dictionary API](https://dictionaryapi.dev/) — definitions, phonetics, audio |
| **Fonts** | Google Fonts (Plus Jakarta Sans, Inter, Sora) + OpenDyslexic CDN + Atkinson Hyperlegible |
| **Offline** | [Service Worker API](https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API) |
| **Storage** | `localStorage` — documents, settings, highlights, notes, bookmarks, stats, auth |
| **PWA** | `manifest.json` — installable, standalone display, themed |

---

## 📁 Project Structure

```
dyslexia-assistant/
├── index.html              # Single-page application shell (all views)
├── manifest.json           # PWA manifest
├── README.md               # This file
│
├── css/
│   ├── main.css            # Core design system, layout, components
│   ├── dyslexia.css        # Accessibility fonts, tints, bionic reading
│   ├── themes.css          # Dark / Light / Auto theme variables
│   ├── animations.css      # Keyframe animations and transitions
│   └── auth.css            # Authentication overlay styles
│
└── js/
    ├── app.js              # Main application class — bootstraps all features
    ├── auth.js             # AuthManager — local register/login/profile logic
    ├── authUI.js           # AuthUI — overlay, header state, profile page
    ├── file-handler.js     # FileHandler — PDF.js + JSZip document parsing
    ├── tts.js              # TextToSpeech — Web Speech API wrapper
    ├── dictionary.js       # DictionaryManager — Free Dictionary API + cache
    ├── highlights.js       # HighlightManager — colour highlighting + export
    ├── notes.js            # NotesManager — CRUD notes + export
    ├── storage.js          # StorageManager — localStorage CRUD + settings
    ├── state.js            # ReadingStats — session tracking + streak
    ├── utils.js            # Utils — bionic reading, debounce, helpers
    └── service-worker.js   # PWA Service Worker — offline caching
```

---

## 🗺️ Roadmap

| Status | Feature |
|---|---|
| ✅ Done | Advanced in-document search with keyword highlighting |
| ✅ Done | Free Dictionary API — definitions, phonetics, audio |
| ✅ Done | Notes & highlights Markdown export |
| ✅ Done | Local authentication with profile management |
| ✅ Done | PWA offline caching via Service Worker |
| ✅ Done | Styled modal dialogs for notes and bookmarks |
| 🔄 Planned | Multi-language TTS voice fallback |
| 🔄 Planned | Cloud sync (Firebase / Supabase) |
| 🔄 Planned | Reading speed test with WPM measurement |
| 🔄 Planned | AI-powered document summarisation |

---

## 🤝 Contributing

Contributions are welcome! To get started:

```bash
git clone https://github.com/YOUR-USERNAME/dyslexia-assistant.git
cd dyslexia-assistant

# Make your changes — no build step needed
# Test by opening index.html in your browser

# Submit a PR with a clear description of your change
```

Please keep accessibility at the centre of any UI changes and test with keyboard-only navigation before submitting.

---

## 📄 License

This project is licensed under the **MIT License**.

---

<div align="center">

Made with ❤️ for accessibility and inclusion

*Built to help dyslexic readers everywhere — because everyone deserves to read without limits.*

</div>
