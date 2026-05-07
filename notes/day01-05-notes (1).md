# 📚 HTML Study Notes — Day 01 to Day 05

> Personal notes from my 10-Day HTML Mastery Challenge  
> Source: Ali Hossain YouTube tutorials + W3Schools

---

## Day 01 — 🌐 What is HTML?

**HTML** stands for **HyperText Markup Language**.  
It is the standard language used to build the structure of every webpage on the internet.

- HTML is **not a programming language** — it is a **markup language**
- It uses tags to describe and organise content
- Every website uses HTML as its foundation. CSS adds design. JavaScript adds interaction.

> 💡 Think of HTML like the frame of a building — CSS is the paint, JavaScript is the electricity.

---

## Day 01 — 🏛️ HTML Structure

Every HTML file follows the same basic structure:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My First Webpage</title>
</head>
<body>
    <h1>Welcome to HTML</h1>
    <p>This is a paragraph.</p>
</body>
</html>
```

| Part | Description |
|------|-------------|
| `<!DOCTYPE html>` | Tells the browser this is an HTML5 document |
| `<html lang="en">` | Root element wrapping the entire page |
| `<head>` | Contains page info (not visible to user) |
| `<meta charset="UTF-8">` | Supports all characters and symbols |
| `<title>` | Text shown on the browser tab |
| `<body>` | Everything the user sees |

---

## Day 02 — 🏷️ Tags & Attributes

### Tags
HTML uses **tags** to mark up content. Most come in pairs:
```
<tagname> content here </tagname>
```

### Common Tags
```html
<h1>Heading</h1>
<p>Paragraph</p>
<a href="https://example.com">Link</a>
<img src="image.jpg" alt="Description">
<ul><li>List item</li></ul>
<ol><li>Ordered item</li></ol>
```

### Attributes
Attributes give extra information about elements. Always in the opening tag.

| Attribute | Used With | Purpose |
|-----------|-----------|---------|
| `href` | `<a>` | Link destination |
| `src` | `<img>` | Image path |
| `alt` | `<img>` | Alternative text for accessibility |
| `width` / `height` | `<img>` | Image size in pixels |
| `style` | Any tag | Inline CSS styling |
| `lang` | `<html>` | Page language |
| `title` | Any tag | Tooltip on hover |

**Best Practices:**
1. Always write attribute names in **lowercase**
2. Always wrap values in **double quotes**
3. Always include `alt` text for images

---

## Day 02 — 🛠️ VS Code + Live Server Setup

**Step 1** — Download VS Code from [code.visualstudio.com](https://code.visualstudio.com)

**Step 2** — Install Live Server Extension:
- Press `Ctrl + Shift + X`
- Search "Live Server" by Ritwick Dey → Install

**Step 3** — Run your file:
- Save file as `index.html`
- Type `!` + Enter for instant boilerplate
- Right-click → **Open with Live Server**
- Auto-refreshes on every `Ctrl + S`

**Emmet Shortcuts:**
| Shortcut | Result |
|----------|--------|
| `!` + Enter | Full HTML5 boilerplate |
| `lorem` + Enter | Full dummy paragraph |
| `lorem20` + Enter | Exactly 20 words of dummy text |

---

## Day 03 — 📝 Paragraphs, Line Breaks & Preformatted Text

### `<p>` — Paragraph Tag
- Defines a block of text
- Browser auto-adds margin before and after
- Extra spaces/line breaks in code are **collapsed** to a single space

### `<br>` — Line Break
- Starts a new line without a new paragraph
- Void/empty tag (no closing tag needed)

### `<hr>` — Horizontal Rule
- Creates a horizontal line to separate sections

### `<pre>` — Preformatted Text
- Displays text **exactly** as written in the code
- Preserves spaces and line breaks
- Uses fixed-width font (like Courier)
- Great for poems and code snippets

---

## Day 04 — 🎨 The Style Attribute & Google Fonts

### Inline CSS Syntax
```
<tagname style="property: value;">
```

### Common Style Properties
| Property | What it does |
|----------|-------------|
| `background-color` | Background color of element |
| `color` | Text color |
| `font-family` | Font type |
| `font-size` | Text size |
| `text-align` | Text alignment (left/center/right) |

Multiple styles separated by semicolon (`;`)

### Google Fonts — Quick Steps
1. Go to [fonts.google.com](https://fonts.google.com)
2. Select a font → copy the `<link>` tag
3. Paste inside `<head>` section
4. Use `font-family: 'FontName', sans-serif;` in style

```html
<head>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>
    <h1 style="font-family: 'Poppins', sans-serif;">Hello World!</h1>
</body>
```

---

## Day 05 — 🔡 Text Formatting Tags

| Tag | Purpose | Visual Result |
|-----|---------|--------------|
| `<b>` | Bold (visual only) | **Bold** |
| `<strong>` | Bold + semantic importance | **Bold** |
| `<i>` | Italic (visual only) | *Italic* |
| `<em>` | Italic + emphasis | *Italic* |
| `<mark>` | Highlighted text | `highlighted` |
| `<small>` | Smaller text | small text |
| `<del>` | Strikethrough | ~~deleted~~ |
| `<ins>` | Underline (inserted text) | underlined |
| `<sup>` | Superscript | x² |
| `<sub>` | Subscript | H₂O |

### When to use `<b>` vs `<strong>`?
- Use `<strong>` for text that is **semantically important** (SEO + screen readers)
- Use `<b>` only for visual boldness with no extra importance

### When to use `<i>` vs `<em>`?
- Use `<em>` when the emphasis **changes the meaning** of the sentence
- Use `<i>` for technical terms, titles, or thoughts (no stress emphasis)

---

*Notes by: My HTML 10-Day Mastery Challenge | May 2026*
