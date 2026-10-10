# Temporary handoff — mobile shopping session

Created: 2026-10-11T04:20:00+05:30 (IST)

## Purpose

This file is a compact continuation packet for the next session after context compaction. The canonical research remains under `mobile-shopping/`; this temporary file can be deleted after handoff.

## Current project structure

- `mobile-shopping/README.md`
- `mobile-shopping/strategy/general-purchase-strategy.md`
- `mobile-shopping/purchases/mobile-phone/requirements.md`
- `mobile-shopping/purchases/mobile-phone/research.md`
- `mobile-shopping/purchases/mobile-phone/evidence.tsv`
- `mobile-shopping/purchases/mobile-phone/mobile-phone-shopping-report.md`
- `mobile-shopping/purchases/mobile-phone/decision-history.md`
- `.gitignore`

## Latest user direction

- Drop eSIM from the mobile-phone requirements.
- Focus on cost-effective phones with the other important qualities retained.
- Keep social proof, user-review summaries, expert reviews, and timestamped evidence enabled for every search.
- Explain cost drivers and show price tiers.
- Search progressively: first full matches, then 8/10 and 6/10 candidates while preserving non-negotiables.

## Current cost-effective shortlist

1. **Samsung Galaxy F36 6GB/128GB** — best all-rounder if battery feedback is acceptable. Flipkart snapshot: 4.3/5, 12,879 ratings, 1,142 reviews, roughly ₹21,999–₹23,999. Super AMOLED, OIS, expandable storage shown up to 2TB. No eSIM.
2. **Motorola G57 Power 8GB/128GB** — strongest battery/popularity value. Flipkart snapshot: 4.4/5, 57,889 ratings, 4,164 reviews, ₹21,999. 7000mAh, Snapdragon 6s Gen 4, FHD display. LCD and Motorola support story are the trade-offs.
3. **Samsung Galaxy A17 6GB/128GB** — Samsung display/protection alternative. Flipkart snapshot: 4.3/5, 2,761 ratings, 244 reviews, about ₹22,660. Super AMOLED, Gorilla Glass Victus, expandable storage shown up to 2TB. Weaker performance/camera than F36.
4. **OnePlus Nord CE5 8GB/128GB** — strong performance/battery and Flipkart popularity: 4.5/5, 12,664 ratings, 873 reviews, ₹22,500, but unavailable in the captured snapshot.

## Recommendation state

- Default all-rounder: Samsung Galaxy F36.
- Best price/battery/popularity: Motorola G57 Power.
- Best Samsung display/protection: Galaxy A17.
- Do not raise the budget to ₹40,000 just for eSIM anymore.

## New evidence rows

The latest round added G57 Power and Galaxy A17 Amazon/Flipkart evidence to `evidence.tsv`, with seller/listing, review-summary and trade-off fields. Existing entries remain timestamped and separate by marketplace.

## Strategy update

`general-purchase-strategy.md` now includes:

- cost drivers and price ladders;
- 10/10, 8/10 and 6/10 progressive requirement relaxation;
- social proof, review summary, expert review and timestamped evidence as always-on gates.

## Git history

- `37dcdb2` Add mobile shopping research and evidence
- `56fb31a` Extend mobile research with timestamped marketplace evidence
- `76f0a19` Add Flipkart social proof and marketplace popularity sources
- `1c70643` Add seller fields and user review summaries
- `5964f40` Refine eSIM recommendation and budget trade-offs
- `52267f9` Re-rank cost-effective phones after dropping eSIM

After updating the strategy for this handoff, create a new commit before continuing.

## Next suggested action

Run one final value comparison for F36 vs G57 Power vs A17 vs Nord CE5, focusing on recurring negative user-review themes, warranty/seller quality, update support, display type, camera/OIS, storage expansion, battery and current stock. Produce a 10/10, 8/10 and 6/10 matrix and state the marginal price of each upgrade.

## Clarifications still useful later

1. Should the search be limited to new phones, excluding used/renewed/refurbished units?
2. Is microSD expansion still a preference, or can reliable 128GB internal storage replace it?
3. Should delivery/service be checked for a particular city, or is India-wide availability enough?
