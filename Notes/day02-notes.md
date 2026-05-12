# 📚 Day 02 Notes — HTML Quotations, Citations & Comments

> 10-Day HTML Mastery Challenge | May 2026

---

## 💬 Quotation Tags

HTML has specific tags for quoting content from other sources.

### `<blockquote>` — Long Block Quote

Used for a longer quote taken from an external source. The browser usually indents it automatically.

```html
<blockquote>
    "Be yourself; everyone else is already taken."
    <strong>— Oscar Wilde</strong>
</blockquote>
```

### `<q>` — Short Inline Quote

Used for a short quotation inside a sentence. The browser automatically adds quotation marks around it.

```html
<p><q>Two things are infinite: the universe and human stupidity. — Albert Einstein</q></p>
```

**Key difference:**
- `<blockquote>` → long quote, displayed as its own block
- `<q>` → short quote, sits inline inside a paragraph

---

## 🔤 `<abbr>` — Abbreviation Tag

Used to mark abbreviations or acronyms. Add the full meaning in the `title` attribute — it appears as a tooltip on hover.

```html
<p><abbr title="HyperText Markup Language">HTML</abbr> is not a programming language.</p>
```

> 💡 Always use `<abbr>` with a `title` for accessibility and clarity.

---

## 📍 `<address>` — Address Tag

Used to define contact information for the author or owner of a page. Browsers typically display it in italic.

```html
<address>Puthia, Rajshahi, Bangladesh</address>
```

Can also hold email, phone, or links — anything that counts as contact info.

---

## 📖 `<cite>` — Creative Work Tag

Used to reference the title of a creative work — a book, film, article, painting, etc. Renders in italic by default.

```html
<p>Rajshahi is very famous for <cite>Mango</cite>.</p>
```

> ⚠️ `<cite>` is for **titles of works**, not for naming a person. Don't confuse it with quoting someone.

---

## 💭 HTML Comments

Comments are invisible to visitors — they only appear in the source code. Used to leave notes for yourself or other developers.

```html
<!-- This is a comment — the browser ignores this -->
<p>This paragraph is visible to visitors.</p>
```

**Use cases:**
- Leave notes explaining your code
- Temporarily hide a section without deleting it
- Mark sections in long HTML files

---

## 📋 All Tags at a Glance

| Tag | Purpose | Renders As |
|-----|---------|------------|
| `<blockquote>` | Long external quote | Indented block |
| `<q>` | Short inline quote | Inline with auto quotation marks |
| `<abbr>` | Abbreviation with full form in `title` | Underlined + tooltip on hover |
| `<address>` | Contact information | Italic block |
| `<cite>` | Title of a creative work | Italic |
| `<!-- -->` | Developer comment | Invisible to visitors |

---

## ✏️ Full Code Practiced

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Day 02 — Quotations & Citations</title>
</head>
<body>

    <h1>Quotation and Comments</h1>

    <!-- Block Quote -->
    <blockquote>
        "Be yourself; everyone else is already taken."
        <strong>— Oscar Wilde</strong>
    </blockquote>

    <!-- Inline Quote -->
    <p><q>Two things are infinite: the universe and human stupidity. — Albert Einstein</q></p>

    <!-- Abbreviation -->
    <p><abbr title="HyperText Markup Language">HTML</abbr> is not a programming language.</p>

    <!-- Address -->
    <address>Puthia, Rajshahi, Bangladesh</address>

    <!-- Cite -->
    <p>Rajshahi is very famous for <cite>Mango</cite>.</p>

    <!-- Comment -->
    <!-- This is a comment — visitors cannot see this -->
    <p>Comments are invisible to visitors.</p>

</body>
</html>
```

---

*Day 02 complete ✅ | HTML Mastery 10-Day Challenge*
