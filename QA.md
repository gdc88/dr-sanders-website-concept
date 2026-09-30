# Verification report

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
