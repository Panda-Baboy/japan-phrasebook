🐼🐷 PandaBaboy V3.8.0 — Japan Ready
Final pre-trip source package • 13 November 2026

HOW TO DEPLOY
1. Before updating, open PandaBaboy on BOTH iPhones while online. Verify that each says "☁️ Up to date". If sync is pending or shows an error, do NOT proceed blindly.
2. Export a backup from each phone (More → Backup & offline check). Save both JSON files privately in Files/iCloud Drive. They can contain hotel addresses and other personal trip details.
3. In GitHub's japan-phrasebook repository on branch main, replace/upload ALL files from the root of THIS ZIP (not the ZIP itself, and not in a subfolder). Keep the filename index.html at repo root. Do not clear Cloud Firestore, Safari website data, or uninstall the old PWA.
4. Open the published site on both iPhones with an Internet connection and refresh so the new service worker can cache the files.
5. Confirm the new V3.8.0 heading, open the Home page and one phrase, then check that your purchases/wardrobe/packing entries are still present. Test the Airplane Mode reload on each phone where practical.
6. If you see a sync conflict warning, stop editing the affected section on the second phone. Both phones have a local copy; export both backups and reconcile, rather than resetting or replacing cloud data.

WHAT'S NEW
- Cleaner Home; bottom Home/Phrases/Trip/Shop/More nav; emergency accessible from every screen.
- Phrasebook categories include Pokémon Center & Cards (35 previously hidden phrases).
- Learning Lab: eight Trip Japanese lessons + optional Japanese Foundations lessons, linked to existing flashcards, quiz and practice pages.
- 24 hand-curated new phrases for tax refund, customs, airport, shopping, hotel, medical help and travel; original 595 entries remain in identical order to keep numeric favourites valid.
- Hotel & travel address cards (Japanese/English address, notes, phone; show/copy/maps).
- Day-trip checklists, independent of K/J suitcase checkmarks; copy essentials, reset and duplicate.
- Daily outfits: compact final look on top and separate edit selection, plus 14 November departure date.
- Japan's tax-refund rules revised for purchases from 1 Nov 2026, sourced from Japan Customs / Japan Tourism Agency.
- Dark-mode readability fixes for How-to guide, staff replies, cards and controls; mobile touch targets and safe-area bottom navigation.
- New full JSON export and conservative merge import, preserving current wardrobe positions and existing outfits when dates overlap.
- Firebase sync protection: preserves other profile (K/J) when saving personal learning progress, journals local changes before sign-in readiness, and blocks potentially conflicting wardrobe/outfit/checklist/hotel edits rather than silently overwriting them.
- Updated offline precache with all local V3.8.0 files.

TESTS COMPLETED
- All 10 JavaScript files: node --check passed.
- All 619 standalone phrases and all 99 staff phrase structures: nonempty English/Japanese/kana/romaji; 247 replies present with those fields.
- Confirmed baseline 595 phrases retained byte-for-byte equivalent JSON values in original order.
- Mocked functional smoke tests: 12 primary views, two lesson views, K/J sync profile preservation, standalone wardrobe update and conflict prevention all pass.
- Static dependency audit: all 15 local HTML references exist; offline cache list includes new assets.
- Calculated contrast for new How-to guide text: dark 12.62:1; light 8.13:1.
- ZIP archive validation and package manifest completed.

NOT TESTED LIVE
- Managed browser policy prevented live localhost visual automation; no live iPhone/Safari or two-phone Firebase sign-in test was possible in this environment.
- This cannot certify that every translation in the original 595 phrases or the 247 existing staff replies is perfectly natural; structural checks and targeted phrase review were performed.
- Offline Japanese voice playback depends on installed Japanese voices on the device.
- Concurrent edits to the SAME record on two phones still require coordination. The new guard prevents blind overwriting for key structured sections, but is not a general real-time conflict resolver.

NO SERVER-SIDE CHANGES
- No Firestore project/rules or existing cloud records were changed to build this package.
- This ZIP is a SOURCE PACKAGE. It has NOT been deployed to GitHub for you.

PRIVACY
- Hotel cards and backups can contain personal addresses. Do not upload backup JSON files to the public GitHub repo.
- Do not store passport numbers, card numbers or passwords in hotel notes.

Official references:
Japan Customs: https://www.customs.go.jp/kaigairyoko/taxrefund.htm
Japan Tourism Agency: https://www.mlit.go.jp/kankocho/tax-free/page01_000001_00028.html
Japan Visitor Hotline: https://faq.japan-travel.jnto.go.jp/en/plan/hotline/
