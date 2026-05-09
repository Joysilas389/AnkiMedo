# 🧠 AnkiMedo — Ace Your Boards

A personal, AI-powered medical flashcard PWA for USMLE Step 1, Step 2CK, Step 3, and MCCQE1 (Toronto Notes).

## Features
- 📄 Upload any medical PDF → Claude AI generates deep, mechanistic flashcards
- 🧠 Every card explains the **WHY** — mechanism, pathophysiology, from first principles
- 🔍 Search by topic, system, keyword, mechanism
- 📊 Spaced repetition (SM-2 algorithm) — Forgot / Hard / Good / Easy ratings
- 🎯 Filter by difficulty (easy / medium / hard), exam, body system
- 📈 Statistics — track mastery by topic
- 📱 PWA — installable on phone and desktop, works offline
- 🔐 Your API key stays in your browser only

## Setup

### Option 1: Open Locally
Just open `index.html` in any modern browser. No server needed.

### Option 2: Deploy (Recommended for PWA install)
Upload the entire folder to any static host:
- **Netlify** — drag the folder to [netlify.com/drop](https://netlify.com/drop)
- **Vercel** — `vercel deploy`
- **GitHub Pages** — push to a repo, enable Pages

### Get Your Claude API Key
1. Go to [console.anthropic.com](https://console.anthropic.com)
2. Create an API key
3. Paste it in Settings inside the app

## How to Use
1. Open Settings → paste your Claude API key → Save
2. Go to Home → upload your PDF (First Aid, Toronto Notes, lecture slides, etc.)
3. Select your target exam (Step 1, Step 2CK, Step 3, MCCQE1)
4. Wait ~30-60 seconds — Claude reads and generates cards
5. Study in Browse Cards or Due Today
6. Rate each card: Forgot / Hard / Good / Easy → spaced repetition schedules next review

## Study Tips
- **Detail Level = Deep Mechanistic** for maximum understanding
- **Focus Areas** in Settings to target weak areas (e.g. "enzyme deficiencies, HF pathophysiology")
- Use keyboard shortcuts during study: Space = flip, 1-4 = rate, Esc = exit
- Review Due Today daily for best retention

## Keyboard Shortcuts (Study Mode)
| Key | Action |
|-----|--------|
| Space / Enter | Flip card |
| 1 | Forgot |
| 2 | Hard |
| 3 | Good |
| 4 | Easy |
| Esc | Exit session |

## Tech Stack
- Vanilla HTML/CSS/JS — no framework
- Bootstrap 5.3 + Bootstrap Icons
- Claude API (claude-sonnet-4) for card generation
- PDF.js for PDF text extraction
- SM-2 spaced repetition algorithm
- localStorage for all data
- Service Worker for offline support
