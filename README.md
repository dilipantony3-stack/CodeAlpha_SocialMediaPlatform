# Vibe 🎨

**A mood-driven social media platform frontend.**

Vibe reimagines the social feed around emotional state instead of 
just chronology or engagement. Set your mood on an interactive 
gradient spectrum, and watch the feed re-sort by emotional proximity, 
posts pick up mood-colored borders, and reactions burst into 
colored particles.

Built as a **single-file, zero-build** HTML/CSS/JS app — no 
frameworks, no bundlers, just open it in a browser. Data structures 
map directly onto Django models, with a working Django backend 
included (`feed` app, seed data, admin-ready).

## ✨ Features

- **Mood Spectrum Bar** — click a gradient to set your emotional state
- **Mood Match Feed Sorting** — posts reordered by emotional proximity
- **Micro-Thoughts** — 60-character quote-card posts in Space Grotesk
- **Reaction Particle Bursts** — colored particles explode on reaction
- **Voice Dictation** — Web Speech API, animated waveform while recording
- **Story Carousel** — auto-advancing stories, gradient rings, tap nav
- **Live Typing Indicators** — simulated real-time presence in comments
- **Three Themes** — Dark, Warm, Aurora (animated gradient accents)
- **Interactive Polls** — animated fill bars on vote
- **Mood Board Widget** — visual cluster of mood-weighted dots

## 🛠️ Tech

- **Frontend:** Vanilla HTML/CSS/JS, CSS custom properties for theming, 
  event delegation, `requestAnimationFrame` for story progress
- **Backend:** Django 4.2+, SQLite, Pillow — models map 1:1 to the 
  frontend's data layer (`User`, `Post`, `Comment`, `Reaction`, 
  `Story`, `Poll`, `Bookmark`)
- Responsive: desktop 3-column → tablet 2-column → mobile single-column 
  with bottom nav
- Accessible: ARIA labels, `prefers-reduced-motion`, keyboard shortcuts 
  (H/E/N, arrows, Esc)

## 🚀 Quick start

**Frontend only** (static, no backend needed):
```bash
# just open index.html, or serve it:
python3 -m http.server 8000
```

**Full stack with Django:**
```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\Activate.ps1
pip install -r requirements.txt
python manage.py migrate
python seed_data.py
python manage.py runserver
```

## 📸 Demo
[Live demo link] · [Screen recording / GIF]

## 📄 License
[Your choice — MIT is common for portfolio projects]
