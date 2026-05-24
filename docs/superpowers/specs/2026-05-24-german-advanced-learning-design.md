# German Advanced Learning Website — Design Spec

## Overview
Extend the existing alphabet learning website into a multi-section German learning tool with tab navigation.

## Sections
5 sections accessible via top tab bar:

1. **Alphabet** — existing 30 letters (A–Z, Ä, Ö, Ü, ß) with example words, unchanged
2. **Phonics** — 14 common German letter combinations: ch, sch, sp, st, ei, ie, eu, äu, ck, tz, pf, qu, ng, nk — each with example word
3. **Numbers** — 0–20 with German name and pronunciation
4. **Phrases** — 15 essential daily phrases (greetings, thanks, introductions)
5. **Vocabulary** — ~30 words across colors, family, food categories

## Technical Approach
- Single HTML file, tab-based SPA
- Each tab hides/shows its grid
- All cards follow same click-to-pronounce pattern
- Vocab section uses sub-category labels (color-coded tags)
- Same visual style (glassmorphism, multi-color cards)

## Data Changes
- Alphabet data stays the same
- Phonics: `{ combo: 'sch', word: 'Schule', trans: '学校' }`
- Numbers: `{ number: 13, german: 'dreizehn', trans: '十三' }`
- Phrases: `{ phrase: 'Guten Morgen', trans: '早上好' }`
- Vocabulary: `{ word: 'rot', trans: '红色', category: '颜色' }`

## Architecture
- Tab bar as horizontal scrollable nav
- Section grids as switchable div containers
- Shared `speak()` function
- Active tab persists via URL hash for bookmarkability
