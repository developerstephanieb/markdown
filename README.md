# Markdown Reference

A comprehensive guide to the most commonly used Markdown syntax.

---

## Table of Contents

[Headers](#headers)  
[Text Formatting](#text-formatting)   
[Lists](#lists)   
[Blockquotes](#blockquotes)   
[Horizontal Line](#horizontal-line)   
[Links](#links)   
[Images](#images)   
[Code](#code)   
[Tables](#tables)   
[Linking to Headers](#linking-to-headers)   
[Escaping Characters](#escaping-characters)   
[Footnotes](#footnotes)   
[Using LaTeX (Math)](#using-latex-math)   
[Using HTML (Comments)](#using-html-comments)   

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

Text can be formatted to be bold, italic, or have a strikethrough.

| Style         | Syntax                       | Example                       |
| ------------- | ---------------------------- | ----------------------------- |
| Bold          | `**text**` or `__text__`     | **This is bold text**         |
| Italic        | `*text*` or `_text_`         | *This is italic text*         |
| Strikethrough | `~~text~~`                   | ~~This is strikethrough~~     |
| Bold & Italic | `***text***` or `___text___` | ***This is bold and italic*** |

---

## Lists

Lists can be unordered, ordered, or task-based, and items can be nested by indenting.

```markdown
Use `*`, `+`, or `-` to create ordered lists:
* Item 1
+ Item 2
  - Nested Item 2a
  * Nested Item 2b
+ Item 3

Use numbers followed by a period to create ordered lists:
1. First item
2. Second item
3. Third item  
   1. Nested item 3a  
   2. Nested item 3b

Use `-[ ]` to create a checkbox and add an `x` inside to mark a task as complete:
- [x] Completed task
- [ ] Incomplete task
- [ ] Another task
```

Use `*`, `+`, or `-` to create unordered lists:
* Item 1
+ Item 2
  - Nested Item 2a
  * Nested Item 2b
+ Item 3

Use numbers followed by a period to create ordered lists:
1. First item
2. Second item
3. Third item  
   1. Nested item 3a  
   2. Nested item 3b

Use `-[ ]` to create a checkbox and add an `x` inside to mark a task as complete:
- [x] Completed task
- [ ] Incomplete task
- [ ] Another task

---

## Blockquotes

Blockquotes are used to indicate quoted text.

```markdown
> This is a blockquote.
>
> > This is a nested blockquote.
```

> This is a blockquote.
>
> > This is a nested blockquote.

---

## Horizontal Line

Create a horizontal rule with three or more asterisks `***`, dashes `---`, or underscores `___`.

---

## Links

Create links to navigate to other pages or external websites using either inline or reference-style formatting.

```markdown
This is an inline link to [Google](https://www.google.com "Visit Google").

This is a reference-style link to [Wikipedia][wiki].

[wiki]: https://www.wikipedia.org "Visit Wikipedia"
```

This is an inline link to [Google](https://www.google.com "Visit Google").

This is a reference-style link to [Wikipedia][wiki].

[wiki]: https://www.wikipedia.org "Visit Wikipedia"

---

## Images

The syntax for images is similar to links, but with a `!` at the beginning.

```markdown
This is an inline image:  
![Inline placeholder](https://placehold.co/400x200/EEE/31343C?text=Inline+Image "Inline Placeholder")

This is a reference-style image:  
![Reference placeholder][img-ref]

[img-ref]: https://placehold.co/400x200/EEE/31343C?text=Reference+Image "Reference Placeholder"
```
 
This is an inline image:  
![Inline placeholder](https://placehold.co/400x200/EEE/31343C?text=Inline+Image "Inline Placeholder")

This is a reference-style image:  
![Reference placeholder][img-ref]

[img-ref]: https://placehold.co/400x200/EEE/31343C?text=Reference+Image "Reference Placeholder"

---

## Code

Use single backticks `` ` `` for inline code, or triple backticks ` ``` ` to create fenced code blocks with optional language syntax highlighting.


````markdown
This is `inline code` inside a sentence.

Here is a fenced code block with JavaScript syntax highlighting:
```javascript
function greet() {
  console.log("Hello, world!");
}
```
````

This is `inline code` inside a sentence.

Here is a fenced code block with JavaScript syntax highlighting:
```javascript
function greet() {
  console.log("Hello, world!");
}
```

---

## Tables

Tables use pipes `|` to separate columns, with hyphens `-` and colons `:` to define headers and set alignment.

```markdown
| Header 1 | Header 2 | Header 3 |
| :------- | :------: | -------: |
| Align L  |  Center  |  Align R |
| Cell 4   |  Cell 5  |   Cell 6 |
```

| Header 1 | Header 2 | Header 3 |
| :------- | :------: | -------: |
| Align L  |  Center  |  Align R |
| Cell 4   |  Cell 5  |   Cell 6 |

---

## Linking to Headers

Use internal links to jump to specific headers within the same document.

```markdown
- [Jump to the next section](#escaping-characters)
- [Jump to the first section](#headers)
```

- [Jump to the next section](#escaping-characters)
- [Jump to the first section](#headers)

---

## Escaping Characters

To display a literal character that has special meaning in Markdown, use a backslash `\` before it.

```markdown
\*This is not italic.\*
```

\*This is not italic.\*

---

## Footnotes

Use `[^label]` in the text and defined elsewhere in the document using `[^label]:`.

```markdown
Here is a statement with a footnote.[^1]

[^1]: This is the footnote text.
```

Here is a statement with a footnote.[^1]

[^1]: This is the footnote text.

---

## Using LaTeX (Math)

LaTeX syntax is often supported in Markdown for mathematical expressions, using single dollar signs `$` for inline math and double dollar signs `$$` for block equations.

```markdown
Inline: The Pythagorean theorem is $a^2 + b^2 = c^2$.

Block:
$$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$
```

Inline: The Pythagorean theorem is $a^2 + b^2 = c^2$.

Block:
$$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

---

## Using HTML (Comments)

Use raw HTML for features Markdown doesn't support, like comments and collapsible sections.

```html
<!-- This is a comment -->

<details>
  <summary>Click to expand!</summary>
  
  This content is hidden by default but is revealed when you click the summary text.
  You can even include **Markdown** `inside` HTML.
</details>
```

<details>
  <summary>Click to expand!</summary>
  
  This content is hidden by default but is revealed when you click the summary text.
  You can even include **Markdown** `inside` HTML.
</details>
