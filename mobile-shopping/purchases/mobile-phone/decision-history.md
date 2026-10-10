# Mobile-phone decision history

This log records how the decision process changed as constraints were clarified.

| Timestamp | Instruction/constraint | Process change | Result |
|---|---|---|---|
| 2026-10-10 | Extract the phones already in the Amazon cart and provide direct links. | Inspected the cart and verified direct Amazon product URLs. | Identified Galaxy M17, Galaxy A56, OnePlus Nord CE6 Lite, and Motorola Edge 70 Fusion. |
| 2026-10-10 | Find a stable alternative under about ₹25,000; avoid Poco/Xiaomi; prefer 6GB/128GB; consider expansion, durability, Gorilla Glass, eSIM, Amazon, Flipkart and impartial reviews. | Built the first shortlist and research report. | Compared Samsung, Motorola, OnePlus, Nothing and Pixel directions. |
| 2026-10-10 | Clarified that Gorilla Glass can be added externally as a screen protector. | Removed built-in Gorilla Glass as a hard requirement and treated it as a bonus. | Added protector/case costs and broadened the shortlist. |
| 2026-10-10 | Start with social proof, then validate with expert reviews; use popularity and rating volume. | Added a social-proof-first purchase strategy. | Recorded rating, review volume, popularity and trade-offs. |
| 2026-10-11 | Preserve evidence across sessions and compare sellers/marketplaces. | Reorganized the work under `mobile-shopping/purchases/mobile-phone/`; created timestamped `evidence.tsv`; added Amazon Bestsellers and Flipkart Popularity sources. | Separate marketplace snapshots can now be compared instead of being merged. |
| 2026-10-11 | Add seller/listing details and summaries of what users liked and disliked. | Added `seller_or_listing` and `user_review_summary` columns. | Qualitative summaries are now explicitly tied to visible review evidence and timestamp. |
| 2026-10-11 | Question whether Galaxy F36 has eSIM; find the minimum-priced eSIM phone that also satisfies the important criteria. | Rechecked model-specific eSIM evidence and separated eSIM-qualified, eSIM-uncertain and non-eSIM options. | F36 should not be counted as eSIM; the lowest practical eSIM direction is an older Pixel 7a around ₹30,000, while the stronger all-round option is Galaxy S24 FE around ₹40,000. |
| 2026-10-11 | Current decision point: determine whether the budget should cross ₹30,000 based on the minimum credible eSIM option. | Keep eSIM as a separate decision gate rather than weakening the other reliability/popularity criteria. | Under ₹25,000: choose a non-eSIM value phone. Around ₹30,000: Pixel 7a is possible but compromised. Around ₹40,000: S24 FE is the first strong all-round eSIM option. |
| 2026-10-11 | Drop eSIM from the requirements and prioritize cost-effectiveness. | Re-ran Amazon/Flipkart value search while keeping stability, popularity, 6–8GB/128GB, warranty, durability and review evidence important. | F36 remains the best all-rounder; Motorola G57 Power is the strongest battery/popularity value; Samsung A17 is the display/protection alternative; Nord CE5 is a strong but stock-limited performance option. |
| 2026-10-11 | Final comparison round with live Flipkart/Amazon snapshots. | Verified stock and prices for F36, G57 Power, A17, CE5; evaluated new candidates A36, M36, M47 against the social-proof gate. | Final pick: F36 Red 6/128 at ₹21,999. Equal-price battery alternative: G57 Power. Potential bargain to verify: M36 Light Green at ₹14,360. Stretch pick: A36 at ₹25,999. Rejected: M47 (3.1 stars), CE5 256GB (overpriced), CE5 8/128 (still out of stock). |

## Current one-line summary

**The process moved from a strict under-₹25k specification search to a social-proof-first, evidence-preserving comparison; built-in Gorilla Glass became optional because a protector can be added, eSIM was tested as a possible budget escalator, and then eSIM was dropped so the decision can return to cost-effective under-₹25k phones.**

## Outstanding questions to confirm

1. Should eSIM be a hard requirement, or only a preference if the price premium is large?
2. Should the search include only new phones, excluding used, renewed and refurbished listings?
3. Is microSD expansion still important if the phone has reliable 128GB storage?
4. Is the target purchase location India-wide, or should delivery/service be checked for a particular city?
