---
title: "Pandoc Demonstration Document"
author: "John Doe"
date: "2024"
toc: true
# classoption: landscape # format as landscape
---


# Introduction

This document demonstrates all available formatting options for PDF creation with Pandoc. It contains **bold text**, *italic text*, `inline code`, and various other formatting options.

## Text Formatting

### Basic Formatting

- **Bold text** with `**text**`
- *Italic text* with `*text*`
- ***Bold and italic*** with `***text***`
- `Inline code` with backticks
- ~~Strikethrough text~~ with `~~text~~`
- Superscript: H~2~O and E = mc^2^

### Lists

#### Unordered List

- First item
- Second item
  - Nested item
  - Another nested item
- Third item

#### Ordered List

1. First numbered item
2. Second numbered item
   a. Nested numbering
   b. Further nesting
3. Third numbered item

# Tables

## Simple Table

| Name | Age | City    |
|------|-----|---------|
| Anna | 25  | Berlin  |
| Hans | 32  | Munich  |
| Lisa | 28  | Hamburg |

## Extended Table with Alignment

| Left          | Centered     |      Right | Default      |
|:--------------|:------------:|-----------:|--------------|
| Left          |    Center    |      Right | Normal       |
| aligned       |   aligned    |    aligned | aligned      |

: Table with different alignments

# Images and Diagrams

## Local Image

![A sample image](images/example.jpg)

**Figure 1:** A sample image with detailed description of the displayed content, loaded from the local images folder.

## External Image

![Placeholder image](https://placehold.co/400x300/lightblue/white?text=External+Image)

# Code Blocks

## Python Code

```python
def fibonacci(n):
    """Calculates the nth Fibonacci number"""
    if n <= 1:
        return n
    else:
        return fibonacci(n-1) + fibonacci(n-2)

# Example call
for i in range(10):
    print(f"F({i}) = {fibonacci(i)}")
```

## Shell Script

```bash
#!/bin/bash
echo "Generating PDF document..."
pandoc note.md --defaults defaults.yaml -o output.pdf
echo "Done!"
```

# Mathematical Formulas

## Inline Mathematics

The formula for the area of a circle is $A = \pi r^2$, where $r$ is the radius.

## Display Mathematics

The Quadratic Formula:

$$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

Euler's Identity:

$$e^{i\pi} + 1 = 0$$

# Quotes and References

## Block Quote

> This is a longer quote that spans multiple lines and contains important information or wisdom from another person. Block quotes are frequently used to lend authority or additional context to a topic.
>
> --- Famous Person

## Nested Quote

> This is the first quote level.
>
> > This is a quote within a quote. It can be used for responses or comments.

# Footnotes and References

This is text with a footnote[^1]. Here is another footnote[^longnote].

[^1]: This is the first footnote.

[^longnote]: Here is a longer footnote with multiple paragraphs.

    Footnotes can contain multiple paragraphs. Subsequent paragraphs are indented to show that they belong to the previous footnote.

        { code }

    The entire paragraph can be indented, or just the first line. This way, multi-line footnotes are easier to write.

# Special Formatting

## Definition Lists

Term 1
:   Definition for Term 1

Term 2
:   Definition for Term 2
    With multiple lines

## Links

- [Internal link to heading](#tables)
- [External link](https://www.pandoc.org)
- [Link with title](https://pandoc.org "Pandoc Homepage")

## Horizontal Lines

Text before the line.

---

Text after the line.

# Smart Typography Extension

## Demonstration of Smart Extension Features

The smart extension automatically converts ASCII punctuation characters into typographically correct Unicode characters when generating output formats like HTML, LaTeX, and PDF.

### Smart Typography Examples

| Feature | Raw Input (Fenced) | Rendered Output |
|---------|-------------------|-----------------|
| **Smart Quotes** | `"Double quotes"` | "Double quotes" |
| | `'Single quotes'` | 'Single quotes' |
| | `It's smart about apostrophes` | It's smart about apostrophes |
| | `"Nested 'quotes' within quotes"` | "Nested 'quotes' within quotes" |
| **Smart Dashes** | `pages 10--20` | pages 10--20 |
| | `break in thought---like this` | break in thought---like this |
| | `state-of-the-art` | state-of-the-art |
| **Ellipses** | `three periods...` | three periods... |
| **Combined** | `"Well," she said, "years 1995--2005"` | "Well," she said, "years 1995--2005" |

### Complete Example Paragraph

**Raw Input:**
```
"Well," she said, "I think we need to consider the years 1995--2005 
as a turning point---though I'm not entirely sure... The question 
remains: what's the best approach?"
```

**Rendered Output:**

"Well," she said, "I think we need to consider the years 1995--2005 as a turning point---though I'm not entirely sure... The question remains: what's the best approach?"

# Summary

This document demonstrates the extensive formatting capabilities of Pandoc for PDF creation. From simple text to complex tables to mathematical formulas and code blocks - Pandoc provides all the necessary tools for professional document creation.

The syntax highlighting features enable clear presentation of code in various programming languages, while the mathematical functions support complex formulas and equations.
