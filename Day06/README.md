# Day 06 – HTML Mastery 10-Day Challenge

**Topic:** Block vs Inline Elements · CSS Classes & IDs · Lists · Tables

---

## 📁 Files in This Folder

| File | What I Practiced |
|---|---|
| `block_and_inline_elements.html` + `elements.css` | Block vs inline elements with visual border demo |
| `id_and_class.html` + `style.css` | CSS class (reusable) vs id (unique) targeting |
| `list.html` + `list.css` | Unordered, ordered, and nav lists |
| `table.html` | Horizontal and vertical HTML tables |

---

## ✅ Key Concepts Learned

### Block vs Inline Elements
- **Block elements** start on a new line and take full width: `<h1>`, `<p>`, `<div>`, `<ul>`, etc.
- **Inline elements** sit inside a line and take only the space they need: `<strong>`, `<a>`, `<span>`, `<img>`, etc.
- **Rule:** Always nest inline elements *inside* block elements — never the other way around.

### CSS Class vs ID
- **Class** (`.className`) — can be used on multiple elements. One element can also have multiple classes: `class="two title"`
- **ID** (`#idName`) — must be unique. Only one element per page should have a given id.
- IDs have *higher specificity* than classes in CSS, so `#four` overrides `.two` if both apply.

### HTML Lists
- `<ul>` — unordered (bulleted) list. Use `list-style-type: none` to remove bullets (great for nav menus).
- `<ol>` — ordered (numbered) list. Use the `type` attribute to change numbering: `1`, `A`, `a`, `I`, `i`.
- `<li>` — list item, used inside both `<ul>` and `<ol>`.

### HTML Tables
- `<table>` → `<tr>` (row) → `<th>` (header cell) or `<td>` (data cell)
- **Horizontal table:** headers in the first row → data below
- **Vertical table:** headers in the first column → data to the right
- CSS: `border-collapse: collapse` removes the double border between cells.

---

## 🐛 Bugs Fixed During Refinement

| File | Bug | Fix |
|---|---|---|
| `list.html` | CSS file linked as `list.csss` | Fixed to `list.css` |
| `list.html` | Missing `</li>` closing tag on JavaScript item | Added closing tag |
| `style.css` | `font-color` is not a valid CSS property | Changed to `color` |
| `style.css` | `border: 1px color #1fd9fa` — invalid syntax | Removed invalid rule |
| `table.html` | "Adress" typo in table header | Fixed to "Address" |
| `table.html` | "Verticle" typo in heading | Fixed to "Vertical" |

---

## 📅 Challenge Progress

| Day | Topic | Status |
|---|---|---|
| Day 01 | HTML Structure & Basic Tags | ✅ Done |
| Day 02 | Text Formatting & Links | ✅ Done |
| Day 03 | Images & Media | ✅ Done |
| Day 04 | Forms & Input | ✅ Done |
| Day 05 | JavaScript Integration & Links | ✅ Done |
| **Day 06** | **Block/Inline · Class/ID · Lists · Tables** | ✅ Done |
| Day 07 | | ⏳ Coming |
| Day 08 | | ⏳ Coming |
| Day 09 | | ⏳ Coming |
| Day 10 | | ⏳ Coming |

---

*Following along with Ali Hossain's HTML tutorial series.*
