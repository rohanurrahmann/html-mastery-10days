# 📅 Day 05 — JavaScript Integration & HTML Links

**10-Day HTML Mastery Challenge**
**Instructor:** Ali Hossain | **Student:** Rohanur Rahman

---

## 📚 Topics Covered

### 1. JavaScript in HTML — Three Methods

| Method | Where | Best For |
|---|---|---|
| **Inline JS** | Inside HTML attribute (`onclick`) | Quick one-liners |
| **Internal JS** | `<script>` tag in same file | Small single-page projects |
| **External JS** | Separate `.js` file via `src=""` | ✅ Professional projects |

---

### 2. HTML Links — Anchor Tag `<a>`

| Feature | Syntax | Purpose |
|---|---|---|
| Basic Link | `<a href="url">` | Navigate to a URL |
| Internal Page | `<a href="page.html">` | Navigate within the site |
| New Tab | `target="_blank"` | Open link in a new tab |
| Image as Link | Wrap `<img>` inside `<a>` | Clickable image |
| Email Link | `href="mailto:email"` | Open email client |

---

## 📁 File Structure

```
Day05/
├── javascript.html     → JS integration demo (inline, internal, external)
├── app.js              → External JS file
├── link.html           → HTML links demo (all types)
├── home.html           → Internal navigation target
├── about.html          → Internal navigation target
├── contact.html        → Internal navigation target
├── blog.html           → Internal navigation target
├── menu.html           → Internal navigation target
├── img.jpeg            → Image used in image-link demo
└── README.md           → This file
```

---

## 💡 Key Concepts

**Block vs Inline Elements:**
- **Block elements** (`<div>`, `<p>`, `<h1>`) — take full width, start on a new line
- **Inline elements** (`<a>`, `<span>`) — flow with surrounding content

**Link Target Values:**
- `_self` — opens in the same tab (default)
- `_blank` — opens in a new tab

**`mailto:` links** trigger the user's default email application automatically.

---

## 🔗 Resources

- [Full Challenge Repo](https://github.com/rohanurrahmann/html-mastery-10days)
- [LinkedIn Progress](https://www.linkedin.com/in/rohanurrahman/)
