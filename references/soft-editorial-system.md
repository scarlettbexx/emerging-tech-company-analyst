# Soft Editorial visual system

## Contents

1. Direction
2. Design tokens
3. Typography and hierarchy
4. Layout grammar
5. Section treatments
6. Responsive behavior
7. Accessibility and technical constraints

## 1. Direction

Make the brief feel like a thoughtful technology magazine: warm, calm, credible, and contemporary. The page should reward scanning while preserving editorial depth.

Avoid:

- generic SaaS dashboard styling;
- glossy gradients, neon glow, glassmorphism, and excessive shadows;
- a card for every fact;
- crowded logo walls;
- decorative charts that do not teach;
- emoji as the primary visual language;
- star ratings.

Use contrast through scale, whitespace, rules, and restrained color rather than decoration.

## 2. Design tokens

Use system fonts so the HTML remains self-contained. A suitable default palette:

```css
:root {
  --paper: #f3eee4;
  --cream: #faf6ed;
  --ink: #1d211d;
  --muted: #686a60;
  --line: rgba(29, 33, 29, .17);
  --green: #173f34;
  --green-soft: #d9e3d9;
  --red: #9f3f32;
  --red-soft: #ead5cf;
  --sans: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont,
    "Segoe UI", "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", sans-serif;
  --serif: Iowan Old Style, Baskerville, "Times New Roman",
    "Songti SC", "STSong", serif;
}
```

These values establish the direction, not a rigid brand. Adjust the accent color when the company identity strongly calls for it, while retaining warm paper, dark ink, and editorial restraint.

Use one dark field for emphasis and one warm caution field. Avoid more than two accent colors.

## 3. Typography and hierarchy

- Use a display serif for company name and major conclusions.
- Use a neutral sans-serif for labels, metadata, tags, citations, and body copy.
- Let the company name dominate the first viewport.
- Use italic serif selectively for a conceptual modifier such as `Developer-first`.
- Keep body text at a comfortable line length, normally 55–75 characters.
- Use small uppercase labels with increased tracking for section numbers and evidence labels.
- Keep industry terms in English when translation would reduce precision.

Example hierarchy:

```css
h1 { font: 700 clamp(5rem, 15vw, 11.5rem)/.82 var(--serif); }
.section-title { font: 560 clamp(2.4rem, 6vw, 4.5rem)/1.02 var(--serif); }
.eyebrow { font: 800 .75rem/1 var(--sans); letter-spacing: .16em; }
```

## 4. Layout grammar

- Put the full brief inside one paper-like frame on desktop; let it become edge-to-edge on mobile.
- Use generous vertical section padding, normally `64–108px`.
- Introduce each section with a small numbered label and one large teaching headline.
- Use grid rules and 1px borders to create editorial structure.
- Keep the industry map wide and central.
- Alternate light sections with at most one dark section for rhythm.
- Use asymmetry deliberately: a large audience block beside smaller business-model cards is preferable to a uniform dashboard.

The page may be long. Scannability matters more than fitting everything above the fold.

## 5. Section treatments

### Hero

- Warm cream background.
- Oversized company wordmark rendered as text.
- One diagonal or geometric tonal field is acceptable.
- Industry tags use muted green pills with fine borders.
- Make Primary Audience the darkest or most visually dominant metadata block.

### Adaptive industry map

- Build in semantic HTML/CSS whenever possible.
- Use rows for layers, columns for actors, or axes for positioning.
- Highlight the company with a dark block and a small `YOU ARE HERE` label.
- Keep peer nodes visually neutral.
- Explain each layer in a short sentence.
- Add a relationship disclaimer when appropriate.

### Customer and business model

- Use one large red or dark audience panel.
- Place two or three compact revenue-mechanism cards beside it.
- Describe billing units, not an exhaustive price sheet.

### Why people choose it

- A dark green field works well.
- Use four large quadrants or three vertical arguments.
- Begin with concrete nouns: `Inference speed`, `Unified API`, `Deployment`, `Ecosystem`.

### Outside perspective

- Use one praise panel and one concern panel only when both have evidence.
- Keep praise on cream or pale green; use pale red for concerns.
- Include source-type labels such as `Community`, `Customer`, `Reporting`, or `GitHub`.
- Keep caveats visually close to anecdotal evidence.

### Remember this

- Use exactly three large numbered conclusions.
- Each card gets one strong sentence and one short explanation.

### Keep exploring and sources

- Use a dark footer.
- Present official links as editorial rows rather than generic buttons.
- Put source citations in a compact two-column list on desktop and one column on mobile.
- Display the research cut-off date.

## 6. Responsive behavior

Recommended breakpoints:

- Below `850px`: stack major grids and reduce headline scale.
- Below `580px`: remove the outer frame, use 20px side padding, and switch all multi-column sections to one column.

Verify:

- no horizontal overflow at 390px;
- the hero wordmark does not clip;
- maps remain readable without tiny text;
- Chinese text does not create isolated punctuation or broken labels;
- tags wrap naturally;
- citation markers remain tappable;
- footer links become one column if needed.

For a layered map on mobile, retain the label column only if it remains legible. Otherwise move the layer label above each row.

## 7. Accessibility and technical constraints

- Set `<html lang>` to the content language.
- Use `main`, `section`, `article`, `nav`, and `footer` landmarks.
- Connect section headings with `aria-labelledby`.
- Give diagrams an accessible label or textual caption.
- Include `:focus-visible` styles.
- Meet readable contrast on colored panels.
- Respect semantic heading order.
- Use real text rather than embedding critical copy in images.
- Add print CSS and avoid splitting major sections where practical.
- Do not use remote fonts, external stylesheets, tracking scripts, analytics, or third-party JavaScript.
- Do not fetch remote images unless the user explicitly wants them and self-containment is not required.
- Keep all research links as normal external anchors; the page itself must still render without network access.

The reference asset `assets/fal-soft-editorial-example.html` demonstrates this system. Treat it as a visual example, not a universal page template: choose a different map, section proportions, or accent treatment when the company's story requires it.
