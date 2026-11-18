# The Omyca Award ✦

> The world's most prestigious film honour, as far as we are aware.

**Live: https://omyca-award.pages.dev**

A movie world-cup knockout game. You are appointed the sole judge of one of eight juries (Action, Comedy, Drama, Sci-Fi, Horror, Romance, Documentary or Animation) and must whittle 48 well-known films down to a single Diamond winner. The Committee (population: you) thanks you for your service.

## How it plays

1. **Preliminaries**: 12 groups of 4; advance the two least disappointing from each.
2. **The Second Chances Committee**: 8 of the 24 dismissed films are graciously un-eliminated.
3. **Knockout**: 32 → 16 → 8 → 4 → 2 → 1, one duel at a time.
4. **The Ceremony**: spotlight reveal, crown bestowal, an acceptance speech of questionable sincerity.
5. **The Official Record**: sign your name, watch the road-to-glory roadmap animate, and download the sealed certificate (PNG).

## Tech

- One self-contained `index.html`: no build, no framework, no dependencies.
- 8 × 48 = 384 films with real poster art (TMDB image CDN, verified links, graceful fallbacks).
- Canvas-drawn certificate with a stamped judge's seal; trailers open as YouTube searches in a new tab.
- All state lives in memory. Two fonts only: Archivo & Instrument Serif.
- Hosted on Cloudflare Pages. Costs nothing to run, which the Committee considers excellent taste.

## Develop & deploy

Open `index.html` in a browser. That's the development environment.

```bash
npx wrangler pages deploy . --project-name=omyca-award --branch=main --commit-dirty=true
```

---

*The Omyca Award is entirely unaffiliated with any similarly named ceremony. Any resemblance is a coincidence we are rather pleased with.*
