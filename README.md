# GRE Vocab — GregMat Edition
 
A full-featured GRE vocabulary study app built as a Progressive Web App (PWA). All 32 GregMat groups (~900 words) with flashcards, quizzes, and a personalised study plan targeting your exam date.
 
---
 
## Features
 
### Study Modes
- **Study Table** — all words in a group laid out as a table (word, type, meaning, example). Hide/show columns to self-test. Star words to highlight them.
- **Flashcard** — colour-coded by knowledge status. Flip to reveal definition, root word, antonym, and word family.
- **Quiz** — pick the right word from 4 options based on the definition.
- **Fill in the Blank** — guess the word from a gapped example sentence.
- **Antonym Drill** — pick the opposite of a given word.
- **Confused Words** — side-by-side comparison of easily mixed-up pairs (e.g. *flout/flaunt*, *tortuous/torturous*).
- **Word List** — searchable list of all words with status badges.
### Flashcard Features
- Cards colour-coded: **plain** = new, **amber** = familiar, **green** = known
- Rate with keyboard: `Z` new · `X` familiar · `C` got it
- Navigate: `←` prev · `→` next · `Space` flip · `R` restart
- Pronunciation: `V` key or ▶ button
- Shows root word, antonym, and word family after reveal
### Progress & Stats
- Progress auto-saved to browser `localStorage`
- Export/import progress as JSON (backup or transfer between devices)
- Stats page: streak, cards rated today, mastery %, 14-day activity chart, weakest words list
- Milestone badges with confetti at 50 / 100 / 250 / 500 / 750 / 900 words known
- Session timer
### Study Plan
- Personalised plan from today to **July 31, 2025** (exam date)
- Days 1–16: learn all 32 groups (2/day) — Study Table + Flashcard + Quiz
- Days 17–25: heavy review of weak words
- Days 26–35: full quiz sweeps + Confused Pairs + Fill Blank
- Days 36–45: Antonym drill + weak word hammering
- Days 46+: final polish
- Daily checkboxes, time breakdowns, and direct jump buttons
- Reset all progress button for a clean slate
---
 
## Files
 
```
gre_vocab.html   ← main app (open this in browser)
manifest.json    ← PWA manifest
sw.js            ← service worker (offline support)
README.md
```
 
All three files must be in the same folder/directory.
 
---
 
## Install as Android App (PWA)
 
1. Upload all three files to **GitHub Pages** or **Netlify**
2. Open the hosted URL in **Chrome on Android**
3. Tap **⋮ menu → Add to Home Screen**
4. The app installs with a fullscreen launcher icon and works offline
### GitHub Pages setup
1. Push the files to a GitHub repo
2. Go to **Settings → Pages**
3. Set source to `main` branch, root folder
4. Your URL will be `https://yourusername.github.io/repo-name/gre_vocab.html`
---
 
## Usage
 
### Getting started
1. Open `gre_vocab.html` in any modern browser (Chrome recommended)
2. Click a group in the sidebar to begin
3. Start with **Study Table** to read through the words, then switch to **Flashcard**
### Recommended daily workflow
1. **Study Table** — read through the day's 2 groups (35 min)
2. **Flashcard** — go through all words, rate with Z/X/C (30 min)
3. **Quiz** — test yourself on the same group (25 min)
4. Check the day off in the **Study Plan**
### Keyboard shortcuts (Flashcard mode)
| Key | Action |
|-----|--------|
| `Space` | Flip card |
| `←` | Previous card |
| `→` | Next card |
| `Z` | Rate: New to me |
| `X` | Rate: Familiar |
| `C` | Rate: Got it |
| `V` | Pronounce word |
| `R` | Restart deck (resets ratings) |
 
---
 
## Progress & Backup
 
Progress is saved automatically in your browser's `localStorage`. To back it up or move it to another device:
 
- Click **↓ Export** in the sidebar to download a `.json` file
- Click **↑ Import** on another device to restore it
---
 
## Study Plan Timeline
 
| Phase | Days | Focus |
|-------|------|-------|
| Learn | 1–16 | 2 new groups/day — all 32 groups covered |
| Review | 17–25 | Weak words + full quiz sweeps |
| Drill | 26–35 | Confused pairs, fill blank, quiz |
| Drill | 36–45 | Antonym drill + weak word hammering |
| Final | 46+ | Light daily review until exam |
 
**Exam date: July 31, 2025**
 
---
 
## Word Data
 
All words sourced from the **GregMat 32-group vocabulary list** (~900 words). Each word includes:
- Definition
- Part of speech
- Example sentence
- Root word (Latin/Greek etymology)
- Antonym (where applicable)
- Word family (related words)
---
 
## Tech Stack
 
- Vanilla HTML/CSS/JavaScript — zero dependencies, zero build step
- `localStorage` for progress persistence
- Web Speech API for pronunciation
- Service Worker for offline support
- PWA manifest for home screen installation
---
 
*Built for GRE prep. Good luck on July 31! 🎓*
 
