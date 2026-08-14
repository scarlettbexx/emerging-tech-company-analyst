---
name: emerging-tech-company-analyst
description: Research an emerging technology company and turn the findings into a concise, polished, self-contained HTML visual brief. Use when the user asks to understand, analyze, map, profile, or visually explain an AI, developer-tools, infrastructure, open-source, deep-tech, or fast-changing startup/company; especially for requests mentioning an industry map, company snapshot, visual brief, Soft Editorial, target customer, business model, company stage, competitive position, developer audience, third-party perspectives, or a three-minute company explainer.
---

# Emerging Tech Company Analyst

Create a visual understanding product, not a long research report. Help a reader understand an unfamiliar emerging-tech company in about three minutes.

## Read the supporting guidance

Before researching or writing:

1. Read `references/content-framework.md` completely for evidence, editorial selection, and adaptive-map rules.
2. Read `references/soft-editorial-system.md` completely before designing the HTML.
3. Use `assets/fal-soft-editorial-example.html` only as a visual composition reference when helpful. Never copy its company facts, citations, dates, or wording into another brief.

## Workflow

### 1. Establish the brief

- Identify the company, requested language, intended reader, and any emphasized audience.
- Default to the user's language while preserving standard English industry terms when they are more natural, such as `Generative AI Infrastructure`, `Inference Platform`, `Developer-first`, `AI Coding`, or `Serverless`.
- Default to one self-contained `.html` file unless the user asks for another format.
- Treat the title `Emerging Tech Company Analyst` as the product identity unless the user renames it.

### 2. Research before designing

- Browse for current information. Record a research cut-off date.
- Start with primary sources: official website, docs, pricing, blog/funding announcements, GitHub, LinkedIn, and official social profiles.
- Add independent sources: reputable reporting, investor or regulatory material when relevant, and traceable community discussions such as Hacker News, Reddit, GitHub issues, or product-review forums.
- Separate first-party claims, named customer testimony, reported facts, and community anecdotes.
- Confirm the latest officially announced funding stage. Treat rumors and talks as unconfirmed and exclude them unless they materially change understanding and are clearly labeled.
- Skip unsupported fields instead of estimating them.

### 3. Build an evidence ledger

For every candidate claim, track:

- the claim;
- direct source URL;
- source type;
- publication/update date when available;
- confidence and any caveat;
- whether the claim changes the reader's understanding.

Do not begin the visual narrative until the company category, primary audience, business model, stage, and external praise/concerns have support or have been deliberately omitted.

### 4. Distill the story

- Write one plain-language sentence explaining what the company does.
- Name the company's industry layer, not just its broad market.
- Emphasize the primary audience visually. If Developers are the core audience, make `Developers` one of the dominant words on the page.
- Choose the visualization that best explains the company's position. Do not force every company into the same industry map.
- Include only facts that change the reader's understanding. Funding belongs when it signals stage, strategic backing, or competitive power—not merely because it exists.
- Make every section teach one thing.

### 5. Compose the brief

Use this default sequence, adapting or omitting sections when evidence or company type calls for it:

1. Hero — company, category, primary audience, one-sentence explanation, and industry tags.
2. Where It Fits — the adaptive industry map as the largest explanatory section.
3. Customer & Money — target customer, business model, and company stage.
4. Why People Choose It — three or four evidence-backed reasons.
5. Outside Perspective — third-party praise and concerns, clearly caveated.
6. Remember This — exactly three memorable conclusions.
7. Keep Exploring — verified official Website, LinkedIn, X, GitHub, Docs, and other relevant official links.
8. Sources — compact citations with a research cut-off date.

Do not use star ratings.

### 6. Design the HTML

- Produce a single HTML file with inline CSS and only necessary inline JavaScript.
- Do not require a build step, package installation, remote font, external stylesheet, or JavaScript framework.
- Use semantic HTML, responsive layouts, visible focus states, adequate contrast, and print-friendly CSS.
- Keep the page visually scannable: strong hierarchy, generous whitespace, short paragraphs, compact labels, and a restrained editorial palette.
- Prefer HTML/CSS diagrams for the adaptive map. Use inline SVG only when it materially improves clarity.
- Make citation markers clickable and place sources close to the claims they support.
- Open external links in a new tab with `rel="noopener"`.

### 7. Verify before delivery

- Open the local file in a browser and inspect desktop and mobile widths.
- Check for horizontal overflow, clipped text, awkward Chinese wrapping, console errors, and broken section anchors.
- Verify official links and a representative sample of citation links.
- Confirm that external claims are distinguishable from company marketing.
- Confirm that no unsupported detail, star rating, or placeholder remains.
- If browser-control tooling is available, follow its local-web-testing workflow.

### 8. Deliver

- Save the finished HTML in the user's writable workspace.
- Return a clickable absolute file link.
- State that it is a local file and not publicly shareable unless deployed.
- Briefly note the research cut-off and that desktop/mobile layouts were checked.

## Quality bar

The output succeeds when a reader can answer, without rereading:

- What does this company actually do?
- Where does it sit in the industry?
- Who is it for?
- How does it make money?
- Why do people choose it?
- What should I be cautious about?
- What three things should I remember?

If a section cannot answer one of these questions with evidence, revise it or remove it.
