# 🎮 The Jump Game

A retro-arcade vertical platformer. Bounce higher and higher, beat your top 10 high scores!

**Live:** `https://YOUR_USERNAME.github.io/the-jump-game/`

---

## 🚀 Deploy in 3 Steps

### 1. Create the GitHub Repo
Go to [github.com/new](https://github.com/new):
- Name: **`the-jump-game`**
- Visibility: **Public**
- **Leave completely empty** (no README, no .gitignore)

### 2. Push the Code
```bash
cd the-jump-game          # folder containing these files
git init
git add .
git commit -m "Initial commit: The Jump Game"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/the-jump-game.git
git push -u origin main
```

### 3. Enable GitHub Pages
1. Open your repo on GitHub → **Settings** → **Pages**
2. Under **Source** select **GitHub Actions**
3. Click **Save**

The Actions workflow fires automatically on every push. Wait ~2 minutes, then visit:

```
https://YOUR_USERNAME.github.io/the-jump-game/
```

---

## 🎮 Controls

| Input | Action |
|---|---|
| `←` / `A` | Move left |
| `→` / `D` | Move right |
| Mobile swipe | Move left / right |

Bounce is **automatic** — just land on a platform!

---

## 📊 Features

- ✅ Physics-based bouncing with squash & stretch animation
- ✅ Procedurally-generated infinite platforms
- ✅ Dynamic background (city dusk → deep space with stars)
- ✅ Particle burst on each bounce
- ✅ Top-10 persistent leaderboard (localStorage, Safari-safe)
- ✅ NEW BEST badge when you beat your record
- ✅ HiDPI / Retina canvas (Device Pixel Ratio aware)
- ✅ Responsive layout — desktop & mobile
- ✅ Zero dependencies — single `index.html`
- ✅ GitHub Actions auto-deploy

---

## 🛠️ Local Development

No build step required:

```bash
# Python
python3 -m http.server 8000

# Node.js
npx http-server .
```

Then open `http://localhost:8000`.

---

## 📁 File Structure

```
the-jump-game/
├── index.html                   # Complete game
├── README.md
├── .gitignore
└── .github/
    └── workflows/
        └── deploy.yml           # Auto-deploy to GitHub Pages
```

---

## ⚙️ Customisation

Edit the `CONFIG` object near the top of `index.html`:

| Key | Default | Effect |
|---|---|---|
| `gravity` | `900` | Physics feel |
| `jumpVelocity` | `520` | Bounce height |
| `maxHorizontalSpeed` | `240` | Movement speed |
| `platformSpacingMin/Max` | `70 / 115` | Gap between platforms |
| `leaderboardSize` | `10` | Number of scores saved |

---

## 🐛 Debugging

Open browser DevTools → Console.

```js
// Clear the leaderboard
localStorage.removeItem('jump-game-leaderboard-v2');
```

---

## 📄 License

MIT — use freely, modify, share!