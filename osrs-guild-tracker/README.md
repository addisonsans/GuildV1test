# OSRS Guild Tracker ⚔️

A free, open-source clan management tool for Old School RuneScape. Track your guild's progress with color-coded skill tiers, leaderboards, goals, and more.

**Powered by [WiseOldMan](https://wiseoldman.net) API**

![Preview](preview.png)

## Features

- 🎨 **Color-coded skill tiers** - Instantly see member progress at a glance
- 👥 **Member overview** - Browse all clan members with sortable stats
- 🏆 **Leaderboards** - Rankings for any skill or total level
- 🎯 **Guild goals** - Set group goals and track completion
- ⚔️ **Competitions** - View ongoing, upcoming, and past competitions
- 📊 **Dashboard** - Quick stats and top performers

## Color Tier System

| Level Range | Color |
|-------------|-------|
| 1-9 | Gray |
| 10-19 | Purple |
| 20-29 | Blue |
| 30-39 | Teal |
| 40-49 | Cyan |
| 50-59 | Lime |
| 60-69 | Yellow |
| 70-79 | Orange |
| 80-89 | Coral |
| 90-98 | Magenta |
| 99 | Green ✓ |

## Quick Start

### Option 1: Use it directly
Just open `index.html` in your browser - no build step required!

### Option 2: Deploy to GitHub Pages (recommended for sharing)

1. **Create a GitHub account** (if you don't have one)
   - Go to [github.com](https://github.com) and sign up

2. **Create a new repository**
   - Click the `+` button → "New repository"
   - Name it `osrs-guild-tracker` (or whatever you want)
   - Make it **Public**
   - Click "Create repository"

3. **Upload the files**
   - On your new repo page, click "uploading an existing file"
   - Drag and drop ALL the files from this folder:
     - `index.html`
     - `src/App.jsx`
   - Click "Commit changes"

4. **Enable GitHub Pages**
   - Go to your repo's **Settings** → **Pages**
   - Under "Source", select **Deploy from a branch**
   - Select **main** branch and **/ (root)** folder
   - Click **Save**

5. **Wait ~2 minutes**, then visit:
   ```
   https://YOUR-USERNAME.github.io/osrs-guild-tracker
   ```

That's it! Share that link with your clan.

## How It Works

1. **Search or enter your WiseOldMan Group ID** on the landing page
2. The app fetches your clan's data from the WiseOldMan API
3. **Goals are saved locally** in your browser (per guild)

### Finding Your WiseOldMan Group

1. Go to [wiseoldman.net/groups](https://wiseoldman.net/groups)
2. Search for your clan
3. Your Group ID is in the URL: `wiseoldman.net/groups/[ID]`

If your clan isn't on WiseOldMan yet, you can [create a group](https://wiseoldman.net/groups/create) for free.

## Customization

### Change colors
Edit the CSS variables in `index.html`:

```css
:root {
  --accent: #f59e0b;        /* Main accent color */
  --bg-dark: #0f1115;       /* Background */
  --tier-99: #22c55e;       /* Level 99 color */
  /* etc... */
}
```

### Add more features
The app is a single React file (`src/App.jsx`). Feel free to fork and modify!

## Tech Stack

- **React 18** (via CDN, no build step)
- **WiseOldMan API** for player data
- **LocalStorage** for goals persistence
- **GitHub Pages** for free hosting

## Contributing

Pull requests welcome! Some ideas:
- Individual player goals
- XP gained over time charts
- Boss KC tracking
- Achievement diaries progress
- Discord webhook notifications

## License

MIT - Do whatever you want with it.

## Credits

- [WiseOldMan](https://wiseoldman.net) - The amazing API that powers this
- [Jagex](https://www.jagex.com) - For creating OSRS

---

Made with 💛 for the OSRS community
