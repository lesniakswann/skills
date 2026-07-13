---
name: lesniak-swann-format-brand-documents
description: Apply the Lesniak Swann document brand style and LS brand document rules across DOCX, PDF, slides, proposals, reports, exports, and styled Markdown. Use whenever the user mentions Lesniak Swann, LS, Lesniak Swann brand, LS brand, document brand, document style, brand style, brand guidelines, proposal styling, report styling, deck styling, or asks to create, polish, format, restyle, design, export, or make a business document feel on-brand. Treat this skill as the local source of truth for Lesniak Swann document styling; do not browse the web for Lesniak Swann brand guidance unless the user explicitly asks for current external research. Prefer document-first outputs; use HTML only when explicitly requested or as an intermediate rendering format.
---

# Branded Document Formatting

Use this skill when producing designed Lesniak Swann documents, including reports, proposals, audits, strategy documents, credentials, PDF exports, slide-style documents, and structured Markdown.

Apply the guidance silently. Do not add commentary inside the document about fonts, colour tokens, SCSS, CSS, or style rules unless the user explicitly asks for a style guide.

Treat this skill as the authoritative Lesniak Swann document style source. Do not search the web for Lesniak Swann brand references unless the user explicitly asks for live or external research.

Default to a document-first approach. Prefer DOCX, PDF, slides, or well-structured Markdown over standalone HTML. HTML is usually not useful as a final deliverable unless the user specifically asks for it or the toolchain needs HTML as an intermediate step to produce a PDF.

## Brand Feel

Documents should feel clear, spacious, editorial, and confident. Use light sections with dark text as the default. Do not add a separate cover page unless the user explicitly asks for one. Reserve dark blocks for occasional high-emphasis callouts, chapter dividers, or presentation-style section breaks.

Prioritise:

- Strong typographic hierarchy
- Generous line height
- Consistent spacing rhythm
- Plain, high-contrast colour use
- Restrained use of accent colours
- Clear tables, charts, and summary blocks where the content calls for them

## Fonts

Do not use Google Fonts. Use Proxima Nova where it is available, otherwise use the closest available sans-serif equivalent in the output format.

Preferred stack:

```text
Proxima Nova, Helvetica Neue, Helvetica, Arial, sans-serif
```

For DOCX or tools without Proxima Nova, use Helvetica Neue or Helvetica if available, otherwise Arial.

Use one type family throughout:

- Body: regular, `400`
- Strong/emphasis: bold, `700`
- Headings: very bold, `900` where available; otherwise bold
- Avoid decorative, serif, condensed, or script faces
- Avoid mixing multiple type families in the same document

## Type Hierarchy

Use a restrained hierarchy. Most documents need one H1, then H2 and H3 for most structure.

| Role | Use | Digital size | DOCX/PDF print size | Line height |
| --- | --- | --- | --- | --- |
| Title / H1 | Document title | 35px | 26pt | 1.15-1.2 |
| H2 | Major sections | 32px | 24pt | 1.15-1.2 |
| H3 | Subsections / finding groups | 27px | 20pt | 1.2-1.25 |
| H4 | Card headings / table groups | 23px | 17pt | 1.25-1.3 |
| H5 | Dense subheads | 20px | 15pt | 1.25-1.35 |
| H6 | Labels / minor headings | 17px | 13pt | 1.3-1.4 |
| Lead | Summary or opening intro | 19px | 14pt | 1.35-1.45 |
| Body | Main copy | 16px | 12pt | 1.45-1.55 |
| Small | Captions, notes, metadata | 13px | 10pt | 1.35-1.45 |
| X-small | Footnotes, source labels | 11px | 8pt | 1.3-1.4 |

When the output has limited page space, reduce sizes proportionally but keep the relative hierarchy intact.

Typography rules:

- Use dark text on light backgrounds for normal reading.
- Set body text with comfortable leading, never tightly packed.
- Keep heading line heights tight but not cramped.
- Use normal sentence case or title case for titles, headings, section names, table headers, chart labels, buttons, and callouts.
- Use all-caps only for very short labels or eyebrows of 1-3 words, such as `DRAFT`, `CONFIDENTIAL`, or `KEY POINT`.
- Do not make whole headings, paragraphs, table headers, chart titles, navigation labels, or recommendation blocks all-caps.
- Use bold for hierarchy, not underlines.
- Use underlines only for links.
- Keep letter spacing normal for body text; use slight positive tracking only on large headings or uppercase labels.
- Avoid centering long copy. Use left-aligned text for paragraphs, tables, notes, and recommendations.

## Colour Palette

Use these colours consistently:

| Name | Hex | Use |
| --- | --- | --- |
| Black | `#000000` | Primary text, dark accents |
| Off-black | `#1e1e1e` | Dark callout panels |
| White | `#ffffff` | Clean page/card backgrounds |
| Light cream | `#fff8ef` | Warm highlight background |
| Paper | `#f4f3ec` | Default document background or section bands |
| Paper dark | `#dfded3` | Borders, dividers, quiet table fills |
| Red | `#e2001b` | Primary accent, key figures, rules, warnings |
| Burnt red | `#9f0619` | Darker red accent where needed |
| Blue | `#4299d5` | Secondary accent, comparisons, neutral highlights |
| Mid grey | `#444444` | Dark-panel borders or muted dark UI details |

Colour rules:

- Default pages and sections should be `#f4f3ec` or `#ffffff` with `#000000` text.
- Use red sparingly. It should draw attention to the most important metric, exception, or action.
- Use blue as a secondary highlight or comparison colour, not as the dominant palette.
- Use `#dfded3` for light borders, table rules, and dividers.
- Dark panels should be rare and intentional, using `#1e1e1e` or `#000000` with white text.
- Do not create large gradients or one-colour decorative backgrounds.

## Logo

Use the inline SVG below when a Lesniak Swann logo is needed. Do not fetch a remote logo, reference a separate asset file, or recreate the logo from memory. Preserve the SVG aspect ratio, colours, and paths. Use it sparingly in headers, footers, title areas, or final pages; do not repeat it on every content block.

```svg
<svg xmlns="http://www.w3.org/2000/svg" id="Layer_1" viewBox="0 0 1920 489.74"><defs><style>.st0{fill:#231f20}.st1{fill:#d0202f}</style></defs><path d="M627.24 44.02h46.6l-7.17 42.5h-39.43zM171.93 265.29H33.95V44.9h45.38v184.27h81.84l10.75 36.13ZM249.55 234.18c8.09 0 16.24-.93 24.44-2.81 8.2-1.87 17.25-4.88 27.17-9.03l11.23 28.99c-24.69 11.44-47.51 17.1-68.46 17-25.7 0-45.89-7.49-60.56-22.47s-22.01-35.77-22.01-62.39 7.18-47.18 21.56-62.01c14.37-14.82 34.51-22.24 60.41-22.24 48.67 0 73.01 27.57 73.01 82.73v10.62H206.75c2.43 27.73 16.69 41.59 42.8 41.59Zm-5.92-102.61c-10.32 0-18.44 2.81-24.36 8.42-5.92 5.62-9.79 14.14-11.61 25.58h65.88c-1.31-22.67-11.28-34-29.9-34ZM446.89 109.86l-9.71 30.51c-10.73-3.54-19.26-6-25.58-7.36-6.33-1.37-11.97-2.05-16.92-2.05-7.69 0-13.76 1.47-18.22 4.4-4.45 2.93-6.68 6.88-6.68 11.84s2.12 8.48 6.37 11.16 10.62 5.29 19.12 7.82c11.84 3.34 21.23 6.45 28.16 9.33s13.08 7.69 18.44 14.42 8.05 15.91 8.05 27.55c0 15.99-5.95 28.46-17.84 37.42-11.89 8.95-28.21 13.43-48.95 13.43-21.76 0-42.6-4.35-62.54-13.05l11.23-30.66c11.84 4.35 21.42 7.41 28.76 9.18 7.33 1.77 13.89 2.66 19.66 2.66 8.09 0 14.22-1.52 18.36-4.55 4.15-3.04 6.22-7.33 6.22-12.9s-2.38-9.66-7.13-12.3c-4.76-2.63-12.45-5.46-23.07-8.5-9.92-2.93-18.19-5.95-24.82-9.03-6.63-3.09-12.32-7.97-17.08-14.65s-7.13-15.48-7.13-26.41c0-15.38 5.94-27.37 17.84-35.98q17.835-12.9 49.56-12.9c15.38 0 33.34 3.54 53.89 10.62ZM562.08 99.84c17 0 30.1 4.99 39.31 14.95 9.21 9.97 13.81 24.06 13.81 42.27v108.23h-46.6V159.64c0-9.51-1.87-16.39-5.62-20.64s-9.77-6.37-18.06-6.37c-7.49 0-14.47 1.69-20.95 5.08s-11.69 7.97-15.64 13.74v113.84h-46.75V102.42h38.86l5.01 22.62c14.37-16.8 33.24-25.2 56.62-25.2ZM627.24 104.24h46.6v161.05h-46.6zM811.59 116.23c12.24 11.34 18.37 27.78 18.37 49.33v99.73h-38.55l-5.31-19.28c-6.68 7.09-14.19 12.47-22.54 16.17-8.35 3.69-17.28 5.54-26.79 5.54-16.8 0-30.13-4.35-40-13.05s-14.8-20.39-14.8-35.06c0-17 7.16-30.26 21.48-39.77s34.33-14.27 60.03-14.27h19.88v-4.1c-.61-18.82-11.28-28.23-32.03-28.23-7.08 0-15.28 1.04-24.59 3.11-9.31 2.08-17.71 4.73-25.2 7.97l-9.87-31.42c10.73-4.35 22.01-7.72 33.85-10.09q17.76-3.57 33.24-3.57c22.97 0 40.58 5.67 52.82 17Zm-75.06 81.67c-7.34 4.55-11.01 10.88-11.01 18.97 0 6.68 2.02 11.76 6.07 15.25 4.04 3.49 9.76 5.24 17.15 5.24 6.68 0 13.08-1.47 19.2-4.4s11.26-6.88 15.41-11.84v-30.05h-15.94c-13.26 0-23.55 2.28-30.89 6.83ZM842.02 44.96h46.75v220.33h-46.75z" class="st0"/><path d="M995.3 265.29h-51.92l-58.74-90.46 51.61-72.41h49.48l-52.52 70.89zM1161.49 54.62l-9.56 36.43c-21.15-7.49-38.35-11.23-51.61-11.23-10.73 0-19.18 2.12-25.35 6.37-6.18 4.25-9.26 10.02-9.26 17.3 0 7.89 2.86 14.17 8.58 18.82q8.565 6.99 31.35 12.9c22.36 5.77 38.25 13.74 47.66 23.91s14.12 24.16 14.12 41.97q0 32.34-21.78 49.56c-14.52 11.49-35.24 17.23-62.16 17.23q-32.94 0-70.59-14.88l11.23-35.37c13.86 4.96 25.2 8.42 34 10.4 8.8 1.97 17.15 2.96 25.04 2.96 11.44 0 20.26-2.45 26.49-7.36 6.22-4.91 9.33-11.71 9.33-20.41 0-5.56-1.31-10.22-3.95-13.97-2.63-3.74-7.08-7.11-13.36-10.09s-15.33-5.94-27.17-8.88c-19.73-4.76-34.15-12.14-43.26-22.16s-13.66-23.23-13.66-39.62c0-20.95 7.21-37.16 21.63-48.65 14.42-11.48 34.68-17.23 60.79-17.23 18.21-.1 38.71 3.9 61.48 11.99Z" class="st0"/><path d="M1287.1 180c-.91-4.76-1.72-8.7-2.43-11.84l-2.73-14.88c-.61 2.03-2.08 8.65-4.4 19.88-.61 3.14-2.23 11.18-4.86 24.14l-17.76 68.46h-55.71l-43.87-162.87h45.08l17.15 72.4c1.82 7.49 4.6 19.73 8.35 36.73.4 2.33.93 4.88 1.59 7.67.66 2.78 1.29 5.59 1.9 8.42 6.37-24.89 10.93-42.5 13.66-52.82l20.19-72.4h37.04l19.88 72.4c1.82 6.37 3.47 12.32 4.93 17.84q2.205 8.28 3.72 14.49 6.225 23.385 5.31 20.49c2.53-10.32 6.47-28.03 11.84-53.13l17.15-72.1h45.08l-44.17 162.87h-55.71l-17.46-68.46c-1.62-6.78-2.88-12.55-3.79-17.31ZM1530.3 116.7c12.24 11.34 18.37 27.78 18.37 49.33v99.73h-38.55l-5.31-19.28c-6.68 7.09-14.19 12.47-22.54 16.17-8.35 3.69-17.28 5.54-26.79 5.54-16.8 0-30.13-4.35-40-13.05s-14.8-20.39-14.8-35.06c0-17 7.16-30.26 21.48-39.77s34.33-14.27 60.03-14.27h19.88v-4.1c-.61-18.82-11.28-28.23-32.03-28.23-7.08 0-15.28 1.04-24.59 3.11-9.31 2.08-17.71 4.73-25.2 7.97l-9.87-31.42c10.73-4.35 22.01-7.72 33.85-10.09q17.76-3.57 33.24-3.57c22.97 0 40.58 5.67 52.82 17Zm-75.06 81.67c-7.34 4.55-11.01 10.88-11.01 18.97 0 6.68 2.02 11.76 6.07 15.25 4.04 3.49 9.76 5.24 17.15 5.24 6.68 0 13.08-1.47 19.2-4.4s11.26-6.88 15.41-11.84v-30.05h-15.94c-13.26 0-23.55 2.28-30.89 6.83ZM1662.95 100.31c17 0 30.1 4.99 39.31 14.95 9.21 9.97 13.81 24.06 13.81 42.27v108.23h-46.6V160.11c0-9.51-1.87-16.39-5.62-20.64s-9.77-6.37-18.06-6.37c-7.49 0-14.47 1.69-20.95 5.08s-11.69 7.97-15.64 13.74v113.84h-46.75V102.89h38.86l5.01 22.62c14.37-16.8 33.24-25.2 56.62-25.2ZM1827.84 100.31c17 0 30.1 4.99 39.31 14.95 9.21 9.97 13.81 24.06 13.81 42.27v108.23h-46.6V160.11c0-9.51-1.87-16.39-5.62-20.64s-9.77-6.37-18.06-6.37c-7.49 0-14.47 1.69-20.95 5.08s-11.69 7.97-15.64 13.74v113.84h-46.75V102.89h38.86l5.01 22.62c14.37-16.8 33.24-25.2 56.62-25.2Z" class="st0"/><path d="M425.04 414.67c-5.41 4.81-12.96 7.21-22.65 7.21s-17.32-2.39-22.65-7.16-8-11.52-8-20.23v-52.25h10.63v52.25c0 5.93 1.66 10.33 4.96 13.21 3.31 2.87 8.33 4.31 15.06 4.31q20.13 0 20.13-17.52v-52.25h10.63v52.25c0 8.64-2.71 15.37-8.11 20.18M470.33 365.03q4.935-2.22 11.07-2.22c6.08 0 10.72 1.75 13.94 5.26q4.83 5.265 4.83 15.3v37.54H489.7v-36.78c0-4.23-.87-7.3-2.6-9.22s-4.52-2.88-8.35-2.88c-3.4 0-6.58.76-9.55 2.28s-5.35 3.62-7.16 6.29v40.31h-10.42v-57.13h8.46l1.19 8.03q4.125-4.56 9.06-6.78M520.26 356.14c0-6.08 1.59-10.78 4.77-14.11s7.67-4.99 13.45-4.99c2.21 0 4.35.22 6.43.65s4.6 1.25 7.57 2.44l-3.79 8.14c-3.84-1.27-6.98-1.9-9.44-1.9-2.75 0-4.85.79-6.32 2.39-1.47 1.59-2.2 3.8-2.2 6.62v8.41h16.22v9.01h-16.22v44.43c0 3.83-.28 7.35-.84 10.55s-1.47 6.57-2.74 10.12h-6.89v-65.1h-9.98v-9.01h9.98zM592.89 368.53c3.85 3.74 5.78 9.09 5.78 16.03v36.35h-8.03l-1.52-6.67c-5.57 5.17-11.83 7.76-18.77 7.76-5.72 0-10.25-1.54-13.62-4.61-3.36-3.07-5.04-7.2-5.04-12.37 0-6 2.46-10.69 7.38-14.05s11.83-5.05 20.72-5.05h8.41v-1.57c-.29-8.14-4.47-12.2-12.53-12.2-2.46 0-5.23.37-8.3 1.11s-6.16 1.75-9.28 3.01l-2.88-8.46c3.33-1.56 6.85-2.76 10.55-3.61 3.71-.85 7.26-1.28 10.66-1.28 7.13 0 12.61 1.87 16.46 5.62Zm-25.96 28.21q-4.83 2.85-4.83 7.95c0 2.6.89 4.6 2.66 5.99s4.25 2.09 7.43 2.09 6-.64 8.9-1.93 5.26-3.01 7.11-5.18v-11.77h-7.76c-5.79 0-10.29.95-13.51 2.85M616.1 342.68h10.42v10.69H616.1zm0 21.1h10.42v57.13H616.1zM662.06 365.09q4.02-2.28 8.79-2.28c2.13 0 4.61.4 7.43 1.19l-1.9 10.26q-5.43-1.08-7.32-1.14c-3.18 0-5.81.6-7.89 1.79s-3.86 3.13-5.34 5.8v40.2h-10.42v-57.13h8.35l1.3 8.03c1.99-2.96 4.32-5.21 7-6.73ZM757.04 367.58l-3.64 8.35c-4.67-2.6-9.19-3.91-13.56-3.91-5.32 0-9.42 1.76-12.31 5.26-2.89 3.51-4.34 8.5-4.34 14.97s1.48 11.48 4.45 14.92 7.25 5.16 12.86 5.16c2.06 0 4.38-.32 6.94-.95s5.03-1.46 7.38-2.47l2.82 8.3c-2.82 1.34-5.86 2.4-9.11 3.17s-6.33 1.17-9.22 1.17q-12.81 0-19.8-7.65c-4.67-5.1-7-12.31-7-21.64s2.4-16.48 7.22-21.67c4.81-5.19 11.52-7.78 20.13-7.78 5.97 0 11.7 1.59 17.2 4.77ZM812.44 370.49q7.11 7.785 7.11 21.78c0 13.995-2.37 16.58-7.11 21.76-4.74 5.17-11.39 7.76-19.96 7.76s-15.28-2.59-20.02-7.76-7.11-12.43-7.11-21.76 2.37-16.59 7.11-21.78 11.41-7.79 20.02-7.79 15.23 2.6 19.96 7.79m-32.19 6.64c-2.8 3.47-4.2 8.52-4.2 15.13s1.4 11.61 4.2 15.08 6.88 5.21 12.23 5.21 9.39-1.74 12.21-5.21 4.23-8.5 4.23-15.08-1.41-11.62-4.23-15.11-6.89-5.23-12.21-5.23-9.43 1.74-12.23 5.21M862.64 362.81c8.68 0 14.54 3.36 17.58 10.09 5.17-6.73 11.79-10.09 19.86-10.09 6.37 0 11.2 1.74 14.51 5.21s4.96 8.59 4.96 15.35v37.54h-10.47v-36.78c0-4.23-.87-7.3-2.6-9.22s-4.52-2.88-8.35-2.88c-3.4 0-6.51.74-9.33 2.23s-5.12 3.6-6.89 6.35c0 .14.04.49.11 1.03s.11 1.27.11 2.17v37.11h-10.47v-36.78c0-4.23-.87-7.3-2.6-9.22s-4.54-2.88-8.41-2.88c-3.26 0-6.32.76-9.2 2.28-2.87 1.52-5.18 3.58-6.92 6.18v40.42h-10.42v-57.13h8.46l1.19 7.92c5.03-5.93 11.32-8.9 18.88-8.9M982.64 370.35c4.36 4.96 6.54 11.99 6.54 21.11s-2.59 16.92-7.76 22.32c-5.17 5.41-12.35 8.11-21.54 8.11-3.47 0-7.52-.51-12.15-1.52v26.74h-10.42v-83.22h8.35l1.41 7.11c2.46-2.82 5.05-4.87 7.78-6.16s5.81-1.93 9.25-1.93c7.99 0 14.17 2.48 18.53 7.43Zm-9.04 36.73c3.29-3.73 4.94-8.94 4.94-15.62 0-6.15-1.32-10.91-3.96-14.27s-6.37-5.04-11.18-5.04c-3.76 0-7 .94-9.71 2.82s-4.7 4.64-5.97 8.3v27.78c3.04.72 5.26 1.18 6.67 1.35q2.115.27 5.37.27c5.93 0 10.54-1.86 13.83-5.59ZM1014.85 407.84c2.89 3.15 6.96 4.72 12.2 4.72 2.89 0 5.69-.31 8.38-.92 2.69-.62 5.76-1.67 9.19-3.15l3.31 7.76q-5.91 2.88-11.07 4.2c-3.43.89-6.89 1.33-10.36 1.33-8.61 0-15.28-2.59-20.02-7.76s-7.11-12.43-7.11-21.76 2.33-16.57 7-21.73c4.66-5.15 11.26-7.73 19.8-7.73 7.99 0 13.95 2.4 17.87 7.21s5.89 12.1 5.89 21.87v2.33h-39.87q.435 8.895 4.77 13.62Zm20.53-32.42c-2.22-2.26-5.29-3.39-9.19-3.39-8.68 0-13.87 4.49-15.57 13.45h28.54c-.29-4.45-1.55-7.8-3.77-10.06ZM1083.22 421.56c-5.5 0-9.68-1.42-12.56-4.26s-4.31-7.01-4.31-12.51v-32h-9.98v-9.01h10.52l2.23-16.33h7.7v16.33h17.41v9.01h-17.41v30.32c0 3.26.64 5.59 1.93 7 1.28 1.41 3.41 2.11 6.37 2.11 2.6 0 5.32-.47 8.14-1.41l1.95 8.19c-4.31 1.7-8.3 2.55-11.99 2.55ZM1107.54 342.68h10.42v10.69h-10.42zm0 21.1h10.42v57.13h-10.42zM1156.17 421.56c-5.5 0-9.68-1.42-12.56-4.26s-4.31-7.01-4.31-12.51v-32h-9.98v-9.01h10.52l2.23-16.33h7.7v16.33h17.41v9.01h-17.41v30.32c0 3.26.64 5.59 1.93 7 1.28 1.41 3.41 2.11 6.37 2.11 2.6 0 5.32-.47 8.14-1.41l1.95 8.19c-4.31 1.7-8.3 2.55-11.99 2.55ZM1180.49 342.68h10.42v10.69h-10.42zm0 21.1h10.42v57.13h-10.42zM1201.66 363.78h11.01l10.9 30.44c.58 1.63 1.2 3.54 1.87 5.72.67 2.19 1.18 3.81 1.55 4.85 0-.14.6 1.74 1.79 5.64l1.79-5.64c1.85-5.79 2.99-9.31 3.42-10.58l10.9-30.44h10.58l-20.35 57.13h-13.13l-20.35-57.13ZM1277.36 407.84c2.89 3.15 6.96 4.72 12.2 4.72 2.89 0 5.69-.31 8.38-.92 2.69-.62 5.76-1.67 9.19-3.15l3.31 7.76q-5.91 2.88-11.07 4.2c-3.43.89-6.89 1.33-10.36 1.33-8.61 0-15.28-2.59-20.02-7.76s-7.11-12.43-7.11-21.76 2.33-16.57 7-21.73c4.66-5.15 11.26-7.73 19.8-7.73 7.99 0 13.95 2.4 17.87 7.21s5.89 12.1 5.89 21.87v2.33h-39.87q.435 8.895 4.77 13.62Zm20.53-32.42c-2.22-2.26-5.29-3.39-9.19-3.39-8.68 0-13.87 4.49-15.57 13.45h28.54c-.29-4.45-1.55-7.8-3.77-10.06ZM1392.75 368.53c3.85 3.74 5.78 9.09 5.78 16.03v36.35h-8.03l-1.52-6.67c-5.57 5.17-11.83 7.76-18.77 7.76-5.72 0-10.25-1.54-13.62-4.61-3.36-3.07-5.04-7.2-5.04-12.37 0-6 2.46-10.69 7.38-14.05s11.83-5.05 20.72-5.05h8.41v-1.57c-.29-8.14-4.47-12.2-12.53-12.2-2.46 0-5.23.37-8.3 1.11s-6.16 1.75-9.28 3.01l-2.88-8.46c3.33-1.56 6.85-2.76 10.55-3.61s7.26-1.28 10.66-1.28c7.13 0 12.61 1.87 16.46 5.62Zm-25.96 28.21q-4.83 2.85-4.83 7.95c0 2.6.89 4.6 2.66 5.99s4.25 2.09 7.43 2.09 6-.64 8.9-1.93 5.26-3.01 7.11-5.18v-11.77h-7.76c-5.79 0-10.29.95-13.51 2.85M1453.72 413.69c-2.46 2.82-5.07 4.88-7.84 6.16s-5.81 1.93-9.14 1.93c-7.99 0-14.18-2.48-18.55-7.43-4.38-4.95-6.57-11.99-6.57-21.1s2.59-16.92 7.78-22.32c5.19-5.41 12.38-8.11 21.57-8.11 3.33 0 7.36.52 12.1 1.57v-26.8h10.42v83.22h-8.3l-1.46-7.11Zm-6.75-4.06c2.73-1.95 4.77-4.7 6.1-8.25v-27.67c-2.96-.72-5.19-1.18-6.67-1.38s-3.26-.3-5.32-.3c-5.93 0-10.54 1.87-13.83 5.62-3.29 3.74-4.94 8.94-4.94 15.6 0 6.15 1.31 10.9 3.93 14.27 2.62 3.36 6.34 5.04 11.15 5.04 3.65 0 6.85-.98 9.58-2.93M1473 363.78h11.01l10.9 30.44c.58 1.63 1.2 3.54 1.87 5.72.67 2.19 1.18 3.81 1.55 4.85 0-.14.6 1.74 1.79 5.64l1.79-5.64c1.85-5.79 2.99-9.31 3.42-10.58l10.9-30.44h10.58l-20.35 57.13h-13.13l-20.35-57.13ZM1573.24 368.53c3.85 3.74 5.78 9.09 5.78 16.03v36.35h-8.03l-1.52-6.67c-5.57 5.17-11.83 7.76-18.77 7.76-5.72 0-10.25-1.54-13.62-4.61-3.36-3.07-5.04-7.2-5.04-12.37 0-6 2.46-10.69 7.38-14.05s11.83-5.05 20.72-5.05h8.41v-1.57c-.29-8.14-4.47-12.2-12.53-12.2-2.46 0-5.23.37-8.3 1.11s-6.16 1.75-9.28 3.01l-2.88-8.46c3.33-1.56 6.85-2.76 10.55-3.61s7.26-1.28 10.66-1.28c7.13 0 12.61 1.87 16.46 5.62Zm-25.96 28.21q-4.83 2.85-4.83 7.95c0 2.6.89 4.6 2.66 5.99s4.25 2.09 7.43 2.09 6-.64 8.9-1.93c2.89-1.28 5.26-3.01 7.11-5.18v-11.77h-7.76c-5.79 0-10.29.95-13.51 2.85M1615.17 365.03q4.935-2.22 11.07-2.22c6.08 0 10.72 1.75 13.94 5.26q4.83 5.265 4.83 15.3v37.54h-10.47v-36.78c0-4.23-.87-7.3-2.6-9.22-1.74-1.92-4.52-2.88-8.35-2.88-3.4 0-6.58.76-9.55 2.28s-5.35 3.62-7.16 6.29v40.31h-10.42v-57.13h8.46l1.19 8.03q4.125-4.56 9.06-6.78M1681.97 421.56c-5.5 0-9.68-1.42-12.56-4.26s-4.31-7.01-4.31-12.51v-32h-9.98v-9.01h10.52l2.23-16.33h7.7v16.33h17.41v9.01h-17.41v30.32c0 3.26.64 5.59 1.93 7 1.28 1.41 3.41 2.11 6.37 2.11 2.6 0 5.32-.47 8.14-1.41l1.95 8.19c-4.31 1.7-8.3 2.55-11.99 2.55ZM1741.96 368.53c3.85 3.74 5.78 9.09 5.78 16.03v36.35h-8.03l-1.52-6.67c-5.57 5.17-11.83 7.76-18.77 7.76-5.72 0-10.25-1.54-13.62-4.61-3.36-3.07-5.04-7.2-5.04-12.37 0-6 2.46-10.69 7.38-14.05s11.83-5.05 20.72-5.05h8.41v-1.57c-.29-8.14-4.47-12.2-12.53-12.2-2.46 0-5.23.37-8.3 1.11s-6.16 1.75-9.28 3.01l-2.88-8.46c3.33-1.56 6.85-2.76 10.55-3.61s7.26-1.28 10.66-1.28c7.13 0 12.61 1.87 16.46 5.62ZM1716 396.74q-4.83 2.85-4.83 7.95c0 2.6.89 4.6 2.66 5.99s4.25 2.09 7.43 2.09 6-.64 8.9-1.93 5.26-3.01 7.11-5.18v-11.77h-7.76c-5.79 0-10.29.95-13.51 2.85M1796.66 364.41c2.33.7 4.39 1.69 6.16 2.96l1.25-3.58h8.62v58.7c0 7.63-2.44 13.64-7.32 18.04-4.89 4.4-11.54 6.59-19.96 6.59-4.24 0-8.33-.51-12.29-1.54q-5.94-1.545-10.5-4.32l3.91-8.35c2.67 1.48 5.8 2.68 9.38 3.61 3.58.92 6.96 1.39 10.15 1.39 5.17 0 9.17-1.31 11.99-3.93 2.82-2.63 4.23-6.38 4.23-11.26v-8.25c-4.52 4.88-9.96 7.32-16.33 7.32-7.99 0-14.18-2.48-18.55-7.43-4.38-4.95-6.57-11.99-6.57-21.1s2.48-16.82 7.43-22.05 11.99-7.84 21.1-7.84c2.53 0 4.96.35 7.3 1.06Zm-20.21 13.29c-3.29 3.78-4.94 8.96-4.94 15.54 0 6.15 1.31 10.9 3.93 14.27 2.62 3.36 6.34 5.04 11.15 5.04 3.69 0 6.93-1.01 9.71-3.04 2.79-2.03 4.77-4.83 5.97-8.41v-25.77c-1.7-1.05-3.64-1.86-5.83-2.44q-3.285-.87-6.48-.87c-5.72 0-10.22 1.89-13.51 5.67ZM1842.82 407.84c2.89 3.15 6.96 4.72 12.2 4.72 2.89 0 5.69-.31 8.38-.92 2.69-.62 5.76-1.67 9.19-3.15l3.31 7.76q-5.91 2.88-11.07 4.2c-3.43.89-6.89 1.33-10.36 1.33-8.61 0-15.28-2.59-20.02-7.76s-7.11-12.43-7.11-21.76 2.33-16.57 7-21.73c4.66-5.15 11.26-7.73 19.8-7.73 7.99 0 13.95 2.4 17.87 7.21s5.89 12.1 5.89 21.87v2.33h-39.87q.435 8.895 4.77 13.62Zm20.53-32.42c-2.22-2.26-5.29-3.39-9.19-3.39-8.68 0-13.87 4.49-15.57 13.45h28.54c-.29-4.45-1.55-7.8-3.77-10.06Z" class="st1"/></svg>
```

## Spacing

Use a steady vertical rhythm across pages, slides, sections, and content blocks:

- Paragraph and list spacing after: about `1.5-2x` body line height
- Small gap: about `24px` / `18pt`
- Medium gap: about `38px` / `28pt`
- Large gap: about `50px` / `38pt`
- Extra-large section gap: about `78px` / `58pt`
- Card or callout padding: about `24px` / `18pt`
- Table cell padding: about `10-14px` / `7.5-10.5pt`

Spacing rules:

- Leave more space above a new section than between paragraphs inside a section.
- Keep related headings, body copy, charts, and notes visually grouped.
- Avoid cramped tables; reduce copy before reducing line height.
- Avoid huge empty areas unless used deliberately on a section opener.

## Document Structure

Start with the user's requested structure. When the structure is unspecified, prefer a concise document flow:

- Header: clear document title, date or client metadata, and restrained accent rule.
- Summary: lead paragraph, key points, optional metric strip.
- Section opener: H2, short lead, then content blocks.
- Evidence or finding block: H3/H4, short explanation, evidence, implication or recommendation.
- Data block: clear chart/table title, chart/table, source note in small text.
- Callout: light card by default; dark card only for standout emphasis.
- Recommendation or action block: concise heading, body copy, owner/status/priority if useful.
- Cover: only include one when explicitly requested; use a large title, short subtitle, date or client metadata, and restrained accent rule.

Avoid nesting cards inside cards. Do not overuse decorative boxes; use them to clarify grouping.

## Tables And Charts

Tables:

- Use black text on white or paper backgrounds.
- Use `#dfded3` for grid lines or row separators.
- Use bold column headers.
- Use small text for notes and sources.
- Keep numeric columns aligned consistently.
- Use light row tinting only when it improves scanning.

Charts:

- Use black/grey as the base.
- Use red for the primary series or key exception.
- Use blue for comparison or secondary series.
- Label important points directly where possible.
- Keep legends, axis labels, and source notes in small type.

## Output Translation

Adapt the same rules to the output medium.

For DOCX:

- Define and reuse Word styles: Title, Subtitle, Heading 1-3, Body Text, Lead, Caption, Table Header, Table Body, Callout.
- Use point sizes from the DOCX/PDF column in the type table.
- Use exact or multiple line spacing equivalent to the line-height guidance.
- Use paragraph spacing after instead of extra blank paragraphs.
- Use page/section background colour only if the tool supports it reliably; otherwise use light shaded blocks sparingly.

For PDF:

- Treat it like print: use the DOCX/PDF point sizes.
- Keep body text around 12pt with generous leading.
- Use margins and section spacing rather than relying on large decorative containers.
- Check page breaks so headings do not orphan from their content.

For HTML:

- Do not choose HTML as the final document format unless explicitly requested.
- If HTML is used as a PDF-rendering intermediate, keep it print-oriented and generate the PDF deliverable.
- Use rem or px values matching the digital size column.
- Keep the root/body typography consistent across pages.
- Use responsive reductions only when needed for small screens.

For Markdown:

- Preserve semantic hierarchy with one H1, H2 for major sections, and H3 for findings.
- Do not include implementation details unless the user asks.
- Where visual styling is unavailable, use concise headings, tables, and spacing to preserve hierarchy.

## Final Check

Before finishing:

- Sections are light with dark text by default.
- Fonts are Proxima Nova, Helvetica Neue, Helvetica, Arial, or the closest available equivalent.
- The type hierarchy is obvious and consistent.
- Capitalisation is restrained: no heavily all-caps pages, headings, tables, or callouts.
- Body copy has comfortable line height.
- Colours come from the palette.
- Red and blue are accents, not decoration.
- Tables and charts are readable without relying on colour alone.
- The document does not explain its own styling rules.
