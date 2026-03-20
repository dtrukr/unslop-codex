# Codex Prompt: Rewrite Existing Homepage Copy

Use this prompt when you want Codex to rewrite SaaS homepage copy without changing the design.

```text
Rewrite the homepage copy in this project.

Scope:
- Change copy only.
- Do not change layout, styling, component structure, spacing, visual hierarchy, or interaction design.
- Keep the same sections unless a section is purely repetitive filler.
- Preserve the actual product meaning, offer, and target buyer.

Goals:
- Make the copy sound specific to this exact product and buyer.
- Remove generic SaaS wording and repeated landing-page formulas.
- Keep the copy conversion-focused, but not interchangeable with every other SaaS site.
- Prefer concrete operational language over abstract benefit language.
- Replace vague trust copy with sharper, more credible statements where possible.
- Keep CTA intent intact, but improve wording if the current labels are generic.

Hard rules:
- Do not write meta delivery text like "Here’s a landing page copy draft you can use."
- Do not include implementation notes, status notes, or "If you want, I can..." language.
- Do not default to stock phrases like "Built for...", "Trusted by...", "Everything your team needs...", "one platform", "one dashboard", "move faster", "scale with confidence", or other generic SaaS filler unless the wording is genuinely necessary and specifically grounded.
- Do not flatten the product into a generic "efficiency software for modern teams" voice.

Process:
1. Read the existing homepage copy carefully.
2. Identify where it sounds generic, interchangeable, or overly abstract.
3. Rewrite the copy section by section.
4. Keep the page structure stable unless a section is obviously filler.
5. Make each section sound like it belongs to this exact category, buyer, and workflow.

Use this unslop profile while rewriting:

[PASTE THE CONTENTS OF saas-copy-unslop/skill.md HERE]

Output format:
- Return the revised homepage copy only.
- Preserve section labels/headings when useful.
- Do not explain your changes unless asked.
```

## Short Version

```text
Rewrite the homepage copy only. Do not change design or layout.

Use this unslop profile:
[PASTE skill.md HERE]

Make the copy specific, concrete, and category-native. Remove generic SaaS phrasing, generic trust-bar language, generic CTA wording, and generic "one platform / move faster / scale with confidence" messaging.

Return only the rewritten copy.
```
