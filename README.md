# Crosscress 1.0 TEST
Native Android Kouchoku crossing-loop puzzle. Android 8+ (min26), target35. Package com.gg007.crosscress. Twelve original unique boards on a 5x5 guide grid.

## Rules
Kouchoku on seven nodes. Tap one node and then another to toggle their straight link; tap the selected node again to cancel. Make one loop visiting every node exactly once. Links can have any slope. All A nodes must be consecutive and all B nodes consecutive, with no blank dot between equal letters. Different letters cannot link directly: travel through at least one unlettered dot between them. Segments may cross only at 90 degrees, away from nodes. Never pass through another node or overlap segments. Straight-through visits at nodes are allowed. Twelve original seven-node layouts on a 5x5 guide grid. Undo/reset, levels and saved loop palette/optional node numbers; letter clues always remain visible. Known Kouchoku adaptation.

## Download and status
https://mega.co.nz/#!xBcASLzT!pMruAqueyg_TgPCEtmS9dgsdsbxgZLtZSS_M2cK3lcY
APK SHA256 ec9418503513fbbcbb5f670cbad20cbbf81554766605f755b467642b0f450773; 20974 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
Portable seed-731110 generator enumerates all 360 undirected Hamiltonian cycles per candidate; twelve different layouts each have exactly one valid loop, five with crossings. Independent oracle uses cycle walking, Java2D Line2D intersection/point tests and squared vector-length identities, while production uses integer orientations, dot products and adjacency checks. All 25,165,824 edge-subset comparisons plus 120,000 random/full-invalid masks agree. Select/cancel, bounds, solved lock, undo/replay/reset pass. Actual drawing-adapter node-pair taps solve all twelve and check menu, privacy, levels, next and saved palette/node numbers/completion. Seven drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 204 live studio descriptions and the current 803-entry web registry for Kouchoku, perpendicular crossings and letter-run constraints. No functional match. Anglewren chooses a noncrossing polygon with acute/right/obtuse angle clues; Crosscress instead permits right-angle crossings and constrains consecutive equal-letter groups, with blank nodes separating different letters and no angle requirement at nodes. Linkcress makes disjoint white/black pairs rather than one loop. Known Kouchoku adaptation; original generated layouts, code and visuals, not a global invention. Six supporting pages cover independent rules/setters, academic context, a variant rulebook and the Angle Loop comparison; no source layout/code/art copied. Alternating-movement variant rules are not used.
Rules https://carrick22spuzzles.blogspot.com/2024/01/kouchoku.html ; independent rules https://logic-masters.de/Raetselportal/Raetsel/zeigen.php?chlang=en&id=000BQ2 .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/crosscress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.crosscress.CrossBoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Crosscress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Loop palette, optional node numbers and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 205-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/3fczn8ony4vy-crosscress-source-archive . Repository https://github.com/iLanis-agent/crosscress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
