# Markdown Tutorial — OIM 7502, Module 3

This file is written in Markdown, which means the raw text you'd see if you
opened this in a plain text editor and the *rendered* version you're looking
at right now (if your viewer renders `.md` files) are two different things.
That gap — plain text in, formatted output out — is the entire idea.

Markdown is what powers formatted text in Jupyter notebook cells, GitHub
READMEs, Slack messages, and a good chunk of the documentation you'll read
for the rest of your career. Learn it once, use it everywhere.

**How to use this tutorial:** This file is a quick reference — read a section, look at the raw syntax next to its rendered output. For hands-on practice actually writing and rendering each element yourself, use the companion notebook, `markdown_tutorial.ipynb`, which walks through the same material with practice cells built in.

---

## 1. Headers

Headers use `#` symbols. The number of `#` characters sets the level —
one `#` is the biggest, six is the smallest.

```
# Header 1
## Header 2
### Header 3
```

**Renders as:**

# Header 1
## Header 2
### Header 3

Use headers to organize a notebook the way you'd organize a report — one
`#` for the notebook's title, `##` for major sections, `###` for
subsections. Don't skip levels (going straight from `#` to `###`) — it
reads fine to you, but it breaks anyone using an outline or screen reader
to navigate.

---

## 2. Emphasis (bold, italic, etc.)

```
*italic text* or _italic text_
**bold text** or __bold text__
***bold and italic***
~~strikethrough~~
```

**Renders as:**

*italic text*
**bold text**
***bold and italic***
~~strikethrough~~

---

## 3. Lists

**Unordered** (use `-`, `*`, or `+` — pick one and stay consistent):

```
- First item
- Second item
  - Nested item
- Third item
```

- First item
- Second item
  - Nested item
- Third item

**Ordered:**

```
1. First step
2. Second step
3. Third step
```

1. First step
2. Second step
3. Third step

---

## 4. Links and Images

```
[link text](https://example.com)
![alt text](path/to/image.png)
```

The only difference between a link and an image is the `!` in front.
That's it. That's the whole trick.

---

## 5. Code

**Inline code** uses single backticks: `` `like this` `` renders as
`like this`.

**Code blocks** use triple backticks, optionally with a language name for
syntax highlighting:

````
```python
import pandas as pd
df = pd.read_csv("data.csv")
```
````

```python
import pandas as pd
df = pd.read_csv("data.csv")
```

This is the block you'll use constantly when your markdown cells need to
reference a variable, function, or snippet of code without actually
running it.

---

## 6. Blockquotes

```
> This is a blockquote.
> It can span multiple lines.
```

> This is a blockquote.
> It can span multiple lines.

Useful for calling out a quote, a warning, or a note you want visually
separated from the surrounding text.

---

## 7. Tables

```
| Column A | Column B | Column C |
|----------|----------|----------|
| 1        | 2        | 3        |
| 4        | 5        | 6        |
```

| Column A | Column B | Column C |
|----------|----------|----------|
| 1        | 2        | 3        |
| 4        | 5        | 6        |

The dashes in the second row are what tell Markdown "this is a table
header" — they need at least three dashes per column, but the columns
don't have to line up neatly in the raw text. Readability is a courtesy
to your future self, not a requirement.

---

## 8. Horizontal Rules

Three or more dashes, asterisks, or underscores on their own line:

```
---
```

Useful for visually separating sections — this whole tutorial uses them.

---

## 9. Line Breaks (the one that trips everyone up)

A single line break in your raw markdown is **ignored** when rendered —
this paragraph
looks like one line in the source
but renders as a single block.

To force a line break, either end a line with two trailing spaces, or
leave a fully blank line between paragraphs to start a new paragraph.
This is the single most common markdown frustration — plan for it.

---

## Practice

The checklist of things to practice — headers, emphasis, lists, links, code
blocks, tables, blockquotes, and more — lives in the companion notebook,
`markdown_tutorial.ipynb`. Use this document as your reference while you
work through it there.
