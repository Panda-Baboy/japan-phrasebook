PandaBaboy V3.6 FINAL RELEASE CANDIDATE — GitHub Pages upload

Upload ALL files in this ZIP into the ROOT of the existing japan-phrasebook repository, replacing matching files, and commit. Do not upload the ZIP itself as a file.

Changes since V3.6:
- Phrase search now handles multiple terms, Unicode width, accent/romaji variations and missing fields more defensively. Search remains on the Home page.
- Clothing dropdown expanded from 9 to 35 colour choices, with Japanese, kana and romaji.
- Cache version changed to v361 to prompt offline refresh.
- Existing browser storage keys and saved-data logic retained.

Safety: export a data backup from each phone before updating. Browser storage belongs to each device; this package does not sync K and J's data. Do not clear Safari site data or remove the Home Screen app.

Testing status: user reported 44 passing checks in V3.6. Remaining offline, import/merge, packing and other checks were not completed. Code syntax and archive integrity checks are not equivalent to end-to-end iPhone testing.

If search still fails, record the query, expected result, actual result and whether on Home page or another page.
