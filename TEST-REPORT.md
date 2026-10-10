# Verification report — 10 October 2026

## Completed

- Retrieved the original public repository's HTML, JavaScript and stylesheet; kept the original tool functions and local-storage key.
- JavaScript syntax checks passed for app.js, manuals.js and sw.js.
- Local HTTP browser preview loaded the finished site with no captured console errors.
- Roster: added a test player with 3 squads, marked ready, and observed attendance 1 / healthy squads 3. Reload preserved these values. Removed test data afterward.
- Command checkbox and notebook text persisted across reload.
- Deadline scenario: elapsed 120, progress 40, entered rate 0.5 yielded 120 minutes remaining, required rate 0.500 and 120 minutes to completion. At elapsed 240, unfinished progress showed the ended window; entered 100% requested official completion verification.
- Item worksheet: expected uses 3 plus buffer 2 yielded a clearly labeled suggested target 5.
- Troop calculator: default healthy 4,700; reserve 1,175; initial commitment 3,525. Setting reserve to 0 yielded commitment 4,700.
- Default HQ/tier produced the flexible support/Battery suggestion.
- Allocation slider changed total from 100 to 101 and displayed the adjustment message.
- Commander tactical rating changed from 3 to 4; total changed from 60 to 66, consistent with its 30% weight.
- CSV export downloaded a file with correct headers and the test player's assignment, squad count and ready status; content inspected.
- JSON plan backup downloaded with both notebook and existing tool state; content inspected. Import restored the original allocation/score/notebook after tool changes.
- Attacker/Defender selector changed the progress objective text correctly.
- Evidence search for teleport returned relevant entries; firsthand filter reduced it to the in-server teleport observation.
- At 390 × 844, document width equaled viewport width (390); no page-level horizontal overflow. Visual inspection found clipped navigation; wrapping was adjusted and rechecked. Desktop view was inspected too.
- Final rendered document had no duplicate IDs and all eight manual sections were present.
- Package integrity: ZIP extracted, file bytes compared with source, relative scripts/styles/manifest checked, and CRC validation passed. ZIP includes no test player data or dependencies.

## Limits

QA used the Codex in-app browser on local HTTP. No broad browser/device matrix, automated accessibility audit or live game mechanic validation was performed. HTTPS service-worker installation/offline fallback and migration from a currently controlling legacy worker were not browser-tested. Evidence is limited to supplied R4 reports and the user's brief; the site labels unresolved mechanics and verification tasks. No GitHub write, push or live deployment occurred.
