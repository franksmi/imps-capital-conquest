# IMPs Capital Conquest — replacement website

Built 10 October 2026. This is a downloadable, buildless static replacement for `franksmi/imps-capital-conquest`. No deployment was performed.

## What is included

- Leader Command Center: multi-day readiness gates, command/deputy handoffs, roles, attacker and defender playbooks, T−60 through T+240 execution, eight contingency decision trees, recovery and debrief.
- Participant Field Guide: personal preparation, role cards, separate attacker/defender action sequences and execution timeline.
- Preserved tools: force allocation, attendance/squad roster, CSV export, commander scoring, HQ/tier role suggestions, troop reserve calculator, command/personal checklists and searchable evidence filters.
- New tools: deadline pace scenario, item-use/buffer worksheet, battle/debrief notebook and JSON backup export/import.
- Responsive styling, keyboard focus indicators, collapsible manuals, relative asset URLs and device-local persistence.

## Evidence and quantities

✓ means firsthand R4 observations supplied by IMPs. These reports were not independently audited and raw screenshots were not supplied. ★ means unresolved mechanics or verification tasks. ◇ means an explicit proposed IMPs process or planning target.

The brief specifies attackers reaching 100% progress within four hours. No 60-minute hold condition is used. The guide asks leaders to check the live event screen and timer before launch. Battery staffing is described as durability; faster firing is unverified. Cross-server escape remains unverified. No fixed shield/item minimum is invented. Item worksheet quantities come from the player's entered expected uses and chosen buffer, not established requirements.

## Upload to GitHub Pages

1. Back up the current repository (Code → Download ZIP) and export any browser plan using the new backup tool when available. Save exports privately; they may contain player names and notes.
2. Extract `imps-capital-conquest-replacement.zip`. The files are at the ZIP root. Upload the extracted files, **not the ZIP**, into the repository's existing publishing folder. Keep `index.html`, `app.js`, `manuals.js`, `styles.css`, `sw.js` and `manifest.webmanifest` together. Include `.nojekyll`; on macOS press Command+Shift+Period to reveal hidden files if needed.
3. Open [franksmi/imps-capital-conquest](https://github.com/franksmi/imps-capital-conquest) → Add file → Upload files. Upload into the same folder as the current `index.html`, replacing the matching filenames. A new branch and pull request offers a reviewable change; merge it when ready. A commit directly to the configured publishing branch will trigger publication if repository rules allow it.
4. In Settings → Pages, retain the existing publishing configuration. For a simple branch-based setup, choose Deploy from a branch, the publishing branch (typically `main`), and `/(root)` when the files are at the repository root. If the site uses `/docs`, place them there. If it uses an existing GitHub Actions workflow, keep that workflow and its expected source folder.
5. Check the Pages deployment in Actions, then open [the site](https://franksmi.github.io/imps-capital-conquest/). Verify the revision date, the Field Guide, evidence search, and a calculator. Publication is complete only when the deployment succeeds and the new content loads.
6. If old content persists, reload after the new service worker activates. Try a hard refresh. Export the plan before clearing site data, because clearing site data also deletes local settings. The new worker removes older `imps-capital-*` caches when activated.

Official instructions: [upload files](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository) and [configure Pages publishing](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## Local use and saved data

No build or external dependency is required. Open `index.html` for a quick local read. For consistent persistence and normal asset/service-worker behavior, serve the folder through a local HTTP server or use GitHub Pages. Existing `imps-capital-v1` tool data is retained on the same browser/origin; new notebook data uses `imps-notebook-v2`. Existing checklist indices retain their meanings. Settings on localhost do not automatically move to GitHub Pages: use Export plan backup and Import backup. Browser profiles/devices do not synchronize. Reset local data clears both tool and notebook state after confirmation. If storage is blocked, export before closing.

The HTTPS service worker provides a cache for visited site assets and uses network-first fetching. Direct-file use does not register it. Offline behavior and live upgrade from the old worker were not exercised in the local HTTP QA.

## Editing and rollback

Edit `manuals.js` for expanded process content and `app.js` for tools/evidence. Styling is in `styles.css`. No personal roster or notebook data is bundled. Restore prior website files with GitHub's revert workflow if needed; browser-local data is separate from repository files.

See TEST-REPORT.md for checks and limits.
