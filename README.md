# HN Live

A real-time feed of the newest stories from Hacker News.

**Live**: https://hn-live-feed.vercel.app

## Features

- **Live updates** - New stories appear automatically every 10 seconds
- **Infinite scroll** - Load older stories as you scroll down
- **Keyboard navigation** - j/k to navigate, Enter to open
- **Offline resilient** - Cached stories display instantly on refresh
- **Dark mode** - Follows system preference
- **Accessible** - Skip links, reduced motion support, screen reader friendly
- **Zero dependencies** - Single HTML file, vanilla JS

## Keyboard shortcuts

| Key | Action |
|-----|--------|
| `j` | Select next story |
| `k` | Select previous story |
| `gg` | Go to top |
| `Enter` | Open selected story |

## How it works

Polls the [Hacker News Firebase API](https://github.com/HackerNews/API) for new stories. When you're at the top of the page, new stories slide in automatically. When you're scrolled down reading, a chip appears showing how many new stories are available.

## Development

```bash
# Serve locally
python3 -m http.server 8000

# Open http://localhost:8000
```

## Deploy

Push to GitHub and connect to Vercel, or:

```bash
vercel --prod
```

## License

MIT
