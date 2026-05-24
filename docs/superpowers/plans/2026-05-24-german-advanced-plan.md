# German Advanced Learning — Implementation Plan

**Goal:** Extend the alphabet website into a multi-section German learning tool.

**Architecture:** Single `index.html` rewritten with tab-based SPA structure. Five sections (Alphabet, Phonics, Numbers, Phrases, Vocabulary) with tab navigation. All existing alphabet functionality preserved.

**Tech Stack:** Vanilla HTML5, CSS3, Web Speech API

---

### Task 1: Rewrite index.html with multi-section architecture

**Files:**
- Modify: `D:/cc_the_first/index.html` — full rewrite

**Changes:**
1. Add tab navigation bar with 5 tabs
2. Restructure content into 5 section containers
3. Add data for Phonics, Numbers, Phrases, Vocabulary sections
4. Add tab switching JS logic with URL hash support
5. Preserve all existing alphabet card behavior
6. Apply consistent styling for cards across all sections
7. Add vocabulary category tags
