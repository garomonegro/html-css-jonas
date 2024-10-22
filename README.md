## theory-lectures-v2-BEST.pdf

https://drive.google.com/drive/folders/1ag9XK4aQS0Aux9-aVkxKTCsieP8_Gs0c?usp=sharing

## Concepts

- Static vs Dynamic Websites

## HTML

HyperText Markup Language: to structure and describe the content of a webpage (not a programming language), consists of elements that describe the type of content (paragraphs, links, headings, images, videos, etc.)

### Concepts

- Elements: (e.g. `<button>`, `<article>`, `<p>`, etc.)
- Attributes: (e.g. `src`, `alt`, `href`, etc.) part on an Element
- Entities: (e.g. `&copy;`) part of the content
- Semantic HTML: (e.g. `<strong>` vs `<b>`, `<em>` vs `<i>`, `<nav>` vs `<div>`)

### Good practices

- only one `<h1>` per page
- `<strong>` instead of `<b>` (html 5)
- `<em>` instead of `<i>` (html 5)
- Always add `alt` to all images, its used by search engines to know what the image is about BUT also for screen readers used by blind people. If the image is broken the alt text is shown.
- The first page should be called `index.html`

## CSS

Cascading Style Sheets: to describe the visual style and presentations of the content written in HTML

### Concepts

- CSS Rule
  - Selector: e.g. `h1`
  - Declaration Block: multiple Declarations contained by curly brackets
    - Declaration or Style: e.g. `front-size: 20px;`
      - Property: e.g. `font-size`
      - Value: e.g. `20px`
- Inline CSS: using the `style` attribute in the html code (Separation of Concern)
- Internal CSS: `style` element instead of an attribute
- External CSS: independent `*.css` file
- RGB/RGBA Notation: `rgb(0,255,255)`, `rgba(0,255,255,0.3)`. The A in RGBA in Alpha or Transparency
- Hexadecimal Notation: #00ffff, 0 to ff instead 0 to 255. Shorthand #0ff
- Element Selector: the element name
- ID Selector: `#` as prefix of the ID name
- Class Selector: `.` as prefix of the class name
- Pseudo Class: automatic/inferred class, e.g. `element:pseudo-class`
- Conflicting Selector Declarations or Selector Declaration Priority: If multiple ID/Class/Pseudo-Class/Element selectors with conflicting Declarations, the last one applies.
  - Declarations marked `!important` have the highest priority, its used as a last resort to resolve conflicts (bad practice)
  - Then Inline Style (bad practice)
  - then ID. If multiple selectors with conflicting Declarations, the last one applies
  - then class or pseudo-class. If multiple selectors with conflicting Declarations, the last one applies
  - then element. If multiple selectors with conflicting Declarations, the last one applies
  - lastly the universal selector
- Universal Selector (\*):
- Multiple Classes: `class="class-1 class-2"`
- Important Keyword: `color: #0f0 !important;`
- Inheritance: child Elements inherit from Parent elements declarations and these have the lowest priority. Not all declarations get inherit, mostly text related ones.

### Good practices

- Do not use Inline CSS
- `id` or `class` instead of descendant selector with the html element
- User `class` instead of `id` even if there is only one use of it
- Hexadecimal for color and RGBA when transparency is needed
- Define element `a` pseudo-classes `visited`, `hover`, and `active` in that same order

## Notes

- The browsers Developer Tool allows you to see, modify and play with the Elements, Styles, pseudo-classes, etc.

## Questions

- Jonas said that HTML, CSS amd JS are the languages browsers accept. Are there other languages?
