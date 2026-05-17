# 📚 Day 04 Notes — HTML Images & Favicons

> 10-Day HTML Mastery Challenge | May 2026

---

## 🖼️ What is the `<img>` Tag?

The `<img>` tag is used to **embed images** into a webpage.

- It is a **void tag** — no closing tag needed
- Images are not inserted into the page — they are **linked** from a source
- Two attributes are always required: `src` and `alt`

```html
<img src="image.jpg" alt="Description of image">
```

---

## 🔗 Key Attributes

| Attribute | Purpose |
|-----------|---------|
| `src` | Path to the image file (local or URL) |
| `alt` | Alternative text — shown if image fails to load (always include) |
| `width` | Image width in pixels |
| `height` | Image height in pixels |
| `style` | Inline CSS (width, height, border, etc.) |
| `title` | Tooltip text shown on hover |

> ⚠️ Always write `alt` text — it helps accessibility and improves SEO.

---

## 📂 Image File Paths

**Local image (same folder):**
```html
<img src="image.jpg" alt="Cat">
```

**Local image (subfolder):**
```html
<img src="images/photo.jpg" alt="Photo">
```

**External image (URL):**
```html
<img src="https://example.com/photo.jpg" alt="Online Photo">
```

---

## 🎬 Supported Image Formats

| Format | Extension | Best For |
|--------|-----------|---------|
| JPEG | `.jpg` / `.jpeg` | Photos, complex images |
| PNG | `.png` | Transparent backgrounds |
| GIF | `.gif` | Animations |
| SVG | `.svg` | Icons, logos (scalable) |
| WebP | `.webp` | Modern web (small file size) |

---

## ⭐ What is a Favicon?

A **favicon** is the small icon that appears on the **browser tab** next to the page title.

- Added inside `<head>` using a `<link>` tag
- Common formats: `.ico`, `.png`, `.jpg`
- Shows on browser tab, bookmarks, and shortcuts

```html
<head>
  <link rel="icon" href="image.jpg">
</head>
```

> 💡 Always add a favicon — it makes your site look professional.

---

## ✏️ Full Practice Code (My VS Code)

**image.html:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Image Tag in HTML</title>
  <link rel="stylesheet" href="image.css">
</head>
<body>

  <h1>Image Tag in HTML</h1>
  <img src="image.jpg" alt="Cat">
  <img src="happy-cat.gif" alt="Happy Cat">
  <img src="cat-computer.gif" alt="Cat at Computer">

</body>
</html>
```

**favicon.html:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Favicon in HTML</title>
  <link rel="icon" href="image.jpg">
</head>
<body>

  <h1>Favicon in HTML</h1>

</body>
</html>
```

---

*Day 04 complete ✅ | HTML Mastery 10-Day Challenge*
