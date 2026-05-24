# German Alphabet Learning Website — Design Spec

## Overview
A single-file HTML website for learning German letters with pronunciation. Users click cards or press keyboard keys to hear correct German letter pronunciation via Web Speech API.

## Features
- All 30 German letters displayed as interactive cards:
  - A–Z (standard Latin alphabet)
  - Ä, Ö, Ü (umlauts)
  - ß (Eszett)
- Each card shows: uppercase letter, lowercase letter, example German word, Chinese translation
- Click card or press keyboard key to pronounce the letter in German
- Special key mappings for umlauts and ß
- Visual feedback on click/keypress (highlight + scale animation)
- Responsive card grid layout
- German flag color accents (red/gold/black)

## Technical Approach
- **Single HTML file** — HTML + CSS + JS in one file
- **Web Speech API** (`SpeechSynthesis`) with `lang='de-DE'` for pronunciation
- **CSS Grid / Flexbox** for responsive card layout
- **CSS animations** for interaction feedback
- No external dependencies, no build step

## Keyboard Mapping
| Key | Letter |
|-----|--------|
| a–z | A–Z |
| [   | Ä      |
| ]   | Ö      |
| \   | Ü      |
| -   | ß      |

## Letter Data
Standard letters A–Z plus:
- Ä/ä — Ärger (anger)
- Ö/ö — Öl (oil)
- Ü/ü — Über (over)
- ß — Straße (street)

## Visual Design
- Clean card style with frosted-glass (backdrop-filter) effect
- Each card ~120x140px with subtle shadow
- Grid auto-fills to screen width
- Active state: card lifts + border highlight
- Background: light gradient

## Constraints
- Must work offline (no external resources)
- Must work in modern browsers (Chrome, Edge, Firefox, Safari)
- Web Speech API voice quality depends on OS/browser speech engine
