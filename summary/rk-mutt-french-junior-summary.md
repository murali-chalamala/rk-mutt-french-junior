# 🇫🇷 RK Mutt French Junior — Project Summary

**Developed by:** Murali Krishna Chalamala (RK Mutt Student)
**Inspired by:** Anuradha Madam · French Teacher · RK Mutt, Hyderabad
**Purpose:** My own idea & personal initiative — to help fellow French learners study effectively
**Licence:** For Educational Purpose Only · Not for commercial use

---

## 📁 Files

| File | Size | URL |
|---|---|---|
| `french-vocab.html` (Main App) | 505 KB | https://murali-chalamala.github.io/rk-mutt-french-junior/ |
| `index_workbook.html` (Festival Workbook) | 83 KB | https://murali-chalamala.github.io/rk-mutt-french-workbook/ |

---

## 🏫 Main App — `french-vocab.html`

### Overview
Single-file HTML app — all CSS and JS inline. No framework, no build step.
Only external dependency: Google Fonts.

### Navigation
Grouped dropdown nav with 3 week groups + Special section:

- **Week 1** — Days 1–5
- **Week 2** — Days 6–10
- **Week 3** — Days 11–17
- **Special** — 📓 Workbook · 📄 PDF Books · 👨‍🎓 About · 📊 Progress · 🔁 Review All · 🔬 Pro Lab

---

### 📅 Day-by-Day Content

| Day | Topic | Key Sections |
|---|---|---|
| Day 1 | Greetings & Courtesy | Flashcards · Quiz · Reverse · Speed · Spelling · Fill · Match · Slideshow |
| Day 2 | Alphabet & Pronunciation | IPA · Accents · Vowel combos · Special sounds · Rule Quiz |
| Day 3 | Pronouns & -ER Verbs | Subject/Object pronouns · Parler · Habiter · S'appeler · Fill · Quiz |
| Day 4 | Verb Groups (ER/IR/RE/Être) | Tables · Fill · Quiz · Homework (Fermer/Rester/Réussir/Agir) |
| Day 5 | Numbers 0–100 & Time | Number table · Flashcards · Days/Months · Calendar · Quiz |
| Day 6 | Reflexive Verbs | Se laver · S'habiller · RE verbs · Tables · Fill · Quiz |
| Day 7 | Être & Nationalities | Être table · Nationalities · C'est/Ce sont · Classroom phrases · Fill · Quiz |
| Day 8 | Se présenter | Intro card · Vocab table · Quiz |
| Day 9 | Prendre & Comprendre | Verb tables · Fill · Quiz |
| Day 10 | Apprendre | Verb table · Grammar notes · Fill · Quiz |
| Day 11 | Aller & Venir + Conversation | Verb tables · Les voisins de Sophie · Fill · Quiz |
| Day 12 | Articles & Adjective Agreement | Grammar · Ordinals · Paris civilisation · Fill · Quiz |
| Day 13 | Lire · Écrire · CER/GER/È rules · Colours | Verb tables · Colours · Homework (Lancer/Avancer/Diriger/Encourager) · Quiz |
| Day 14 | Dire & Faire | Verb tables · Homework (Dire/Faire drills) · Quiz |
| Day 15 | Articles Contractés | À group & De group · Exercise A & B · Homework · Quiz |
| Day 16 | Aller & Venir · Tu ou Vous · Prépositions | Conjugation · Tu/Vous rules · À & De tables · Où/D'où · 3 Conversations · Vocabulary |
| Day 17 | Adjectifs interrogatifs · Leçon 6 | Quel/Quelle/Quels/Quelles · Exercice 4 (10 items) · Leçon 6 vocab · Registration conversation |

---

### 🎮 Features

#### Study Modes (Day 1)
- **Flashcards** — flip animation with IPA, pronunciation hint, audio
- **Quiz** — 4-option MCQ with score tracking
- **Reverse Quiz** — English → French
- **Speed Round** — timed challenge with countdown
- **Spelling** — type the French word
- **Fill Blank** — sentence completion
- **Match** — drag/tap matching game
- **Slideshow** — auto-play presentation mode

#### Grammar Practice (Days 3–17)
- **Fill-in-Blank** — conjugation drills (Days 7–12 generic, Days 13–15 homework tabs)
- **Verb tables** — 14 verbs: S'appeler · Être · Prendre · Comprendre · Apprendre · Aller · Venir · Lire · Écrire · Commencer · Manger · Acheter · Dire · Faire
- **Homework tabs** — Days 4, 13, 14, 15 with dedicated CER/GER/Dire/Faire drills

#### Pronunciation
- **IPA** on every Day 1 flashcard
- **Pronunciation hints** (English-friendly phonetics) — 97+ across the app
- **TTS audio** via Web Speech API — click any 🔊 to hear
- **Google Translate fallback** — for browsers without TTS
- **Pro Lab** — Type & Listen · Real Audio · Minimal Pairs · Nasal Vowels · Liaison
- **Conversation pronunciation** — every dialogue line has phonetic hint

#### Review & Progress
- **Review All** — 8 question types from all 17 days: vocab · conjugation · grammar · translation · number · phrase · pronunciation · article. Session sizes: 10 / 20 / 30 questions
- **Progress Tracker** — per-day completion %, quiz best scores, course completion bar, day grid badges
- **Leaderboard** — score history per mode, best scores saved to localStorage
- **Streak bar** — daily streak, stars, best quiz, course % , days done counter

#### Smart Extras
- 🌙 **Dark/Light mode** — persists on reload via `fr_theme` localStorage
- 🔤 **Bigger Text toggle** — accessibility font size
- ⌨️ **Keyboard shortcuts** — Arrow keys (next/prev card), Space (flip card)
- 📤 **Share button** — native share on mobile, clipboard copy on desktop
- 🎉 **Confetti + toast** — fires on 100% quiz score and first day completion
- 🖨️ **Print mode** — clean stylesheet, hides nav/footer
- 🏆 **Day completion badges** — shown in dropdown nav chips

#### Special Sections
- **📓 Workbook Practice** — 6 tabs: Vocabulary · Numbers · Verbs · Colours · Conversation match game · Articles Contractés
- **📄 PDF Books** — 5 books: Festival Main Book · Festival Workbook · Festival Transcript · Mon Passeport Units 01 & 03
- **👨‍🎓 About** — Developer info · App stats · Inspiration · Quick links
- **📊 Progress** — Full course tracker with per-day cards
- **🔁 Review All** — Cross-day revision with stats
- **🔬 Pro Lab** — Advanced pronunciation tools

---

### 🗄️ localStorage Keys

| Key | Stores |
|---|---|
| `fr_learned` | Learned word set |
| `fr_starred` | Starred words |
| `fr_streak` | Daily streak count |
| `fr_lastdate` | Last study date |
| `fr_name` | Student name |
| `fr_best` | Best quiz score |
| `fr_scores` | Full score history (JSON) |
| `fr_review_sessions` | Review All session history |
| `fr_day_progress` | Per-day progress (JSON) |
| `fr_theme` | light / dark preference |

---

### 🏗️ Architecture

```
french-vocab.html (single file, 505 KB)
├── <style>          — all CSS (dark/light themes, mobile responsive)
├── <body>           — 25 content sections (day1–day17 + special)
│   ├── header       — streak bar, name bar, WOTD banner
│   ├── toolbar      — Bigger Text, Theme, Print, Scores, Festival WB, Share
│   ├── day-nav      — grouped dropdown (Week 1/2/3 + Special)
│   ├── day1–day17   — lesson content
│   ├── workbook     — practice sections
│   ├── pdflib       — 5 PDF cards
│   ├── about        — developer info
│   ├── progress     — course tracker
│   ├── reviewAll    — cross-day quiz
│   ├── proLab       — pronunciation lab
│   └── global-footer— on every page
└── <script>         — all JS (quiz engine, progress, audio, nav)
```

---

## 📓 Festival Workbook — `index_workbook.html`

### Overview
Interactive workbook for Festival Leçons 0–4. Practice exercises with fill-blank, MCQ, ordering, matching, true/false, and verb tables. All with English pronunciation hints and meanings.

### Lessons

| Leçon | Topic |
|---|---|
| Leçon 0 | Numbers · Famous people · Alphabet |
| Leçon 1 | Greetings · Nationalities · Être |
| Leçon 2 | -ER verbs · Subject pronouns · Il/Elle |
| Leçon 3 | Colours · Likes/Dislikes · Aimer |
| Leçon 4 | Les voisins · Present tense · Sentence order |

### Features

- **Practice / Exam / Revision** — 3 modes with score tracking
- **Mistakes tracker** — review wrong answers
- **Answer Key** — complete answers per lesson
- **Vocabulary modal** — searchable word list with pronunciation
  - Shows complete French sentence (answer filled in green)
  - Pronunciation in brackets `(zhay)` next to answer
  - English meaning below
- **Answer lines** — every exercise type shows:
  - ✅ Correct answer
  - 🔊 Pronunciation hint badge
  - English meaning
- **Exercise types:**
  - Fill-in-blank (pronoun drills)
  - MCQ (4 options)
  - MCQ Choice (odd one out)
  - Match (drag pairs)
  - Order (sentence scramble)
  - True/False
  - Verb conjugation tables
- **Grammar Tip** button per exercise
- **Global score** bar + progress %
- **Print** support

### Languages
- 🇫🇷 French (original)
- 🇬🇧 English meaning + pronunciation hint
- *(Telugu fully removed)*

---

## 🚀 GitHub Deployment

### Main App
```
Repository:  github.com/murali-chalamala/rk-mutt-french-junior
Branch:      main
File:        index.html  (upload french-vocab.html as index.html)
Live URL:    https://murali-chalamala.github.io/rk-mutt-french-junior/
```

### Festival Workbook
```
Repository:  github.com/murali-chalamala/rk-mutt-french-workbook
Branch:      main
File:        index.html  (upload index_workbook.html as index.html)
Live URL:    https://murali-chalamala.github.io/rk-mutt-french-workbook/
```

### PDF Files (upload to pdfs/ folder in main repo)
```
pdfs/festival_main_book.pdf
pdfs/festival-workbook.pdf
pdfs/festival_transcript.pdf
pdfs/mon-passeport-01_smart-board.pdf
pdfs/mon-passeport-03_smart-board.pdf
```

---

## 📊 App Statistics

| Stat | Value |
|---|---|
| Days of content | 17 |
| Verb tables | 14 |
| Pronunciation hints | 97+ |
| Numbers covered | 0–100 (101 words) |
| Quiz types | 8 |
| Conversations | 7 full dialogues |
| PDF books | 5 |
| localStorage keys | 10 |
| Workbook exercise types | 7 |
| Total app size | ~590 KB (both files) |

---

## 🏆 Version History

| Version | Changes |
|---|---|
| v1.0 | Days 1–12 · Flashcards · Quiz · Fill |
| v1.5 | Days 13–15 · Homework tabs · CER/GER/Dire/Faire |
| v2.0 | Days 16–17 · Workbook tab · PDF Library · About · Progress · Review All · Pro Lab · Global footer · Share · Keyboard shortcuts · Theme persistence · Day completion celebration |

---

*RK Mutt French Junior · Version 2.0 · Built with ❤️ by Murali Krishna Chalamala (RK Mutt Student)*
