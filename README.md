# BBC Towards Advanced – Companion App

A PWA (Progressive Web App) companion for the BBC Learning English *Towards Advanced* course. Works on iPhone, Android, and desktop. Syncs progress across all devices via a private GitHub Gist.

---

## 🚀 Deploy to GitHub Pages (5 minutes)

### Step 1 — Create a GitHub repository
1. Go to [github.com/new](https://github.com/new)
2. Name it `bbc-companion` (or anything you like)
3. Set it to **Public** (required for free GitHub Pages)
4. Click **Create repository**

### Step 2 — Upload the app files
Upload all four files from this folder:
- `index.html`
- `manifest.json`
- `sw.js`
- `icon-192.png`
- `icon-512.png`
- `apple-touch-icon.png`

You can drag & drop them all at once on the GitHub repository page.

### Step 3 — Enable GitHub Pages
1. In your repo, go to **Settings → Pages**
2. Under *Source*, select **Deploy from a branch**
3. Choose **main** branch, **/ (root)** folder
4. Click **Save**

After ~1 minute, your app is live at:
```
https://YOUR-USERNAME.github.io/bbc-companion/
```

---

## 📱 Install on iPhone (Add to Home Screen)

1. Open Safari on your iPhone (must be Safari, not Chrome)
2. Go to your GitHub Pages URL above
3. Tap the **Share** button (box with arrow pointing up)
4. Scroll down and tap **"Add to Home Screen"**
5. Tap **Add**

It will appear on your home screen as a full-screen app with no browser bars.

---

## 🔄 Set up cross-device sync

The app uses a **secret GitHub Gist** as a tiny personal database — free, private, and no server needed.

1. Go to [github.com/settings/tokens/new](https://github.com/settings/tokens/new)
2. Give it a name like `bbc-companion`
3. Under *Scopes*, tick **only `gist`** — nothing else
4. Click **Generate token** → copy it immediately
5. Open the app → tap **⚙️ Settings** → paste your token → tap **Connect & Sync**

Do this on each device once. They'll all share the same Gist automatically.

---

## 💡 How to use

| Action | What it does |
|--------|-------------|
| Tap a session tile | Opens the BBC lesson in your browser |
| **Long-press** a session button (mobile) | Marks it as done ✓ |
| Right-click a session button (desktop) | Marks it as done ✓ |
| Tap ↻ in the header | Manually pulls latest progress from other devices |

Progress auto-saves to your GitHub Gist within 1 second of any change.

---

## 📂 Files

| File | Purpose |
|------|---------|
| `index.html` | The entire app |
| `manifest.json` | Makes it installable as a PWA |
| `sw.js` | Service worker — enables offline use |
| `icon-*.png` | App icons |
