# German Alphabet Learning Website — Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Build a single-file HTML website for learning German letters with keyboard/click pronunciation.

**Architecture:** Single `index.html` with embedded CSS and JS. Uses Web Speech API for pronunciation, CSS Grid for responsive layout. No build step or dependencies.

**Tech Stack:** Vanilla HTML5, CSS3 (Grid + Animations), Web Speech API

---

## File Structure

- `D:/cc_the_first/index.html` — the complete application (single file)

---

### Task 1: Create the HTML file with all structure, styling, and logic

**Files:**
- Create: `D:/cc_the_first/index.html`

- [ ] **Step 1: Write the complete HTML file**

The file includes:
1. **HTML structure**: header with title, card grid container, keyboard hint bar at bottom
2. **CSS styles**: responsive grid layout, card styling with frosted-glass effect, German flag color accents, key press animation, mobile-friendly
3. **JS logic**: letter data array with uppercase, lowercase, example word, Chinese translation; keyboard event listener mapping keys to letters; click handler on cards; SpeechSynthesis pronunciation with lang='de-DE'

Letter data (30 entries):
- A a Apfel 苹果 | B b Bär 熊 | C c Computer 电脑 | D d Dose 罐头 | E e Elefant 大象 | F f Fisch 鱼 | G g Gitarre 吉他 | H h Haus 房子 | I i Insel 岛屿 | J j Jacke 夹克 | K k Kaffee 咖啡 | L l Lampe 灯 | M m Maus 老鼠 | N n Nase 鼻子 | O o Ohr 耳朵 | P p Pilz 蘑菇 | Q q Quelle 源头 | R r Rose 玫瑰 | S s Sonne 太阳 | T t Tisch 桌子 | U u Uhr 钟 | V v Vogel 鸟 | W w Wasser 水 | X x Xylophon 木琴 | Y y Yoga 瑜伽 | Z z Zeit 时间 | Ä ä Ärger 生气 | Ö ö Öl 油 | Ü ü Über 超越 | ß Straße 街道

Keyboard mapping:
- a-z → A-Z (direct mapping)
- [ → Ä | ] → Ö | \ → Ü | - → ß

- [ ] **Step 2: Create the file**

Write the complete file to `D:/cc_the_first/index.html`.

- [ ] **Step 3: Test in browser**

Open `D:/cc_the_first/index.html` in a browser. Verify:
- All 30 letter cards render correctly
- Clicking a card triggers speech
- Pressing keyboard keys triggers speech for corresponding letter
- Special keys [ ] \ - work for Ä Ö Ü ß
- Responsive layout works at different screen widths
