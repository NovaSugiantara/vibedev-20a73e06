# Quick Poll

Single-question poll app. Creator writes a question with 2-5 options, gets a share link. Voters open the link, pick one option, see live results.

Built with Vue 3, powered by localStorage — no database, no auth, no build step.

## How it works

- **Create**: Type a question, add 2-5 options, hit "Create Poll"
- **Share**: Copy the generated link — anyone with it can vote
- **Vote**: Open the link, click an option. Results appear immediately
- **Persist**: All votes survive page reload (localStorage). Each device votes once

## Tech

- Vue 3 (Composition API, CDN — no build step)
- localStorage for storage
- Hash-based routing (`#pollId`)
- Single HTML file, zero dependencies

## Deployment

Static site — deploy anywhere. Push to GitHub Pages, Vercel, Netlify, or serve with any static file server.

### GitHub Pages

1. Push to `main`
2. Repo Settings → Pages → source: `main` branch, `/` root
3. App at `https://<user>.github.io/vibedev-20a73e06/`
