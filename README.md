# 🔥 GitHive — GitHub Activity Heatmap

A beautiful, responsive GitHub activity heatmap that visualizes any public user's contribution patterns. Built as a standalone HTML file with zero dependencies.

![GitHive Preview](https://img.shields.io/badge/status-live-brightgreen)
![Size](https://img.shields.io/badge/size-40KB-blue)
![Themes](https://img.shields.io/badge/themes-3-orange)

👉 **Live demo:** `https://nwfella.github.io/github-activity-heatmap`

---

## Features

- **📅 Contribution Heatmap** — GitHub-style 12-week grid showing daily activity
- **📊 Stats Dashboard** — Total events, active days, current streak, best day, longest streak
- **📂 Repo Filter** — Click any repo to see activity for just that project
- **📊 Language Breakdown** — Automatic language detection from repos you've pushed to
- **⚡ Activity Breakdown** — See pushes, PRs, issues, stars, forks at a glance
- **🎨 3 Themes** — Dark (default), Light, and Blue ocean — smoothly animated
- **🔍 Tooltip Hover** — Hover any cell to see exact count and date
- **🔑 Optional Token** — Add a GitHub token for higher rate limits
- **📱 Fully Responsive** — Works on desktop, tablet, and mobile
- **💾 Persistent** — Saves your last username, theme, and token in localStorage

## Usage

1. **Open** the app (GitHub Pages or just open `index.html`)
2. **Enter** any GitHub username
3. **Hit Enter** or click **Load**
4. **Explore** — hover cells, filter by repo, switch themes

Or click **🎲 Random** to see a random popular developer's activity.

## Themes

| Theme | Preview |
|-------|---------|
| 🌙 Dark | GitHub-dark inspired, easy on the eyes |
| ☀️ Light | Clean white background, high contrast |
| 🌊 Blue | Deep ocean blues, vibrant accents |

Click the theme buttons in the top-right corner to switch.

## Deployment

### GitHub Pages (recommended)

```bash
git clone https://github.com/nwfella/github-activity-heatmap
cd github-activity-heatmap
git push origin main
```

Then enable GitHub Pages in repo Settings → Pages → Source: `main` → root.

### Local

Just open `index.html` in any browser — it's a single file with no build step.

## Tech Stack

- **Vanilla JS** — No frameworks, no build tools
- **CSS Grid** — For the heatmap layout
- **CSS Custom Properties** — Theme system
- **GitHub REST API v3** — Events + Languages endpoints
- **localStorage** — Persistence

## API Notes

- **No auth**: 60 requests/hour (IP-based)
- **With token**: 5,000 requests/hour — add your `ghp_xxx` token in the UI
- Fetches up to 400 recent public events (4 pages × 100)

## License

MIT — use it, fork it, show it off on your portfolio.
