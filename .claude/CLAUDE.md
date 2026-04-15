# Project: Rally KJC Campaign Deck

> **WORK HERE** — Project context only. Keep under 25 lines.

## Overview
Single-file HTML presentation deck for Rally AI × Katong–Joo Chiat partner campaign.

## Project-Specific Notes
- Stack: Vanilla HTML/CSS/JS, no build tool
- Main file: `rally-kjc-deck_1.html` (696 lines, 8 slides)
- Map source: `../rally-kjc/` — Leaflet map + `data/outlets.json` (800+ KJC outlets)
- Map live: https://letsrally-ai.github.io/rally-kjc/
- Skills: symlinked via sync-skills.sh (18 skills available)

## Slides
1. Cover | 2. What is Rally | 3. Intelligence | 4. Why Consumers
5. KJC Campaign (map embed target: `#mapLayer`) | 6. Merchants
7. Partnership (KJCBA / Alibabar / Anywheel tabs) | 8. Data Privacy

## Partner URLs
- `?p=kjcba` → 8 slides, KJCBA partnership tab only
- `?p=alibabar` → 8 slides, Alibabar tab only
- `?p=anywheel` → 8 slides, Anywheel tab only
- No param → internal view, all 8 slides + all tabs
