# Markdown Reference Guide

This is a comprehensive guide to the most commonly used Markdown syntax.

---

## Headers

Headers are created using the `#` symbol. The number of `#` symbols corresponds to the header level.

```markdown
# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6
```

---

## Text Formatting

You can easily format text to be bold, italic, or have a strikethrough.

| Style         | Syntax                       | Example                       |
| ------------- | ---------------------------- | ----------------------------- |
| Bold          | `**text**` or `__text__`     | **This is bold text**         |
| Italic        | `*text*` or `_text_`         | *This is italic text*         |
| Strikethrough | `~~text~~`                   | ~~This is strikethrough~~     |
| Bold & Italic | `***text***` or `___text___` | ***This is bold and italic*** |

---

## Blockquotes

Blockquotes are used to indicate quoted text.

```markdown
> This is a blockquote.
>
> > This is a nested blockquote.
```

---

## Lists

### Unordered Lists

Use `*`, `+`, or `-` to create unordered lists.

```markdown
* Item 1
* Item 2
  * Nested Item 2a
  * Nested Item 2b
* Item 3
```

### Ordered Lists

Use numbers followed by a period.

```markdown
1. First item
2. Second item
3. Third item
   1. Nested item 3a
   2. Nested item 3b
```

---

## Code

### Inline Code

Wrap code with single backticks `` ` ``.

```markdown
This is an example of `inline code`.
```

### Fenced Code Blocks

Use triple backticks ` ``` ` to create a code block. You can also specify the language for syntax highlighting.

````markdown
```javascript
function greet() {
  console.log("Hello, world!");
}
```
````

---

## Links

Create links to navigate to other pages or websites.

```markdown
[Google](https://www.google.com "Link to Google")
```

---

## Images

The syntax for images is similar to links, but with a `!` at the beginning.

```markdown
![A placeholder image](https://placehold.co/600x400/EEE/31343C?text=Placeholder+Image "Placeholder Image")
```

---

## Horizontal Rule

Create a horizontal rule with three or more asterisks `***`, dashes `---`, or underscores `___`.

```markdown
***
---
___
```

---

## Tables

Tables are created using pipes `|` and hyphens `-`.

```markdown
| Header 1 | Header 2 | Header 3 |
| :------- | :------: | -------: |
| Align L  |  Center  |  Align R |
| Cell 4   |  Cell 5  |   Cell 6 |
```

---

## Task Lists

Create task lists (checkboxes) within a list.

```markdown
- [x] Completed task
- [ ] Incomplete task
- [ ] Another task
```

---

## Math and Equations (using LaTeX)

For mathematical and scientific notation, many Markdown renderers support LaTeX.

### Inline Math

Wrap your equation in single dollar signs `$` for inline math.

```markdown
The Pythagorean theorem is $a^2 + b^2 = c^2$.
```

### Block Equations

Wrap your equation in double dollar signs `$$` to display it as a centered block on its own line.

```markdown
The quadratic formula is:
$$x = \frac{-b \pm \sqrt{b^2-4ac}}{2a}$$
```

---

## Escaping Characters

To display a literal character that has special meaning in Markdown, use a backslash `\` before it.

```markdown
\*This is not italic.\*
