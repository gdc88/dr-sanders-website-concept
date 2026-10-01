# Verification report

## Arbeitskonzept revision 03 verified on 1 October 2026

This scoped revision follows the client's direct review of the published one-page concept rather than treating the newly supplied AI-style variants as approved requirements:

- overlapping moisture, mould, basement-water, roof and façade entries were consolidated into one cause-and-damage path;
- the problem grid now contains seven distinct situations in a balanced 4 + 3 desktop composition;
- the neutral `Warum Dr. Sanders?` section now explains the connection between planning, practical construction experience and expert assessment;
- the office role is stated consistently as inspection, planning, coordination and professional supervision, while appointed specialist contractors carry out construction work;
- the example case now describes technical assessment and optional professional support instead of implying that the office performs refurbishment work;
- the unverified `1978`, `100+` publications and `3` patents proof strip was removed from the public concept;
- the hero photograph is labelled as a working image with project attribution and image rights still requiring confirmation;
- all visible photograph labels and alternative text are localized in DE/RU/EN;
- FAQ, Ratgeber, Turkish localization, named clients, prices, response promises and a multi-page production architecture were intentionally not added.

Verification evidence:

- W3C Nu HTML validator: **0 messages**;
- JavaScript syntax and Git whitespace checks: passed;
- every visible text and image-alt key is present in DE/RU/EN;
- rendered DOM confirms `lang`, seven cards, `Warum Dr. Sanders?`, contractor boundaries and working-image labels in all three languages;
- exactly **7** problem cards and **6** service rows;
- no duplicate IDs or missing local assets;
- Lighthouse: Performance **99**, Accessibility **100**, Best Practices **100**, SEO **66**; the SEO score remains intentionally reduced by the concept's `noindex` policy;
- German steel desktop, English graphite-green desktop and Russian graphite-green mobile visual checks passed;
- full-page visual QA confirmed the balanced 4 + 3 problem grid, anonymized case, neutral differentiation section, contractor boundary, process, contact and footer without clipping or collisions.

## Final Arbeitskonzept verified on 30 September 2026

The second working concept implements the client's latest direction:

- the page now starts with eight concrete client problems before services;
- six services remain in the confirmed priority order;
- the hero emphasizes technical expertise and integrated support;
- technical condition and market valuation remain separate;
- the sixth service is framed as a client journey from specification to acceptance;
- the competitor-comparison table was not adopted;
- the case study is anonymized and visibly marked as a structure pending project approval;
- the public draft label accurately states that the concept is viewable but not production-approved;
- steel-blue and graphite-green palette options can be switched in-page and selected with `?theme=steel` or `?theme=green`.

Verification evidence:

- W3C Nu HTML validator: **0 messages**;
- JavaScript syntax and Git whitespace checks: passed;
- 107 visible translation keys complete in DE/RU/EN;
- exactly 8 problem cards and 6 service rows;
- no duplicate IDs, missing local assets, forms, masked telephone links, or old client-path section;
- Lighthouse: Performance **99**, Accessibility **100**, Best Practices **100**, SEO **66** (intentional `noindex` prototype);
- desktop 1440×1100 steel and graphite-green variants visually passed;
- Russian mobile 375×900 visually passed after increasing theme controls to 44px minimum height;
- tall-viewport hero height is capped to prevent artificial blank space before the following sections;
- full sequence visually confirmed: hero → problems → services → anonymized case → neutral advantages → process → contact → footer.

## Update verified on 30 September 2026

The discussion concept was aligned with the latest client interview before publication:

- hero now presents integrated engineering services for Berlin, Teltow and Brandenburg;
- three client paths explain purchase/sale, existing-property work and new construction;
- technical condition assessment is explicitly separated from market valuation;
- six services are ordered by the client's stated business priority;
- the scope note makes clear that specialist contractors perform construction work;
- no unverified branch offices, brokerage/legal services, testimonials or universal-service claims were added.

Current checks:

- JavaScript syntax (`node --check`) and Git whitespace checks passed;
- 103 visible translation keys are complete in DE/RU/EN;
- no duplicate IDs, missing local resources or images without alternative text;
- required sections, 3 client paths and 6 service rows are present;
- desktop 1440×1100 and mobile 375×900 first-screen visual QA passed after explicit German soft hyphenation;
- full-site print review found no screen-content overflow; page splits remain print-only artifacts.

Verified locally on 25 September 2026 before the original GitHub Pages publication.

## Automated checks

- JavaScript syntax: `node --check script.js` — passed.
- HTML structure/link/i18n check: no duplicate IDs, missing local assets, untranslated visible keys, missing image alternatives or forms.
- W3C Nu HTML validator: **0 errors** after fixes.
- Language rendering through `?lang=de`, `?lang=ru`, `?lang=en`: translated hero copy and `<html lang>` verified in rendered DOM.
- Browser console/load errors: none in DE/RU/EN rendered-DOM runs.
- Contrast spot checks:
  - ink / paper: 14.22:1
  - white / dark copper: 7.82:1
  - white / ink: 15.92:1
  - muted text / paper: 5.22:1
  - soft ink / paper: 9.00:1

## Lighthouse (local HTTP)

Final scores at `http://127.0.0.1:8765/`:

- Performance: **99**
- Accessibility: **100**
- Best Practices: **100**
- SEO: **66** — intentionally reduced because this discussion prototype explicitly uses `noindex` and disallows crawling.

The first run identified and the final build fixed:

- missing favicon (404 console error);
- insufficient contrast on process step numbers;
- accessible-name mismatch on the brand link.

## Visual QA

Reviewed actual Chrome-rendered screenshots at:

- desktop: 1440 × 1100;
- mobile: 375 × 900;
- print/full-page contact sheet covering all sections.

Corrections made from the first visual pass:

- removed the fixed meeting toast that covered CTA/content;
- shortened and resized the hero title;
- fixed mobile long-word overflow;
- aligned the image with the top of the hero;
- replaced the hero image with a vertical project photograph that does not foreground the ZÜBLIN brand;
- removed a fake slider count from a static image;
- enlarged language hit targets;
- strengthened fine-print and project-label contrast.

Final desktop and mobile first-screen review found no blocking visual defects. Full-page print review found no missing images or broken sequence; apparent page splits are print-pagination artifacts, not browser layout failures.

## Slop diagnostic

Score: **0/10**.

- no glossy tech gradient;
- no generic indigo/violet accent;
- no equal-weight feature-tile grid;
- no decorative accent rails;
- no unearned glass panels;
- no oversized decorative statistics;
- no icon-topped filler cards;
- no centred-stack composition;
- typography and palette are chosen for the engineering/editorial context;
- the composition matches a Decide/Learn surface.

## Known intentional constraints

- This is a public-link prototype, not private content. The `noindex` and `robots.txt` directives are crawler requests, not access control.
- The top `Arbeitskonzept / Nicht zur Veröffentlichung` strip intentionally remains visible to prevent the draft being mistaken for an approved production website.
- No form backend, analytics, cookies, external fonts or tracking are present.
- Project images/facts come from the client's current public archive and still require final confirmation and usage approval for production.
- Legal/privacy texts are deliberately not invented in this concept.
