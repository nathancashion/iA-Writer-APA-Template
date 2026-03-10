# APA 7 Style Template

## Setup

1. **Install the template**: Double-click `APA7.iatemplate` in Finder (or drag it to the iA Writer icon in Dock). On iOS, use AirDrop or "Copy to iA Writer."

2. **Set your author name** in iA Writer Preferences. This will appear on the title page.

3. **Edit title page placeholders**: Open the installed bundle (Preferences → Templates → right-click → "Show in Finder") and edit `title.html` to replace placeholder text for your department, university, course, and instructor.

4. **Select the template**: In iA Writer, go to Preferences → Templates and choose "APA 7."

## Writing Your Paper

Use standard Markdown headings mapped to APA 7 heading levels:

| Markdown | APA Level | Format |
|----------|-----------|--------|
| `#`      | Level 1   | Centered, Bold |
| `##`     | Level 2   | Flush Left, Bold |
| `###`    | Level 3   | Flush Left, Bold Italic |
| `####`   | Level 4   | Indented, Bold |
| `#####`  | Level 5   | Indented, Bold Italic |

### Title Page

The title page is generated automatically from `data-title` (your filename), `data-author` (from Preferences), and `data-date`. Fields for department, university, course, and instructor use placeholder text that you should customize in the template bundle.

### Block Quotations

Use Markdown block quotes (`>`) for quotations of 40 words or more. These will be indented 0.5" from the left margin per APA 7.

### Notes and References

MultiMarkdown footnotes `[^Lorem ipsum.]` and citations `[p. 23][#Doe:2006]` should be used to cite notes and works. The template will automatically separate them (unlike other templates), and it will alphabetically sort citations. References are formatted with a hanging indent on export.

### Math

TeX expressions delimited by the classical `$ ... $, $$ ... $$, \( ... \) \[ ... \]` are supported using [KaTeX](https://katex.org/).

## Known Limitations

- **Level 4/5 headings**: APA specifies these as inline headings (text continues on the same line after a period). CSS cannot merge block-level heading elements with the following paragraph, so they appear as standalone indented lines.
- **Professional papers**: This template targets the student paper format. Running heads and author notes for professional papers are not yet supported.
