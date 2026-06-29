---
name: Lesniak Swann Report Style
description: Apply the Lesniak Swann report style across DOCX, PDF, slides, and styled Markdown. Use when creating or restyling reports where consistent typography, line height, spacing, hierarchy, and brand colours matter. Prefer document-first outputs; use HTML only when explicitly requested or as an intermediate rendering format.
---

# Lesniak Swann Report Style

Use this skill when producing a designed report or report-like document for Lesniak Swann, regardless of output format.

Apply the guidance silently. Do not add commentary inside the report about fonts, colour tokens, SCSS, CSS, or style rules unless the user explicitly asks for a style guide.

Default to a document-first approach. For reports, prefer DOCX, PDF, slides, or well-structured Markdown over standalone HTML. HTML reports are usually not useful as final deliverables unless the user specifically asks for one or the toolchain needs HTML as an intermediate step to produce a PDF.

## Overall Feel

Reports should feel clear, spacious, editorial, and confident. Use light sections with dark text as the default. Do not add a separate cover page unless the user explicitly asks for one. Reserve dark blocks for occasional high-emphasis callouts or chapter dividers.

Prioritise:

- Strong typographic hierarchy
- Generous line height
- Consistent spacing rhythm
- Plain, high-contrast colour use
- Restrained use of accent colours
- Clear tables, charts, and summary blocks

## Fonts

Do not use Google Fonts. Use a widely available sans-serif stack or the closest equivalent available in the output format.

Preferred stack:

```text
Helvetica Neue, Helvetica, Arial, sans-serif
```

For DOCX or tools without Helvetica Neue, use Helvetica if available, otherwise Arial.

Use one type family throughout:

- Body: regular, `400`
- Strong/emphasis: bold, `700`
- Headings: very bold, `900` where available; otherwise bold
- Avoid decorative, serif, condensed, or script faces
- Avoid mixing multiple type families in the same report

## Type Hierarchy

Use a restrained hierarchy. A report should normally need only one H1, then H2 and H3 for most structure.

| Role | Use | Digital size | DOCX/PDF print size | Line height |
| --- | --- | --- | --- | --- |
| Title / H1 | Report title | 40-72px | 30-54pt | 1.1-1.2 |
| H2 | Major sections | 36-60px | 27-45pt | 1.1-1.2 |
| H3 | Subsections / finding groups | 28-52px | 21-39pt | 1.15-1.25 |
| H4 | Card headings / table groups | 24-40px | 18-30pt | 1.2-1.3 |
| H5 | Dense subheads | 20-32px | 15-24pt | 1.25-1.35 |
| H6 | Labels / minor headings | 20-28px | 15-21pt | 1.25-1.4 |
| Lead | Executive summary intro | 18-24px | 13.5-18pt | 1.35-1.45 |
| Body | Main copy | 16-18px | 12-13.5pt | 1.5-1.6 |
| Small | Captions, notes, metadata | 14px | 10.5pt | 1.35-1.45 |
| X-small | Footnotes, source labels | 12px | 9pt | 1.3-1.4 |

When the output has limited page space, reduce sizes proportionally but keep the relative hierarchy intact.

Typography rules:

- Use dark text on light backgrounds for normal reading.
- Set body text with comfortable leading, never tightly packed.
- Keep heading line heights tight but not cramped.
- Use all-caps only for short labels or eyebrows.
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
| Paper | `#f4f3ec` | Default report background or section bands |
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

## Spacing

Use a steady vertical rhythm:

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

## Layout Patterns

Use these recurring report patterns:

- Header: use a clear report title, date or client metadata, and restrained accent rule. Start reports with this header by default rather than a separate cover page.
- Cover: only include one when explicitly requested; use a large title, short subtitle, date or client metadata, and restrained accent rule.
- Executive summary: lead paragraph, 3-5 key findings, optional metric strip.
- Section opener: H2, short lead, then content blocks.
- Finding block: H3/H4, short explanation, evidence, implication or recommendation.
- Data block: clear chart/table title, chart/table, source note in small text.
- Callout: light card by default; dark card only for standout emphasis.
- Recommendation: concise heading, body copy, owner/status/priority if useful.

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
- Keep body text around 12-13.5pt with generous leading.
- Use margins and section spacing rather than relying on large decorative containers.
- Check page breaks so headings do not orphan from their content.

For HTML:

- Do not choose HTML as the final report format unless explicitly requested.
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
- Fonts are Helvetica Neue, Helvetica, Arial, or the closest available equivalent.
- The type hierarchy is obvious and consistent.
- Body copy has comfortable line height.
- Colours come from the palette.
- Red and blue are accents, not decoration.
- Tables and charts are readable without relying on colour alone.
- The report does not explain its own styling rules.
