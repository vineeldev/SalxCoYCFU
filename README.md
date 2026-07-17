# SalxCo & YCFU × Lyric — Partnership Structure Dashboard

Interactive scenario dashboard for the SalxCo / YCFU partnership discussion.
Single static HTML file, no build step, no dependencies (logo is embedded).

## Structure
- `index.html` — the entire dashboard (markup, styles, model logic)

## Deploy on Vercel
1. Import this repo at vercel.com/new
2. Framework preset: **Other** · Build command: none · Output directory: `.`
3. Deploy — every push to `main` redeploys automatically

## Updating deal terms
All model inputs live in one config block near the top of the `<script>` in `index.html`:

- `OFFERS.original` / `OFFERS.revised` — price, rollover %, deferral schedule, exit multiple, outperformance, distribution timing
- `UNADJ`, `ADJ_EBITDA_BASE`, `AVG_EBITDA_2731` — projection constants from the underlying model

Edit, commit, push.
