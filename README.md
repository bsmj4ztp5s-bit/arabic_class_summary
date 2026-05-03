# Arabic Class AI Scribe 🎓

An AI-powered web app that converts your Zoom class transcripts into structured study materials — slides, vocabulary cards, grammar notes, flashcards, and a downloadable PDF.

## Live Demo
🌐 [your-username.github.io/arabic-scribe](https://your-username.github.io/arabic-scribe)

## Features
- 📋 Paste Zoom .vtt transcript (even phonetic English works)
- 📊 Auto-generates 5 structured lesson slides
- 📖 Extracts vocabulary with Arabic script + transliteration
- 📐 Identifies grammar rules
- 💬 Key phrases with Arabic script
- 🃏 Interactive flip flashcards
- 🌙 Cultural notes
- ⬇ Download full PDF study guide

## Tech Stack
```
Frontend:    HTML + CSS + Vanilla JavaScript
AI Brain:    Google Gemini 1.5 Flash API (free tier)
PDF Export:  jsPDF (CDN)
Hosting:     GitHub Pages (free)
```

## How It Works
```
User pastes Zoom transcript
        ↓
App cleans VTT timestamps
        ↓
Sends to Gemini API
        ↓
Gemini returns structured JSON
(slides, vocab, grammar, flashcards)
        ↓
JavaScript renders the UI
        ↓
User downloads PDF
```

## Setup & Deploy

### 1. Get a free Gemini API key
- Go to [aistudio.google.com](https://aistudio.google.com)
- Sign in with Google
- Click **Get API Key** → Create API Key
- Copy it (starts with `AIza...`)

### 2. Deploy to GitHub Pages
1. Fork this repository
2. Go to **Settings → Pages**
3. Set Source to **main branch / root**
4. Your app is live at `https://your-username.github.io/arabic-scribe`

### 3. Use the app
1. Open the live URL
2. Paste your Gemini API key
3. Paste your Zoom transcript
4. Hit **Generate** → explore slides, notes, flashcards
5. Click **Save PDF** to download your study guide

## Getting Your Zoom Transcript
1. In Zoom: **Settings → Recording → enable "Audio transcript"**
2. Record your class as normal
3. After class, find the `.vtt` file in your Zoom recordings folder
4. Open it in any text editor → copy all → paste into the app

## Project Structure
```
arabic-scribe/
├── index.html      ← entire app (single file)
└── README.md       ← this file
```

## Cost
- **Google Gemini API**: Free tier = 15 req/min, 1M tokens/day
- **GitHub Pages**: Free forever
- **Total cost**: $0

## Screenshots
*Add screenshots here after deployment*

## Author
Built as a learning project to automate Arabic class note-taking.

## License
MIT
