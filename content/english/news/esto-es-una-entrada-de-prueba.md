---
title: Esto es una entrada de prueba
---
<!--StartFragment-->

# Markdown Crash Test

## Benchmarking the support of Markdown with a comprehensive checklist

**You're working on a project featuring Markdown?**

Drop [the source of this page](https://raw.githubusercontent.com/RoneoOrg/markdown/main/README.md) wherever you want to test *or showcase* the support of Markdown, and check that every single feature is properly rendered.

**Table of Contents**

* [Basic formatting](#basic-formatting)
* [Blockquotes](#blockquotes)
* [Lists](#lists)
* [Linebreaks](#linebreaks)
* [Links](#links)
* [Code formatting](#code-formatting)
* [Images](#images)
* [Task lists](#task-lists)
* [Tables](#tables)
* [Footnotes](#footnotes)
* [Definition List](#definition-list)
* [Headings](#headings)

## Basic formatting

### **Bold** text

**Syntax:**

```

```

**Output:**

You can mark some text as bold with **two asterisks** or **two underscores**.

### *Italic*

```

```

**Output:**

Use a *single asterisk* or a *single underscore* for italic.

### ***Bold and italic***

```

```

Three stars gives ***bold and italic***

### ~~Strikethrough~~

Using `~~two tildes~~` will strikethrough: ~~two tildes~~

## Blockquotes

**Syntax:**

```

```

**Output**:

> blockquote

### Nested blockquotes

**Syntax:**

```

```

**Output:**

> First level
>
> > Second level

### Markdown in blockquotes

```

```

**Output:**

> **Markdown** can be used *inside quotes*
>
> 1. This is the first list item.
> 2. This is the second list item.
>
> ~~strikethrough~~
>
> Here's some example code:
>
> ```
>
> ```

## Lists

### Unordered list

Cant be marked with `-`, `+` or `*`

```markdown

```

```markdown

```

```markdown

```

**Output:**

* First item
* Second item
* Third item
* First item
* Second item
* Third item
* First item
* Second item
* Third item

### Ordered lists

Incrementation is automatic, you can simply use `1.` everywhere

```

```

**Output:**

1. First item
2. Second item
3. Third item

### Nested list

```

```

**Output:**

* First item
* Second item
* Third item

  1. Indented item
  2. Indented item
* Fourth item

## Linebreaks

**When you hit enter just once** between two lines, both lines are joined into a single paragraph.

But, if you **leave a blank line between them**, they will split into two paragraphs.

**Demonstration**:

```

```

**Output:**

This text is a paragraph. This won't be another paragraph, it will join the line above it.

This will be another paragraph, as it has a blank line above it.

### Force line breaks

To force a line break, **end a line with two or more whitespaces**, and then type return.

```

```

**Output:**

This is the first line.\
Second line

### Horizontal lines

Can be inserted with four `*`, `-` or `_`

```

```

**Output:**

- - -

- - -

- - -

## Links

### Basic links

```

```

**Output:**

[Semantic description](https://roneo.org/markdown)\
[address@example.com](mailto:address@example.com)\
<https://roneo.org/markdown> works too. Must be used for explicit links.

### Links using text reference

```

```

**Output:**

[I'm a link](https://jamstack.club)

[This link](https://roneo.org/markdown) will do the same as well. It works as the identifier itself.

**Note:** The reference text is *not* case sensitive

### Link with a title on hover

```

```

**Output:**

[Random text](https://roneo.org/markdown "This example has a title"). Hover the mouse over it to see the title.

Several syntaxes are accepted: [One](https://eff.org "First site") [Two](https://jamstack.club "Second site") [Three](https://debian.org "Third site")

### Links with Markdown style

To ***emphasize*** links, add asterisks before and after the brackets and parentheses.

```

```

To denote links as `code`, add backticks *inside* the brackets:

```

```

**Output:**

I love supporting the **[EFF](https://eff.org)**.\
This is the *[Markdown Guide](https://www.markdownguide.org)*.\
See the section on [`code`](#code).

### Attribute a custom anchor to a heading

Anchors are automatically generated based on the heading's content. You can customize the anchor this way:

```

```

**Output:**

#### Heading {#custom-id}

## Code formatting

### Inline

Wrap with single backticks to highlight as`` `code` `` → `code`

### Codeblocks

Create a code block with three backticks ```` ``` ```` before and after your block of code.

**Output:**

```

```

Also possible with a tabulation or four empty spaces at the beginning of the lines:

**Tabulation**

```

```

**Four whitespaces**

```

```

Let's test the wrapping of a long line:

```

```

### Codeblocks with syntax highlighting

Set the language right after the first backticks (for example ```` ```html````) to get syntax highlighting

#### Samples:

#### HTML

```html

```

#### CSS

```css

```

#### Bash

```bash

```

#### Diff

```diff

```

### Escaping with backslashes

Any ASCII punctuation character may be escaped using a single backslash.

Example:

```

```

**Output:**

\*this is not italic\*

Markdown provides backslash escapes for the following characters:

```

```

## Images

### Basic syntax

```markdown

```

![Semantic description of the image](https://roneo.org/img/ok.png)

**Note: The text inside the square brackets is important!**

Screen reader users get informations about the image with this attribute called `ALT`, for *alternative text*.

Including **descriptive** alt text [helps maintain accessibility](https://webaim.org/techniques/alttext/) for every visitor and should always be included with an image. When you add alt text be sure to describe the content and function of the picture.\
In addition to the accessibility benefits, `ALT` is useful for SEO. It's also displayed when, for some reason, the picture is not loaded by the browser.

### Image with title and caption

```

```

![Semantic description](https://roneo.org/img/ok.png "Your title")*Your caption*

### Clickable images

For clickable images, simply wrap the image markup into a [link markup](#links):

```

```

**Output:**

[![Semantic description](https://roneo.org/img/ok.png "Your title")](http://jamstack.club)

### Image with an identifier

You can call the image with an identifier as we do for [links](#links)

```

```

![Semantic desc.](https://roneo.org/img/ok.png "Title")

## Task lists

```

```

**Output:**

* Write the press release
* Update the website

## Tables

```

```

or

```

```

will render the same way:

| Syntax    | Description |
| --------- | ----------- |
| Header    | Title       |
| Paragraph | Text        |

### Text alignment in tables

```

```

See the way the text is aligned, depending on the position of `':'`

| Syntax    | Description | Test Text   |
| --------- | ----------- | ----------- |
| Header    | Title       | Here's this |
| Paragraph | Text        | And more    |

## Footnotes

```

```

**Output:**

Here's a sentence with a footnote[^1].\
(see the result at the bottom of the page)

[^1]: This is the first footnote.

### Long footnote

```

```

**Output:**

Here's a longer one.[^bignote] (see the result at the bottom of the page)

[^bignote]: Here's one with multiple paragraphs and code. Indent paragraphs to include them in the footnote. `{ my code }` Note that you can place the footnote anywhere you want in your article

## Definition List

```

```

**Output:**

term : definition

second term : meaning

complex term : long definition including **bold text**. Velit tempor cillum aute culpa pariatur enim laboris consectetur tempor. Aute elit non do ipsum. Nisi quis culpa magna esse ipsum. Ad aliquip ullamco minim cillum in ullamco.

## Headings

Add `##` at the beginning of a line to set as Heading.\
You can use up to 6 `#` symbols for the corresponding Heading levels

```

```

## Heading 2

pedit quia voluptates atque nobis, perspiciatis deserunt perferendis, nostrum, voluptatem voluptas dolorem iure voluptatum? Accusantium a dolores dicta?Pariatur voluptates quam ut, cum aliquid eum, officiis laudantium totam suscipit, ducimus odit nobis! Corrupti, doloremque sed optio voluptatibus deserunt quas repellat eius minus quasi, ipsam unde esse sequi deleniti.

### Heading 3

pedit quia voluptates atque nobis, perspiciatis deserunt perferendis, nostrum, voluptatem voluptas dolorem iure voluptatum? Accusantium a dolores dicta?Pariatur voluptates quam ut, cum aliquid eum, officiis laudantium totam suscipit, ducimus odit nobis! Corrupti, doloremque sed optio voluptatibus deserunt quas repellat eius minus quasi, ipsam unde esse sequi deleniti.

#### Heading 4

pedit quia voluptates atque nobis, perspiciatis deserunt perferendis, nostrum, voluptatem voluptas dolorem iure voluptatum? Accusantium a dolores dicta?Pariatur voluptates quam ut, cum aliquid eum, officiis laudantium totam suscipit, ducimus odit nobis! Corrupti, doloremque sed optio voluptatibus deserunt quas repellat eius minus quasi, ipsam unde esse sequi deleniti.

##### Heading 5

pedit quia voluptates atque nobis, perspiciatis deserunt perferendis, nostrum, voluptatem voluptas dolorem iure voluptatum? Accusantium a dolores dicta?Pariatur voluptates quam ut, cum aliquid eum, officiis laudantium totam suscipit, ducimus odit nobis! Corrupti, doloremque sed optio voluptatibus deserunt quas repellat eius minus quasi, ipsam unde esse sequi deleniti.

###### Heading 6

pedit quia voluptates atque nobis, perspiciatis deserunt perferendis, nostrum, voluptatem voluptas dolorem iure voluptatum? Accusantium a dolores dicta?Pariatur voluptates quam ut, cum aliquid eum, officiis laudantium totam suscipit, ducimus odit nobis! Corrupti, doloremque sed optio voluptatibus deserunt quas repellat eius minus quasi, ipsam unde esse sequi deleniti.

## References

* Source of this page: [roneo.org/markdown](https://roneo.org/markdown)
* [Markdown Guide - Basic Syntax](https://www.markdownguide.org/basic-syntax)
* [Markdown Guide - Extended Syntax](https://www.markdownguide.org/extended-syntax)
* [Daring Fireball: Markdown Syntax Documentation](https://daringfireball.net/projects/markdown/syntax)
* [Markdown Guide at Gitlab.com](https://about.gitlab.com/handbook/markdown-guide/)
* [CommonMark Spec](https://spec.commonmark.org/0.29/)

## Related projects

* https://github.com/ericwbailey/markdown-test-file
* https://scottspence.com/posts/writing-with-markdown
* https://codingnconcepts.com/markdown/markdown-syntax/
* https://codeit.suntprogramator.dev/basic-markdown-syntax/
* https://daringfireball.net/projects/markdown/syntax.text

<!--EndFragment-->