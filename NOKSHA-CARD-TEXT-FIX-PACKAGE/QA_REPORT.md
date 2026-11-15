# NOKSHA — Card Typography Fix QA Report

## Requested correction

The user marked text in the product category cards and collection cards that was appearing dark and visually misaligned.

## Applied fix

- Product card titles are explicitly white (`#fff`).
- Product card subtitles are soft white (`rgba(255,255,255,.78)`).
- Product card text containers use left alignment and left-anchored flex layout.
- Collection card titles are explicitly white.
- Collection card subtitles are soft white.
- Collection card copy is anchored at the bottom-left with consistent inset spacing.
- Mobile font sizes and spacing are retained with the same white/left-aligned treatment.
- Existing product images, card layout, brand colors and website interactions were not intentionally changed.

## Verification

- Confirmed the override is present in both `index.html` and `NOKSHA-standalone.html`.
- Confirmed both HTML files are byte-identical.
- Parsed the embedded CSS and checked for stylesheet parse errors.
- Confirmed the footer credit `Developed by RAFEUL` remains present.
- Generated `previews/NOKSHA-CARD-TEXT-FIX.png` to show the corrected product and collection card typography.
- ZIP integrity is checked after packaging.

## Scope

This update addresses only the marked product/category and collection card text styling. It does not claim to repair or re-test the live product editor workflow.
