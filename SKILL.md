---
name: premium-portfolio
description: Transform an existing developer or professional portfolio website into a distinctive, premium, production-ready experience. Use when asked to redesign, polish, modernize, elevate, or make a portfolio feel high-end, editorial, elegant, or award-quality, while preserving real content and the existing stack.
---

# Premium Portfolio Transformation

## Mission
Act as a senior product designer, creative director, frontend engineer, accessibility specialist, and performance reviewer. Transform the user's **existing** portfolio into a refined, memorable, visually cohesive, trustworthy website. Implement the improvements in code rather than merely describing them.

The goal is **distinctive premium quality**, not gratuitous animation, bland SaaS templates, or visual complexity.

## 1. Inspect before editing
- Inspect project structure, framework, routing, styles, components, dependencies, content, assets, configuration, and git status.
- Identify the portfolio's intended audience, the owner's role, distinctive strengths, and the desired action (hire, contact, view work, download CV).
- Review existing pages and components. If browser/screenshot tools are available, capture desktop and mobile before screenshots.
- Inventory content to preserve: identity, biography, resume, project names, descriptions, links, dates, contact info, analytics, SEO, and external integrations.
- Do not invent achievements, work experience, metrics, testimonials, clients, or project claims. Do not add fake social proof or placeholder projects.
- Identify at least five concrete weaknesses, prioritized by their effect on credibility, aesthetics, usability, or conversion.
- Use the existing framework/design system where practicable. Do not rewrite the stack just for aesthetics.

## 2. Choose a visual direction
Before implementing, formulate a short creative direction: audience, brand adjectives, typography strategy, color palette, layout rhythm, motion principles, and one signature visual detail. Prefer a coherent direction like editorial minimalism, warm modernism, high-end technical, or understated brutalism, chosen to fit the person's work.

Quality bar:
- Strong typographic hierarchy, intentional scale, balanced whitespace, precise alignment, coherent grid, and predictable spacing tokens.
- Carefully chosen restrained palette with excellent contrast; optional accent used intentionally, not everywhere.
- Premium component detailing: beautiful navigation, project previews, refined buttons and links, thoughtful borders and surfaces, professional footer.
- Real personality. Avoid generic gradient blobs, excessive glassmorphism, default purple gradients, arbitrary icons, cloned templates, unnecessary loading screens, and wall-to-wall animations.
- If using photographs, screenshots, fonts, or illustrations, follow licensing and available assets. Never silently substitute invented portfolio work.

## 3. Upgrade the actual experience
Implement changes appropriate to the repository, prioritizing:
1. **Hero:** immediate professional positioning, distinctive headline, concise value proposition, clear primary action, optional secondary action.
2. **Navigation:** intuitive sections, responsive menu, visible active/hover/focus states, easy contact access.
3. **Work/projects:** curated case-study-like presentation with accurate problem, contribution, stack, outcome, and working links where source content supports them. Surface the best projects first.
4. **About/experience/skills:** readable, credible, scannable, avoid endless logo grids or generic filler.
5. **Contact:** clear human invitation and functioning contact methods, not an untested form.
6. **Finishing details:** consistent iconography, thoughtful microcopy, empty/error states, metadata, social previews where assets exist, favicon when appropriate.

Use CSS variables/design tokens or the stack's equivalent for typography, spacing, colors, radii, and motion. Factor reusable components only where helpful; avoid unnecessary abstraction.

## 4. Animation and interactions
- Use subtle, purposeful movement: tasteful entrances, hover feedback, project transitions, and micro-interactions only where they improve comprehension or delight.
- Respect `prefers-reduced-motion`; do not hide content behind animations that may never run.
- Ensure every button, menu, anchor, download, external link, and form actually works.
- Prefer lightweight CSS animations over heavy libraries unless the project already uses suitable tools.
- Keep scrolling smooth without hijacking scrolling or harming keyboard navigation.

## 5. Responsive, accessible, fast
- Test layout at narrow phone (approximately 360px), larger phone, tablet, laptop, and wide desktop sizes where feasible.
- Ensure no horizontal overflow, clipped headlines, unreadable text, or awkward project cards.
- Semantic HTML, correct heading order, alt text, accessible labels, keyboard navigation, visible focus, contrast, and touch-friendly targets.
- Optimize fonts, images, lazy loading, bundle size, and unnecessary client JavaScript. Preserve perceived performance.
- Follow existing SEO conventions; keep or improve page title, description, canonical/Open Graph metadata if supported.
- Do not add dependencies without clear benefits; never insert secrets or break env handling.

## 6. Implement, run, inspect, iterate
- Make code changes; do not stop at a mockup or a list of recommendations.
- Install dependencies only when genuinely needed and allowed by the environment.
- Run available formatting, lint, typecheck, tests, and build commands; fix problems introduced by the work.
- If a local browser or screenshot capability exists, **render the site and visually inspect** desktop and mobile. Iterate on typography, rhythm, navigation, contrast, spacing, and motion at least once based on what you see.
- Check console errors, broken navigation, links, form behavior, image loading, keyboard access, and reduced motion as feasible.
- Preserve unrelated user changes and avoid destructive resets. If blocked by missing tooling or credentials, state the limitation instead of claiming validation.

## 7. Completion report
Return a concise summary covering:
- Chosen art direction and what makes it specific to this portfolio.
- Main improvements actually implemented and important files changed.
- Tests/builds and visual checks performed (with outcomes).
- Any remaining limitations or actions requiring user input (such as real project imagery or content).

## Non-negotiable rules
- Preserve factual portfolio content unless user explicitly requests copy changes; polish language without fabricating facts.
- No fake testimonials, fictitious employers, metrics, project imagery presented as genuine, or dead CTA links.
- Do not confuse visual polish with excessive effects. Prefer editorial confidence and execution quality.
- Finish with working code, not just suggestions.


## Site-specific brief: Iyadh Manai (iyadhmanai.github.io)
This section applies when working on the repository backing https://iyadhmanai.github.io/.

### Existing site and positioning
- The current site has navigation for Work, Projects, Skills, Contact, plus a hero, experience, three projects, capabilities, delivery story, education, process, and contact sections.
- Preserve the identity Iyadh Manai and the substance of the work. Recast presentation toward a premium technical/product engineering portfolio, not a generic designer portfolio or a fictitious startup agency.
- Revisit the hero copy: it currently reads "Building dependable software at the meeting point of business and engineering." Keep the underlying engineering + business differentiator, but make the line clearer, sharper, and more memorable.
- Refine content hierarchy: visitors should understand who Iyadh is, what he builds, his best evidence, and how to contact him within seconds. Consolidate repetitive sections if appropriate, without losing substantive information.

### Projects: bespoke art direction
1. **Embedded internet radio / bachelor thesis (grade 1.0):** give it the lead case-study treatment. Showcase genuine STM32F769I-Discovery visuals if available in assets, architecture/system diagram, and concrete work in C, HTTPS streaming, networking, redirects and reconnect reliability. Do not invent test results or claim it was a commercial product. If diagrams are derived from the repository, label them appropriately.
2. **Dealna:** show as an *in-progress* marketplace MVP / technical project management case study for MENA. Emphasize roadmap, requirements, stakeholders, voucher redemption lifecycle, risk and scope. Use genuine screenshots if they exist; any speculative UI illustrations must be clearly labeled "Concept" and not represented as implemented features.
3. **Luma Bank:** show as an *in-progress* fintech architecture/delivery foundation. Highlight TypeScript, Next.js, NestJS, PostgreSQL, analytics, investment catalogue and compliance-aware planning only to the extent supported by source files. Any hypothetical banking dashboard must be transparently labeled a concept mockup, not a functional product.
- Give each project its own strong visual identity while keeping a unified site design. Replace uniform text-card treatment with spacious editorial project sections, authentic imagery, and succinct evidence of contribution.
- Keep working GitHub links and make every project CTA accurate; don't add case study URLs unless pages actually exist.

### Visual recommendation
Choose a sophisticated contemporary editorial style with restrained colors, precise Swiss-inspired typography, generous whitespace, calm motion, and technical detail. Make it distinctive, not template-like. Consider a dark charcoal / warm off-white dual-tone system with a single restrained accent, but adapt to existing photography and branding. Prefer very strong project art direction over decorative 3D effects.

### Content accuracy checks
- The deployed page currently says Cleversoft Group QA "2023 – Present" and "Current role". These may be outdated. Ask for or use verified resume/repository facts before changing dates; do not silently assume still employed.
- The deployed site shows B.Sc. Information Systems at TUM (Oct 2022–May 2026). Verify whether current studies should also include a master's degree before publishing changes.
- Inspect the downloadable CV and reconcile inconsistencies only when facts can be validated; otherwise flag them clearly in the completion report.
- Preserve real portrait, accurate contact methods, and SEO identity. Do not replace the owner's photo with AI-generated identity imagery.

### Acceptance criteria for this portfolio
- Obvious, memorable above-the-fold identity and CTA.
- Radio thesis stands out as the flagship engineering case study; Dealna and Luma Bank are clearly marked as in progress.
- Distinct visual storytelling for the projects instead of repeated generic cards.
- Excellent screen-space usage across 360px mobile to large desktop; deliberate tablet layout.
- Polished accessible navigation, working anchors, reduced-motion support, authentic copy, and production build passing.
- Audit actual rendered output after implementation; iterate on desktop/mobile screenshots if a browser tool is available.
