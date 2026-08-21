---
name: emerging-tech-company-analyst
description: Research an emerging technology company, begin with a beginner-friendly analogy that creates an intuitive mental model, and first present a concise, reviewable company-analysis framework; after the user approves the direction, turn it into a polished, self-contained HTML visual brief. Use when the user asks to understand, analyze, map, profile, or visually explain an AI, developer-tools, infrastructure, open-source, deep-tech, or fast-changing startup/company; especially for requests mentioning an industry map, company snapshot, visual brief, Soft Editorial, target customer, business model, company stage, competitive position, developer audience, third-party perspectives, or a three-minute company explainer.
---

# Emerging Tech Company Analyst

Create a visual understanding product, not a long research report. Help a reader understand an unfamiliar emerging-tech company in about three minutes. Organize the explanation in progressive layers so the reader can stop early without losing the main idea.

Use a two-stage workflow by default:

1. Research and present a concise content framework for review.
2. Create the HTML visual brief only after the user approves the framework.

If the user's initial request explicitly asks for an HTML file or says to skip review and deliver the finished visual, proceed directly to Stage 2 after research. Do not treat a general request such as “了解一下这家公司” as approval to create HTML.

## Read the supporting guidance progressively

- Before researching or writing Stage 1, read `references/content-framework.md` completely for evidence, editorial selection, and adaptive-map rules.
- Read `references/soft-editorial-system.md` completely only when entering Stage 2.
- Use `assets/fal-soft-editorial-example.html` only as a visual composition reference during Stage 2 when helpful. Never copy its company facts, citations, dates, or wording into another brief.

## Stage 1 — Research and content framework

### 1. Establish the brief

- Identify the company, requested language, intended reader, and any emphasized audience.
- Default to a smart newcomer with no industry vocabulary unless the user demonstrates or requests a higher level of expertise.
- Resolve ambiguous company names with a focused check. State the identity selected and continue when the match is strong; ask only when ambiguity would materially change the result.
- Default to the user's language while preserving standard English industry terms when they are more natural, such as `Generative AI Infrastructure`, `Inference Platform`, `Developer-first`, `AI Coding`, or `Serverless`.
- Treat `Emerging Tech Company Analyst` as the product identity unless the user renames it.

### 2. Research current facts

- Browse for current information and record a research cut-off date.
- Start with primary sources: official website, docs, pricing, blog or funding announcements, GitHub, LinkedIn, and official social profiles.
- Add independent sources: reputable reporting, investor or regulatory material when relevant, and traceable community discussions such as Hacker News, Reddit, GitHub issues, or product-review forums.
- Separate first-party claims, named customer testimony, reported facts, and community anecdotes.
- Confirm the latest officially announced funding stage. Treat rumors and talks as unconfirmed and exclude them unless they materially change understanding and are clearly labeled.
- Skip unsupported fields instead of estimating them.

### 3. Build an evidence ledger

For every candidate claim, track:

- the claim;
- direct source URL;
- source type;
- publication or update date when available;
- confidence and any caveat;
- whether the claim changes the reader's understanding.

Do not compose the framework until the company category, primary audience, business model, stage, and external praise or concerns have support or have been deliberately omitted.

### 4. Distill the story

- Find one familiar real-world situation that mirrors the company's role and relationships.
- Write one plain-language sentence explaining what the company does.
- Name the company's industry layer, not just its broad market.
- Identify the primary audience. If Developers are core, mark `Developers` as the emphasis for the eventual visual.
- Choose the visualization that best explains the company's position. Do not force every company into the same industry map.
- Include only facts that change the reader's understanding. Funding belongs when it signals stage, strategic backing, or competitive power—not merely because it exists.
- Make every proposed section teach one thing.
- Decide which single conclusion matters most and state it early. Supporting detail should deepen that conclusion, not repeatedly announce it.

### 5. Build the opening analogy

Start the reader's experience with one concrete analogy before using industry taxonomy.

- Create a small scene with actors, a problem, and an action. Explain who has the problem, what the company observes or changes, and why that matters.
- Explain relationships and workflow, not merely word meanings. An acronym expansion or a sentence such as “X is like a smart analytics tool” is not an analogy.
- Map two to four parts of the scene back to the real product only after the scene is understandable.
- Use one central analogy rather than a chain of unrelated metaphors. Reuse it lightly when introducing later concepts.
- State the analogy's limit when it could create a misleading impression.
- Introduce each necessary industry term only after the mental model exists. On first use, attach it to a concrete role in the analogy and a short plain-language phrase.

Good pattern:

> Imagine a global sports broadcast as hundreds of thousands of living rooms watching at once. The broadcaster's control room cannot see which specific televisions are buffering. The company acts like a lightweight observer beside each screen, reporting problems live so engineers can see that one device model in one region broke after an update. Only then name the observer as a `Sensor / SDK` and the viewing smoothness as `QoE`.

Avoid opening with a glossary, category definition, acronym list, or a paragraph dense with translated jargon.

### 6. Compress into progressive depth

Build Stage 1 as three useful stopping points:

1. **30 seconds — understand the role:** one analogy, a compact analogy-to-reality mapping, and the core conclusion.
2. **Two minutes — understand the business:** where the company sits, who uses and pays for it, how it makes money, its confirmed stage, and two or three reasons it earns consideration.
3. **Final layer — form a judgment:** the strongest outside signals, the most important risk or unknown, and exactly three things to remember.

For a Chinese brief, aim for roughly 800–1,200 Chinese characters before the source list; use a comparable three-minute reading length in other languages. Exceed this only when omitting context would materially distort the company.

Apply a strict repetition budget:

- Explain each central idea fully once.
- It may appear once more only as a one-sentence memory cue in `Remember This`.
- Do not restate the same category thesis across the analogy mapping, industry map, core judgment, and conclusion.
- When two sections answer the same question, merge them or delete the weaker one.

### 7. Present the reviewable framework

Deliver a compact text-first draft. Do not create an HTML file, image, visual asset, or elaborate layout at this stage.

Use this default structure, adapting or omitting unsupported parts:

1. **30-second understanding** — the opening analogy, a two-to-four-item reality mapping, and the core conclusion.
2. **Two-minute business read** — Where It Fits, Customer & Money, company stage, and two or three reasons people choose it. Include a simple adaptive-map sketch only when it clarifies the company's role.
3. **Judgment layer** — the strongest third-party praise or concern, the key strategic risk or unknown, and exactly three short memory cues.
4. **Evidence boundary** — distinguish verified facts, company plans, third-party views, and analyst inference; name only important unknowns.
5. **Source snapshot** — four to six of the strongest primary and independent sources with links and the research cut-off date.

Keep Stage 1 concise enough to review quickly. Prefer a clear thesis and compact bullets over polished prose. Before delivery, remove any paragraph that does not add a new answer, implication, or piece of evidence.

### 8. Stop at the approval gate

- End by asking whether the framework and emphasis are correct and whether the user wants the HTML version.
- Do not begin Stage 2 in the same turn unless the user already explicitly requested immediate HTML delivery.
- Treat responses such as “OK”, “可以”, “就按这个”, “做成 HTML”, or equivalent explicit approval as authorization to enter Stage 2.
- If the user requests changes, revise the framework first and wait for approval again.

## Stage 2 — HTML visual brief

Enter this stage only after explicit approval or an explicit initial request for immediate HTML.

### 9. Compose the visual narrative

Preserve the same progressive reading path in the visual. Use this default sequence, adapting, merging, or omitting sections when evidence or company type calls for it:

1. Start Here — the approved beginner-friendly analogy as the first reading path, before dense labels or industry terms.
2. Hero — company, category, primary audience, one-sentence explanation, and industry tags.
3. Where It Fits — the adaptive industry map as the largest explanatory section.
4. Customer & Money — target customer, business model, and company stage.
5. Why People Choose It — three or four evidence-backed reasons.
6. Outside Perspective — third-party praise and concerns, clearly caveated.
7. Remember This — exactly three memorable conclusions.
8. Keep Exploring — verified official Website, LinkedIn, X, GitHub, Docs, and other relevant official links.
9. Sources — compact citations with a research cut-off date.

The opening should deliver the 30-second understanding, the middle should explain the business, and the final layer should support judgment. `Remember This` is a compressed recall device, not a second explanation of the page.

Do not use star ratings.

### 10. Design the HTML

- Produce a single HTML file with inline CSS and only necessary inline JavaScript.
- Do not require a build step, package installation, remote font, external stylesheet, or JavaScript framework.
- Use semantic HTML, responsive layouts, visible focus states, adequate contrast, and print-friendly CSS.
- Keep the page visually scannable: strong hierarchy, generous whitespace, short paragraphs, compact labels, and a restrained editorial palette.
- Let the analogy shape the first visual explanation when useful, but do not add a decorative illustration that teaches nothing.
- Prefer HTML/CSS diagrams for the adaptive map. Use inline SVG only when it materially improves clarity.
- Make citation markers clickable and place sources close to the claims they support.
- Open external links in a new tab with `rel="noopener"`.
- Preserve the approved framework's thesis and emphasis. If new research materially changes them, explain the change before redesigning the narrative.
- Do not turn removed detail back into decorative cards. Whitespace is preferable to repeated content.

### 11. Verify before delivery

- Open the local file in a browser and inspect desktop and mobile widths.
- Check for horizontal overflow, clipped text, awkward Chinese wrapping, console errors, and broken section anchors.
- Verify official links and a representative sample of citation links.
- Confirm that external claims are distinguishable from company marketing.
- Confirm that a newcomer can explain the company after the opening analogy and that no unexplained acronym appears before it.
- Scan section openings and conclusions for duplicate claims. Keep the fullest explanation in the section that owns the idea and reduce any later recurrence to a short memory cue.
- Confirm that no unsupported detail, star rating, or placeholder remains.
- If browser-control tooling is available, follow its local-web-testing workflow.

### 12. Deliver

- Save the finished HTML in the user's writable workspace.
- Return a clickable absolute file link.
- State that it is a local file and not publicly shareable unless deployed.
- Briefly note the research cut-off and that desktop/mobile layouts were checked.

## Quality bar

The Stage 1 framework and final HTML should both let a reader answer, without rereading:

- What familiar situation helps me understand this company before I learn its terminology?
- What does this company actually do?
- Where does it sit in the industry?
- Who is it for?
- How does it make money?
- Why do people choose it?
- What should I be cautious about?
- What three things should I remember?

If a section cannot answer one of these questions with evidence, revise it or remove it.
