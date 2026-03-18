# Arabic Article Generation Prompt

Write a single **Arabic** article about the given topic in a style that is both **educational and enjoyable to read**.

The goal is **edutainment**:
- teach the reader clearly
- keep the article interesting
- avoid dry academic writing
- avoid overly complex page design

## Input

- `topic`: the topic of the article

## Main Goal

Create one self-contained HTML article file:

- `./content/<slug>.html`

Then update:

- `./index.html`

## Very Important

Do **not** try to make the page overly sophisticated.

Avoid:
- crowded layouts
- too many effects
- too many cards
- too many decorative elements
- complex visual systems
- trying to impress with design alone

Aim for:
- simple layout
- clear hierarchy
- good spacing
- readable sections
- a few interesting visual moments

The page should feel **clean, smart, and pleasant**, not busy.

## Language

- Write the article in **Arabic**
- Keep technical terms and proper nouns in **English** when needed
- Use `<html lang="ar" dir="rtl">`

## Writing Style

Write in **Arabic edutainment style**.

That means:
- clear and simple language
- interesting and lively tone
- easy explanations
- strong flow from one section to the next
- teach without sounding like a textbook

The article should feel like:
- a smart magazine piece
- an enjoyable explainer
- something a curious reader wants to continue reading

Avoid:
- academic stiffness
- long dense paragraphs
- too much jargon
- jumping too quickly into formal details

## Content Structure

The article should usually follow this flow:

1. **Interesting opening**
   - start with a question, problem, surprising fact, or vivid example

2. **What is it?**
   - explain the basic idea simply

3. **Why does it matter?**
   - show why the topic is useful, important, or fascinating

4. **Build understanding step by step**
   - move from intuition to deeper explanation
   - use examples and analogies

5. **Show it visually**
   - include a figure, simple diagram, illustration, or visual explanation where helpful

6. **Go a bit deeper**
   - include technical detail only after the reader understands the idea

7. **Wrap up well**
   - end with a clear summary and memorable takeaway

This structure is a guide, not a strict template.

## Colors

The site uses a **black and white** palette only.

- Background: white (`#ffffff`)
- Text: black/near-black (`#111111`)
- Muted text: gray (`#555555`)
- Borders: light gray (`#e0e0e0`)
- No accent colors, no brand colors, no colored backgrounds

Keep everything monochrome. Use weight, size, and spacing for emphasis — not color.

## Fonts

The default body font is **Noto Naskh Arabic** (a Naskh-style Arabic serif font).

Rules:
- All body text, paragraphs, metadata, and UI text **must** use Noto Naskh Arabic
- You **may** pick a different interesting font for **headlines or one decorative section** if it fits the article's personality — but this is optional, not required
- If you use a special font, load it from Google Fonts CDN
- Never use more than two fonts total in one article
- The special font should complement Naskh, not clash with it

## Design Guidance

Keep the layout **simple**.

Use:
- clean sections
- clear headings
- good whitespace
- readable typography
- one or two strong visual ideas

Do not force a fancy layout.
Do not make every section visually heavy.

A good page can be:
- mostly clean text sections
- with a few highlighted visual sections
- with one or two interactive moments
- with a diagram, figure, chart, or comparison block where useful

## Visuals and Interactivity

Include **some** visuals and interactivity, but keep them light.

Good options:
- a simple inline SVG diagram
- a small timeline
- a comparison figure
- a simple chart
- a highlighted explainer box
- an expandable section
- a hover effect
- a copy button for code
- a small interactive demo if relevant

Use visuals to **explain**, not just decorate.

You do **not** need many interactive elements.
One or two good ones are enough.

## Uniqueness

Do not copy the exact structure or style of other articles in the project.

Each article should feel fresh, but still simple.

That does **not** mean making it complicated.
It means choosing a fitting presentation for the topic.

## Research

Before writing, search the web for strong sources.

Prefer:
- official documentation
- papers
- original blog posts
- reputable technical articles
- quality talks or interviews

Check key facts before writing.

## Links and References

Add links naturally inside the article when referencing outside material.

Use normal HTML links like:

`<a href="URL">text</a>`

At the end, include a section titled:

## المصادر والمراجع

Include 5 to 10 useful sources.
For each source, add:
- linked title
- short Arabic note explaining why it is useful

## Code and Examples

If code helps explain the topic:
- include real code snippets
- explain them simply
- keep them readable

Do not include code just for show.

## HTML Rules

The article must be a **single standalone HTML file**.

Requirements:
- all CSS inside the file
- all JavaScript inside the file
- no build step
- no frameworks
- no extra local files
- CDN libraries are allowed if truly useful

## Basic HTML Shape

```html
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Article Title</title>
  <meta name="description" content="وصف عربي للمقال">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Noto+Naskh+Arabic:wght@400;500;600;700&display=swap" rel="stylesheet">
  <style>
    /* black and white palette, Noto Naskh Arabic as base font */
    /* all CSS here */
  </style>
</head>
<body>
  <!-- article content -->
  <script>
    /* all JS here */
  </script>
</body>
</html>
```

## Index Page

After creating the article, update `./index.html`.

If it does not exist, create it.

The index page should:
- be in Arabic
- use `lang="ar"` and `dir="rtl"`
- list articles clearly
- link to `./content/<slug>.html`
- use a simple and clean card or list layout

Each article entry should include:
- title
- short description
- author
- date

## Author

Clearly show the author in the article using the model name and version.

Do not use generic labels like "AI" or "LLM".

## Final Check

Before finishing, make sure:

- the article is in Arabic
- the tone is edutainment, not textbook-like
- the explanation is simple and clear
- the layout is simple, not crowded
- there are some useful visuals or interactive elements
- the visuals help understanding
- the page is self-contained
- the article feels interesting to read

## Summary

Write a **clear Arabic edutainment article** with:
- simple language
- enjoyable flow
- a clean layout
- a few useful visuals or interactions
- solid explanations that help the reader truly understand the topic
