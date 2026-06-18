---
layout: post
title: "Template"
date: 2026-06-18
tag: test
excerpt: "A comprehensive testing template for Jekyll and Liquid syntax structures."
published: true
---
## 1. Text Layouts & Typography

You can write normal body text here. To wrap text to a new line within the same paragraph, leave two spaces at the end of a line.  
Like this. Or press `Enter` twice to create an entirely new paragraph block.

* **Bold Text**: Use `**strong**` or `__strong__` to make text **bold**.
* *Italic Text*: Use `*emphasis*` or `_emphasis_` to make text *italic*.
* ***Combined***: Use `***three asterisks***` for ***bold and italic*** text.
* ~~Strikethrough~~: Use `~~two tildes~~` to create a ~~strikethrough~~ effect.

---

## 2. Headings (SEO Structure)

# Heading Level 1 (Usually reserved for Post Title)
## Heading Level 2 (Main Sections)
### Heading Level 3 (Sub-sections)
#### Heading Level 4 (Minor Sub-sections)
##### Heading Level 5
###### Heading Level 6

---

## 3. Lists

### Unordered (Bullet Points)
* Main bullet point item
* Another main bullet point item
  * Indented sub-bullet (Press Spacebar 2 or 4 times)
  * Second indented sub-bullet
* Back to the main list

### Ordered (Numbered Lists)
1. First chronological step
2. Second chronological step
   1. Sub-step under step two
   2. Another sub-step
3. Third chronological step

### Task Checkboxes (GitHub Flavored Markdown)
- [x] This task is marked as finished
- [ ] This task is still pending or incomplete
- [ ] Another pending item

---

## 4. Blockquotes

Use the greater-than symbol `>` to highlight callouts, quotes, or important notes.

> "This is a single-line blockquote container. It helps break up long text blocks and draws the reader's eye to important quotes."

> Multi-line blockquotes work too.
> 
> > You can even nest blockquotes inside other blockquotes by doubling the symbol.

---

## 5. Fenced Code Blocks & Inline Code

### Inline Code
To reference a file path, variable, or quick command like `git status` inside a regular sentence, wrap it in single backticks.

### Syntax Highlighted Code Blocks
Jekyll natively supports automatic syntax highlighting for almost any programming language using triple backticks.

```html
<!DOCTYPE html>
<html>
<head>
  <title>Jekyll Blog Page</title>
</head>
<body>
  <h1>Hello World</h1>
</body>
</html>
```

```markdown
# This is meta-markdown text
Check out [this link](https://github.com).
```

---

## 6. Links and Embedded Media

### Links
* **Direct Link**: [Visit Google](https://google.com)
* **Link with Hover Text**: [Visit GitHub Pages](https://github.com "GitHub Pages Help")
* **Raw URL**: <https://jekyllrb.com>

### Images
To insert images safely, make sure the asset path points correctly to your site files.

![Alternative Text Descriptions](/assets/images/blog-placeholder.jpg "Optional image title caption")

---

## 7. Tables

Jekyll supports markdown tables out of the box. Use colons `:` to align text within the columns.

| Column Item | Alignment Rule | Status Option |
| :--- | :---: | ---: |
| Left-Aligned text | Centered text | Right-Aligned text |
| Row Item A | Row Item B | Row Item C |
| Next Data | Next Data | Next Data |

---

## 8. Miscellaneous Utilities

### Horizontal Divider Lines
You can create clean separating break lines using three hyphens, asterisks, or underscores.

---

***

### Escaping Formatting Characters
If you want to type literal formatting characters (like an asterisk or a hashtag) without triggering Markdown rules, add a backslash `\` directly before the character.

\*This text is surrounded by literal asterisks and will not render in italics\*

### Basic HTML Elements
Jekyll safely processes basic standard HTML inside your markdown posts if you need deeper styling control.

You can use keyboard styles like <kbd>Ctrl</kbd> + <kbd>V</kbd>, or change text properties manually using a <span style="color: blue; font-weight: bold;">custom styled inline HTML span tag</span>.

