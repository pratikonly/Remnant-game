# REMNANT — Open World Survival Game
### Deploy to Vercel in 3 steps

---

## 🚀 Deploy to Vercel

### Option 1 — Vercel CLI (Fastest)
```bash
npm i -g vercel
cd remnant-vercel
vercel --prod
```

### Option 2 — Vercel Dashboard (No-code)
1. Go to **vercel.com/new**
2. Drag & drop this entire `remnant-vercel/` folder
3. Click **Deploy**
4. Your game is live at `https://remnant-xxxx.vercel.app` 🎉

### Option 3 — GitHub + Vercel (Auto-deploy)
```bash
git init
git add .
git commit -m "REMNANT v1.0"
gh repo create remnant --public --push
# Connect repo at vercel.com/import → auto-deploys on every push
```

---

## 📁 Project Structure
```
remnant-vercel/
├── vercel.json          ← Routing, headers, CDN config
└── public/
    ├── index.html       ← Main menu (animated background, how-to-play)
    ├── game.html        ← Full game (2500+ lines, all phases)
    ├── manifest.json    ← PWA manifest (install as app)
    ├── sw.js            ← Service Worker (offline caching)
    └── icon.svg         ← App icon
```

---

## 🎮 What's In The Game

| Phase | Feature |
|-------|---------|
| 1 | Procedural terrain · Sky shader · Day/night cycle · Campfire |
| 2 | Full player model + skeleton · Walk/sprint/idle animations · Survival stats |
| 3 | Enemy AI (4 types) · Combat · Crafting (12 recipes) · Building system |
| 4 | Simulated multiplayer · Chat · Minimap · Weather · Mobile joysticks · Audio |
| 5 | PWA · Service Worker · FPS counter · Wake lock · Production polish |

---

## ⚙️ Controls

| Key | Action |
|-----|--------|
| WASD | Move |
| Mouse | Look (click to lock) |
| Shift | Sprint |
| Space | Jump |
| LMB | Attack |
| E | Interact / Pick up |
| I | Inventory |
| C | Crafting bench |
| B | Build mode |
| F | Toggle first/third person |
| T | Chat |
| 1-5 | Hotbar slots |
| ESC | Close panels |

---

## 📱 Mobile
- Auto-detected touch controls (joystick + action buttons)
- Installable as PWA — add to home screen
- Adaptive quality for low-end GPUs
- Screen wake lock prevents sleep mid-game

---

## 🔧 Performance Tips

- The game targets **60 FPS** on mid-range hardware
- Use **Settings panel (⚙)** in-game to reduce shadows/fog/quality
- For best experience use **Chrome or Edge** (best WebGL2 support)
- Hosted on Vercel's **global edge network** — fast from anywhere

---

## 🌐 Vercel Free Tier Limits
- ✅ 100GB bandwidth/month
- ✅ Unlimited deployments
- ✅ Custom domain (free)
- ✅ HTTPS by default
- ✅ Global CDN

---

*Built by Claude (Anthropic) · Three.js · WebGL2 · Web Audio API*
