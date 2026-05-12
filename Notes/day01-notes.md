# 📚 Day 01 Notes — HTML Structure, Tags & Attributes

> 10-Day HTML Mastery Challenge | May 2026

---

## 🌐 What is HTML?

**HTML** stands for **HyperText Markup Language**.
It is the standard language used to build the structure of every webpage.

- HTML is **not a programming language** — it is a **markup language**
- It uses tags to describe and organise content
- Every website is built on HTML. CSS adds design. JavaScript adds interaction.

> 💡 Think of HTML like the frame of a building — CSS is the paint, JavaScript is the electricity.

---

## 🏛️ HTML Document Structure

Every HTML file follows this basic structure:

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
| `<head>` | Contains page info — not visible to the user |
| `<meta charset="UTF-8">` | Supports all characters and symbols |
| `<title>` | Text shown on the browser tab |
| `<body>` | Everything the user sees on the page |

---

## 🏷️ Tags & Attributes

HTML uses **tags** to mark up content. Most tags come in pairs:

```html
<tagname>content here</tagname>
```

**Common tags practiced:**

```html
<h1>Main Heading</h1>
<h2>Sub Heading</h2>
<p>A paragraph of text</p>
<ul>
    <li>Unordered list item</li>
</ul>
<ol>
    <li>Ordered list item</li>
</ol>
```

**Attributes** give extra information about elements. They always go in the opening tag:

| Attribute | Used With | Purpose |
|-----------|-----------|---------|
| `href` | `<a>` | Link destination URL |
| `src` | `<img>` | Image file path |
| `alt` | `<img>` | Alternative text (accessibility) |
| `width` / `height` | `<img>` | Image size in pixels |
| `style` | Any tag | Inline CSS styling |
| `lang` | `<html>` | Sets the page language |
| `title` | Any tag | Tooltip text on hover |
| `target="_blank"` | `<a>` | Opens link in a new tab |

**Best Practices:**
1. Always write attribute names in **lowercase**
2. Always wrap attribute values in **double quotes**
3. Always include `alt` text on images

**Code practiced:**

```html
<h1 title="This is a tooltip — hover over me!">HTML Attributes Practice</h1>
<a href="https://www.w3schools.com">W3Schools Website</a>
<a href="https://www.google.com" target="_blank">Open Google in a new tab</a>
<img src="image.jpg" alt="A placeholder image" width="200" height="100">
<p style="color: blue;">This text is blue!</p>
```

---

## 📝 Paragraphs, Line Breaks & Preformatted Text

| Tag | Purpose |
|-----|---------|
| `<p>` | Block of text — browser adds margin before/after |
| `<br>` | Line break — new line without a new paragraph (void tag) |
| `<hr>` | Horizontal divider line to separate sections |
| `<pre>` | Preserves spaces and line breaks exactly as written |

> ⚠️ Extra spaces and line breaks inside `<p>` are **collapsed** to a single space by the browser.

**Code practiced:**

```html
<p>This is a standard paragraph. Even if I add
multiple    spaces    or
line breaks, the browser shows it as one line.</p>

<p>This paragraph<br>uses line breaks<br>to start new lines.</p>

<pre>
    The woods are lovely, dark and deep,
    But I have promises to keep,
    And miles to go before I sleep.
</pre>
```

---

## 🎨 Style Attribute & Google Fonts

**Inline CSS syntax:**

```
<tagname style="property: value;">
```

| Property | What it does |
|----------|-------------|
| `background-color` | Background color of an element |
| `color` | Text color |
| `font-family` | Font type |
| `font-size` | Text size (px, %, em) |
| `text-align` | `left`, `center`, or `right` |
| `padding` | Inner space around content |

Multiple styles are separated by a semicolon `;`

**Google Fonts — steps:**
1. Go to [fonts.google.com](https://fonts.google.com) → pick a font → copy the `<link>` tag
2. Paste inside `<head>`
3. Use `font-family: 'FontName', sans-serif;` in your style attribute

**Code practiced:**

```html
<head>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap" rel="stylesheet">
</head>

<body style="background-color: powderblue;">
    <h1 style="color: dodgerblue; text-align: center; font-family: 'Poppins', sans-serif;">
        Welcome to My Styled Page
    </h1>
    <p style="font-family: verdana; font-size: 160%; color: darkslategrey;">
        Custom font, larger size, specific color.
    </p>
    <div style="background-color: tomato; color: white; padding: 20px;">
        <p>Styled container using a div!</p>
    </div>
</body>
```

---

## 🔡 Text Formatting Tags

| Tag | Purpose | Result |
|-----|---------|--------|
| `<b>` | Bold — visual only | **Bold** |
| `<strong>` | Bold + semantic importance | **Important** |
| `<i>` | Italic — visual only | *Italic* |
| `<em>` | Italic + emphasis | *Emphasis* |
| `<mark>` | Highlighted text | highlighted |
| `<small>` | Smaller text | small |
| `<del>` | Strikethrough | ~~deleted~~ |
| `<ins>` | Underline (inserted text) | underlined |
| `<sup>` | Superscript | x² |
| `<sub>` | Subscript | H₂O |

**`<b>` vs `<strong>`** — Use `<strong>` for semantically important text (better for SEO + screen readers).

**`<i>` vs `<em>`** — Use `<em>` when emphasis changes meaning. Use `<i>` for terms, titles, or thoughts.

**Code practiced:**

```html
<p><b>Visual bold</b> vs <strong>Semantic bold</strong></p>
<p><i>Visual italic</i> vs <em>Semantic emphasis</em></p>
<p>Don't forget to <mark>study this part</mark>!</p>
<p>Was <del>$100</del>, now only <strong>$75!</strong></p>
<p><ins>New addition to the document.</ins></p>
<p>a<sup>2</sup> + b<sup>2</sup> = c<sup>2</sup></p>
<p>Water: H<sub>2</sub>O | Sulphuric Acid: H<sub>2</sub>SO<sub>4</sub></p>
```

---

## 🛠️ VS Code Setup

| Step | Action |
|------|--------|
| Install | Download from [code.visualstudio.com](https://code.visualstudio.com) |
| Extension | Install **Live Server** by Ritwick Dey (`Ctrl+Shift+X`) |
| Run | Right-click `.html` file → Open with Live Server |
| Auto-refresh | Saves and refreshes browser on every `Ctrl+S` |

**Emmet Shortcuts:**

| Shortcut | Result |
|----------|--------|
| `!` + Enter | Full HTML5 boilerplate instantly |
| `lorem` + Enter | Full dummy paragraph |
| `lorem20` + Enter | Exactly 20 words of dummy text |

---

*Day 01 complete ✅ | HTML Mastery 10-Day Challenge*
