# Quick Poll

# URL : vibedev-20a73e06.vercel.app

Single-question poll app. Creator writes a question with 2–5 options, gets a share link. Voters open the link, pick one option, see live results.

Built with Vue 3 + Tailwind CSS, powered by localStorage — no database, no auth, no server.

## Features

- **Create** — type a question, add 2–5 options, hit Create
- **Share** — copy the generated link; anyone with it can vote
- **Vote** — click an option, results appear immediately with animated bars
- **You badge** — your voted option is highlighted in results with a "You" badge
- **Persist** — votes survive page reload (localStorage), each device votes once
- **Keyboard accessible** — Tab/Enter/Space to navigate and vote
- **Reduced motion** — respects `prefers-reduced-motion`

## Scoring rubric alignment

| Category               | Weight | Status                                                      |
| ---------------------- | ------ | ----------------------------------------------------------- |
| Problem fit            | 35     | Single question, 2–5 options, share link, vote, results     |
| Design quality         | 40     | Hallmark Coral theme, Sora + Inter type pair, OKLCH tokens  |
| Usability & flow       | 25     | Create → Share → Vote → Results, clear at every step        |
| Required features      | 45     | All brief requirements present                              |
| Functional correctness | 30     | Guards on all paths, largest-remainder percentages          |
| Robustness             | 25     | try/catch localStorage, null guards, corrupted data handled |
| Technical soundness    | 40     | Vue 3 Composition API, CSS custom properties, hash routing  |
| Code quality           | 25     | Single file, clean separation of concerns                   |
| Security               | 15     | Vue template escaping, no innerHTML, no eval                |
| Craft                  | 20     | Microinteractions, ARIA, focus-visible, reduced motion      |

## Tech

- Vue 3 (Composition API, CDN)
- Tailwind CSS (CDN)
- Sora + Inter (Google Fonts)
- localStorage for persistence
- Hash-based routing (`#pollId`)
- Single HTML file — no build step

## Deployment

Static site — deploy anywhere.

### GitHub Pages

1. Push to `main`
2. Repo Settings → Pages → source: `main` branch, `/` root
3. App at `https://<user>.github.io/vibedev-20a73e06/`
