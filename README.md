# Responsive layout repair demo

An original, standalone HTML/CSS demonstration of three common layout mistakes:

- Cards overflowing the mobile viewport.
- A fixed footer covering the final card.
- A visual stretched by an incorrect height rule.

Open `index.html` in a browser. Use **View reproduced defects** and **View repaired layout** to compare the two states. The broken mode is intentional. No build, account or external asset downloads are needed for the demo.

## What changes in the repaired state

The card grid uses flexible minimum widths and a mobile breakpoint. The footer returns to normal document flow. The geometric hero keeps its intended aspect ratio. Inspect the source to see the small CSS differences.

These techniques need adaptation to each site. Do not fix all overflow by hiding it globally: that can hide controls. A fixed footer can also be intentional; check whether the page makes enough room for it.

## A repeatable repair workflow

1. Reproduce the issue at the affected viewport.
2. Capture a before screenshot.
3. Change the responsible container or shared template.
4. Check the same viewport and at least one wider layout.
5. Test navigation, focusable controls, and unaffected pages.
6. Deliver a source diff and before/after evidence.

## Optional paid companion

[Responsive Layout Check Kit on Gumroad](https://purpledusttim.gumroad.com/l/gntlof) contains a Node.js/Playwright CLI for local multi-width screenshots, horizontal overflow checks, an optional footer-order check, HTML/JSON reports, and a repair checklist.

This free repository is useful on its own. The paid kit does not repair code automatically or certify visual correctness. It requires command-line use, Node.js and Chromium. Its installation was tested on macOS; other operating systems were not verified.

## Provenance

This is a synthetic, AI-assisted work sample, not a customer website, past client project, or testimonial. No personal data is collected by this demo. The Gumroad link opens an external commercial product page.

The MIT license below applies to this free demo repository. The separate paid kit has its own purchaser license.
