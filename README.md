A lightweight static prototype for an **OSRS Armory-style** player lookup site.

## Current scope (v0)

- Single-page UI in `index.html`.
- Rune-themed dark visual style.
- Player search form for OSRS names.
- Attempts live hiscores fetch from the OSRS endpoint.
- Graceful fallback to demo profile data if browser/API restrictions block live requests.

## Why demo fallback exists

OSRS hiscores access from client-side JavaScript can fail in some browsers/environments due to CORS/network policies. This repo keeps a demo profile fallback so UX and layout work can continue while API strategy is finalized.

## Local development

```bash
python3 -m http.server 8080
```

Then open <http://localhost:8080>.

## Next milestones

1. Add backend proxy endpoint for reliable live hiscores.
2. Expand skills/boss stats coverage.
3. Add shareable profile URLs and recent searches.
