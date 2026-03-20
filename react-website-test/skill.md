Unslop profile for React marketing website.

## Hero patterns to never use
- Do not use the standard split hero with copy on the left and a glossy visual card on the right.
- Do not use the stack `eyebrow pill -> giant H1 -> short muted paragraph -> two-button CTA row`.
- Do not put a small rounded eyebrow directly above the H1.
- Do not use the exact hero rhythm `context label, oversized headline, 1-2 sentence blurb, primary CTA, secondary CTA`.
- Do not place a fake dashboard, fake analytics panel, fake browser window, fake stat stack, or fake product console in the hero.
- Do not use a framed rounded rectangle as the hero visual by default.

## Page structure defaults to avoid
- Do not build the page as `sticky nav -> split hero -> 3-card features -> testimonials -> pricing -> FAQ -> final CTA -> thin footer`.
- Do not repeat the same left-heading/right-paragraph section intro before every grid.
- Do not default to three-column mid-page sections for benefits, features, use cases, reviews, studies, or collections.
- Do not map arrays of exactly three items into card grids just because it is the easiest layout.
- Do not end with a large rounded CTA band, email signup slab, or demo card near the bottom.
- Do not use a low-information footer row with one brand line and a few muted links.

## Navigation patterns to avoid
- Do not use a sticky top nav as the default.
- Do not use the same nav hierarchy every time: brand on the left, links in the middle, one pill CTA on the far right.
- Do not blur or frost the nav shell.
- Do not make the nav another rounded floating pill.

## Color defaults to avoid
- Do not use off-white, beige, oat, ivory, sand, cream, or pale mint page backgrounds as the safe default.
- Do not use green-led palettes as the default brand system: `#0f7a5c`, `#0f6f52`, `#21382c`, sage, forest, emerald, moss, mint.
- Do not pair muted green with one warm accent and call that enough contrast.
- Do not use amber, clay, sand, or pale mint as the predictable secondary accent against green.
- Do not use dark green as the one `featured` or `premium` surface.
- Do not put white text on green gradients for the main CTA just because it reads as `modern SaaS`.

## Background and surface effects to avoid
- Do not build the page background from 2 blurred radial gradients over a soft linear wash.
- Do not add glow blobs in the corners to fake depth.
- Do not use translucent white panels over a tinted background as the base look.
- Do not rely on soft diffuse shadows everywhere to imply polish.
- Do not combine thin borders, blur, glow, and large radii on every important surface.

## Typography habits to avoid
- Do not default to `Manrope`.
- Do not use the same heavy, tightly tracked, oversized hero headline on every site.
- Do not use hero headlines with `clamp(...)` plus negative letter-spacing as the automatic move.
- Do not stack the H1 into 3-5 short lines with the same black-ish weight and compressed rhythm every time.
- Do not render supporting copy in the same muted gray-green tone across the whole page.
- Do not use small uppercase, mono, or label text as decoration for every eyebrow, chip, stat, and metadata row.

## Copy formulas to avoid
- Do not open with eyebrow text like `New`, `Now live`, `Built for teams`, `Trusted by`, `For modern teams`, `AI-native`, `Secure by design`, `Move faster`, `Ship faster`, `Scale with confidence`.
- Do not use hero headline formulas like `X that helps you Y`, `The platform for X`, `All your X in one place`, `Run X with clarity`, `Grow faster with X`, `The future of X`, `X for modern teams`.
- Do not pair the hero with filler lines like `Manage everything in one intuitive workspace`, `Turn complexity into clarity`, `Unlock insights`, `Streamline operations`, `Built to help your team move faster`.
- Do not use CTA pairs like `Get started` + `Learn more`, `Start free` + `Book demo`, `Start trial` + `See pricing`, `Talk to sales` + `Watch demo`.
- Do not add trust microcopy like `No credit card required`, `Cancel anytime`, `Trusted by 5,000+ teams`, `Loved by founders`.

## Component defaults to avoid
- Do not make every button a pill with `border-radius: 999px`.
- Do not make every badge, chip, pill, tag, filter, status marker, and eyebrow the same capsule shape.
- Do not use white or translucent rounded cards with faint 1px borders as the universal component shell.
- Do not use one dark featured pricing card surrounded by lighter cards as the default pricing hierarchy.
- Do not use short testimonial cards with a quote and compact author row as the default proof block.
- Do not use a small rounded-square logo mark with 1-2 initials as a stand-in brand.
- Do not over-round everything into the `14px` to `32px` radius band.

## Decorative tropes to avoid
- Do not use fake SaaS dashboards, fake stats, fake status rows, fake charts, fake compliance panels, or fake product widgets as decoration.
- Do not use abstract UI fragments as imagery: bars, dots, cards, browser chrome, KPI tiles, status pills.
- Do not use halo shadows around status dots.
- Do not use decorative circles, glows, and subtle blobs as filler texture.

## Layout and spacing defaults to avoid
- Do not constrain everything to the usual centered shell around `1120px` to `1180px`.
- Do not keep reusing slightly asymmetrical hero columns like `1.05fr / 0.95fr` or `1.15fr / 0.85fr`.
- Do not keep card padding clustered around `20px` to `24px` across the whole page.
- Do not keep gaps clustered around `12px` to `18px` across grids, button rows, and card internals.
- Do not use evenly stacked section bands with the same spacing logic all the way down the page.
- Do not treat mobile as one breakpoint where every grid collapses to `1fr`.

## React and code-level defaults to avoid
- Do not ship the same single-file HTML page with inline CSS, React from unpkg, ReactDOM from unpkg, Babel standalone, and `<script type="text/babel">`.
- Do not recreate the same `:root` token scaffold every time: background, text, muted, line, primary, accent, shadow, radius.
- Do not keep reusing class names like `.shell`, `.hero`, `.nav`, `.nav-inner`, `.brand`, `.brand-mark`, `.mark`, `.btn`, `.btn-primary`, `.btn-secondary`, `.card`, `.eyebrow`, `.section-head`, `.sectionHead`, `.pricing`, `.price`.
- Do not build nearly every section from the same grid/flex wrappers with minimal semantic variation.
- Do not reuse the same card property cluster everywhere: background fill, faint border, large radius, soft shadow, optional blur.
- Do not patch layout and spacing with repeated inline `style={{...}}` overrides all over the JSX tree.
- Do not treat `smooth-scroll + anchor links` as the default interaction model for every marketing page.

## Final check
- If any section starts looking like a reskinned version of the same landing page, stop.
- If the page still reads as the same template family with different copy, stop.
- Instead of reaching for any of these defaults, be creative. Vary your approach. If you catch yourself about to use any of the patterns listed above, stop and do something different.
