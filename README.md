# HTML + CSS + JS Assignment

A single-page site built with vanilla HTML, CSS, and JavaScript to practice core web fundamentals: page structure, layout without CSS, the box model, font sizing units, and CSS positioning.

**Live site:** 
[https://eleahburman.github.io/html-css-js-assignment/](https://eleahburman.github.io/html-css-js-assignment/)
---

## Structure

- `index.html` — all page markup
- `style.css` — all styling
- `script.js` — linked at the bottom of `<body>`, currently unused for this assignment but wired up and ready

---

## Section Breakdown

### 1. Page structure: navbar, header, sections, footer

A `<nav>` with a horizontal link list, a `<main>` containing one `<h1>` and four `<h2>` sections, and a `<footer>`.

**10 most useful HTML tags:**

1. `div` — generic block container, the backbone of layout
2. `span` — generic inline container, for styling text without breaking flow
3. `a` — links, navigation
4. `img` — images
5. `ul` / `li` — lists, navs, menus
6. `form` — collecting user input
7. `input` — form fields
8. `button` — clickable actions
9. `section` — grouping related content semantically
10. `nav` — semantic navigation landmark

### 2. SEO header tags

Researched which tags matter most for search engine optimization:

- `<title>` — most important on-page SEO signal; shown in search results and browser tab
- `<meta name="description">` — the snippet shown under the title in search results
- `<h1>` — one per page, describes the main topic
- `<h2>`–`<h6>` — hierarchical subheadings that help search engines parse page structure
- `<meta name="viewport">` — mobile-friendliness affects ranking
- `<link rel="canonical">` — avoids duplicate-content penalties
- `<img alt="...">` — supports accessibility and image search

### 3. 3×3 grid without CSS or tables

Built using only `div`s (block-level, stack vertically = rows) and `span`s (inline, flow horizontally = columns), spaced with `&nbsp;`. No CSS applied to this section on purpose.

### 4. Box model gallery

Three rows of `div`s inside `.box-row` flex containers, each row varying one box-model property across three columns:

- Row 1 — `border` (0px / 5px solid / 10px dashed)
- Row 2 — `margin` (0px / 5px / 10px)
- Row 3 — `padding` (0px / 5px / 10px)

### 5. Font sizes with inline styles

A `<ul>` where each `<li>` uses a different CSS length unit via inline `style`, with a one-line explanation of when to use it:

- `px` — fixed size, precise control (e.g. icon labels)
- `em` — relative to parent, good for nested elements that scale together
- `rem` — relative to root, consistent sizing site-wide
- `%` — relative to parent, responsive text
- `vw` — relative to viewport width, scales with screen size (e.g. hero text)
- keyword (`large`) — browser-defined absolute size, simple default

### 6. Positioning + sticky footer

A demo box showing all four positioning options:

- `static` — default document flow
- `relative` — shifted from its normal spot, original space preserved
- `absolute` — removed from flow, positioned against nearest positioned ancestor
- `fixed` — stays fixed in the viewport regardless of scroll

The footer is pinned to the bottom of the screen using a flex layout on `html`/`body` (`min-height: 100vh`, `flex: 1` on `main`) rather than positioning — this keeps it at the bottom of the *page* rather than fixed to the *viewport*, so it doesn't overlap content on short pages.

---

## How to Run Locally

Open `index.html` with the **Live Server** VS Code extension, or open the file directly in a browser.