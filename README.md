# Drip Landing Page

> Software that runs itself within your budget.

## About Drip

Drip is the first agent-native SaaS billing layer. An AI agent manages your resource lifecycle in real time — monitoring credits, making tradeoffs under budget pressure, and gracefully scaling containers to zero when funds run low.

Unlike traditional billing (Stripe + cron jobs), the Drip agent *thinks*:
- Monitors credit balances via PayWithLocus in real time
- Proactively messages customers when credits are running low
- Makes budget-aware tradeoffs: reduces crawl frequency, skips lower-signal sources, switches to cheaper synthesis
- Gracefully tears down containers at $0, preserving state in Postgres
- Auto-restores containers when customers top up

## Design Philosophy

**Apple-Minimalist:** Clean, spacious, purposeful. Generous whitespace. Clear visual hierarchy.

**Locus-Inspired:** Technical authenticity. Modular design. API-first vibe. Status indicators and data visualization.

**Agent-First:** The landing page feels alive. Live agent logs, status transitions, and budget tradeoffs are visible in real time.

## Tech Stack

- **Framework:** [Astro](https://astro.build/) - Fast, modern static site generation
- **Styling:** Tailwind CSS v4 - Utility-first CSS
- **Typography:** Inter (UI) + JetBrains Mono (logs)
- **Deployment:** Vercel / Netlify / GitHub Pages

## Local Development

```bash
# Install dependencies
npm install

# Start dev server
npm run dev

# Build for production
npm run build
```

## Project Structure

```
├── src/
│   ├── pages/
│   │   └── index.astro     # Landing page (all sections)
│   └── styles/
│       └── global.css      # Custom utilities
├── public/                  # Static assets
└── dist/                    # Build output (ignored)
```

## Sections

1. **Hero** — Value proposition + live agent demo card
2. **How It Works** — 4-step process (Provision → Monitor → Think → Restore)
3. **Agent Difference** — Side-by-side comparison table
4. **Live Demo** — Terminal-style agent log visualization
5. **Architecture** — Locus stack visualization
6. **Self-Hosting** — "Skin in the game" narrative
7. **CTA** — Demo access and GitHub links

## Credits

Built for **Locus Paygentic Week 2** — $1,000 prize hackathon, April 20-22 2026.

- PayWithLocus — agent wallet management
- BuildWithLocus — container lifecycle management
- AgentMail — autonomous user notifications

## License

MIT — Fork it, build your own agent-native SaaS.
