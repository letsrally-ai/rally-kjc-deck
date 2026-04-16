# Project: Rally KJC Campaign Deck

> **WORK HERE** — Project context only. Keep under 25 lines.

## Overview
Single-file HTML presentation deck for Rally AI × Katong–Joo Chiat partner campaign.

## Project-Specific Notes
- Stack: Vanilla HTML/CSS/JS, no build tool
- Main file: `index.html` (~2640 lines, 8 slides)
- Map source: `../rally-kjc/` — Leaflet map + `data/outlets.json` (800+ KJC outlets)
- Map live: https://letsrally-ai.github.io/rally-kjc/
- Skills: symlinked via sync-skills.sh (18 skills available)

## Slides
1. Cover | 2. What is Rally | 3. Intelligence | 4. Why Consumers
5. KJC Campaign (map embed: `#mapLayer`) | 6. Merchants
7. Data Privacy | 8. Partnership (KJCBA / Alibabar / Anywheel / Grab tabs)

## Partner URLs
- `?p=kjcba | ?p=alibabar | ?p=anywheel | ?p=grab` → partner's tab only, tab bar hidden
- No param → internal view, all slides + all tabs
- Adding a new partner → see `.claude/rules/partners.md`
