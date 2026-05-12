# 📚 Day 03 Notes — CSS in HTML

> 10-Day HTML Mastery Challenge | May 2026

---

## 🎨 What is CSS?

**CSS** stands for **Cascading Style Sheets**.
It controls how HTML elements look — colors, fonts, sizes, spacing, layouts.

There are **3 ways** to add CSS to an HTML file:
1. **Inline CSS** — inside the element's `style` attribute
2. **Internal CSS** — inside a `<style>` block in `<head>`
3. **External CSS** — in a separate `.css` file linked to the HTML

---

## 1️⃣ Inline CSS

Written directly inside a tag using the `style` attribute.

```html
<p style="color: green; font-family: Arial, sans-serif; font-size: 18px;">
    This paragraph has inline styling.
</p>
```

**When to use:** Quick, one-off styling on a single element.

**Downside:** Hard to maintain — if you need to change a style, you have to update every single element.

---

## 2️⃣ Internal CSS

Written inside a `<style>` block in the `<head>` section. Applies styles to the whole page.

```html
<head>
    <style>
        pre {
            font-family: Impact;
            font-size: 18px;
            font-weight: 100;
        }
        q {
            background-color: aqua;
            font-size: 20px;
            font-family: 'Lucida Sans';
        }
    </style>
</head>
```

**When to use:** Single-page projects or when styles apply to only that one page.

**Downside:** Styles don't carry over to other pages — you'd have to copy-paste them.

---

## 3️⃣ External CSS

Styles are written in a separate `.css` file and linked to the HTML with a `<link>` tag.

**In your HTML file:**
```html
<head>
    <link rel="stylesheet" href="style.css">
</head>
```

**In your `style.css` file:**
```css
p {
    color: navy;
    font-size: 16px;
}
```

**When to use:** Always — for real projects. This is the **best practice**.

**Why it's the best:**
- One CSS file can style many HTML pages
- Clean separation of structure (HTML) and design (CSS)
- Easy to update — change one file, all pages update

---

## ⚖️ Comparison Table

| Method | Where it lives | Scope | Best For |
|--------|---------------|-------|---------|
| **Inline** | Inside the HTML tag | One element only | Quick single fixes |
| **Internal** | `<style>` in `<head>` | One page only | Single-page projects |
| **External** | Separate `.css` file | Entire website | All real projects ✅ |

> 💡 **Rule of thumb:** Always prefer External CSS for real projects. Keep HTML for structure, CSS for design — never mix them up more than needed.

---

## 🔁 CSS Priority (Cascade Order)

When the same element has styles from multiple sources, the browser follows this priority:

```
Inline CSS  >  Internal CSS  >  External CSS
```

The most specific style wins. Inline is highest priority because it's closest to the element.

---

## ✏️ Full Code Practiced

**HTML file (`Day03-CSS in html.html`):**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>CSS in HTML</title>

    <!-- Internal CSS -->
    <style>
        pre {
            font-family: Impact;
            font-size: 18px;
            font-weight: 100;
        }
        q {
            background-color: aqua;
            font-size: 20px;
        }
    </style>

    <!-- External CSS -->
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <h2>Inline CSS</h2>
    <p style="color: green; font-family: Arial, sans-serif; font-size: 18px;">
        This paragraph uses inline styling.
    </p>

    <hr>

    <h2>Internal CSS</h2>
    <pre>This text is styled with Internal CSS via the &lt;style&gt; block.</pre>
    <q>This quote has aqua background from Internal CSS.</q>

    <hr>

    <h2>External CSS — Best Practice for Production</h2>
    <p>This paragraph is styled by the external style.css file.</p>
</body>
</html>
```

**CSS file (`style.css`):**

```css
p {
    color: navy;
}
```

---

*Day 03 complete ✅ | HTML Mastery 10-Day Challenge*
