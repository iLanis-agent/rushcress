# Rushcress 1.0 TEST
Native Android traffic-slider puzzle. Android8+ min26/target35. Package com.gg007.rushcress.

## Rules
Known traffic-slider adaptation. Bring gold X to the right edge of its fixed third-row lane on a 6x6 board. Select a car by tapping any occupied cell, then tap LEFT/RIGHT/UP/DOWN. One button tap moves one cell and counts one move. Cars and trucks occupy two or three cells. Horizontal cars move only left/right; vertical cars only up/down. No rotation, sideways movement, jumping, overlapping or lifting. Other cars remain on the board. Finish when X occupies the two rightmost cells, not by leaving the board. Twelve original generated eight-car layouts, shortest routes 9-18 single-cell moves. Multiple valid routes and final layouts are allowed. Undo/reset, levels and saved palette/car letters; X always stays visible.

## Download and status
https://mega.co.nz/#!hUdwmIgZ!5Nt7Mnlkf6DcIDUu_oPLIQN7mPgjvbfFW7gwWirzE-A
APK 20974 bytes; SHA256 f164cf20934c57c6743d06bcfe2406ab6588dde293942a7153feeff62962104a. Original certificate SHA2561651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. No requested permissions; original GG007 icon unchanged. Anonymous downloaded bytes match.

## Checks
Seed-871110 generator places eight nonoverlapping axis-locked vehicles, then breadth-first search retains twelve different solvable layouts/starts with shortest routes 9-18 single-cell moves. Independent Java oracle uses pairwise rectangle intersection and geometric bounds, separate from production 36-bit occupancy. All 390625 positional arrays per layout plus 120000 random invalid arrays and one null array: 4807501 state/goal comparisons. Across 124676 valid states, 3989632 directional transition checks pass. Independent rectangle-based breadth-first search confirms all twelve shortest route lengths. Bounds, wrong axis, collision, selection/cancel, no-selection and solved locks, undo/replay/reset pass. Actual drawing-adapter car-center selections and direction-button routes solve twelve at their shortest counts; menus/privacy/next/levels/saved palette/car letters/completion pass. Seven drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
All 218 prior studio and 803 legacy descriptions were reviewed. Rejected code-breaking because legacy Mastermind already has it. Railcress is static car-placement deduction from empty-step counts; Latchline is walker-led cargo push/pull; Fifteen swaps single tiles with a vacancy. Rushcress changes the positions of multiple rigid, axis-locked two/three-cell vehicles to transfer free space between intersecting lanes and open a boundary route. No matching factory mechanic found. Known Rush Hour-style adaptation, not globally new. Original generated layouts, program and drawings; no published cards, solver code or source images reused. Six fully read sources span academic game rules and programming problem, rule publisher, mechanical analysis, encyclopedia and developer Q&A. Physical sources use an off-board goal and variable-distance slides, while the programming problem defines single-cell moves and a right-edge finish; this edition explicitly follows the latter. No claim of unique routes or unique final boards.

## Build and tests
JDK17/AndroidSDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/rush-test src/com/gg007/rushcress/Board.java BoardTest.java then java -cp /tmp/rush-test com.gg007.rushcress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your private signing material. No signing secret is included. adapter/android contains the Java2D drawing adapter used with RushAdapterTest.java, not an Android runtime.

## Privacy and branding
Rushcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, car letters and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 menu, original icon, studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative219-card studio and publishing fragments privately preserved:
https://files.instinct.com/msysdkodhinu-rushcress-source-archive
https://github.com/iLanis-agent/rushcress holds README only, full Git source pending. New Jekyll include holds the older top cards unchanged; Rushcress stays in the main index; existing two includes and Pages settings untouched. Both sites verified separately.

## Rule sources
https://gamescrafters.berkeley.edu/games.php?puzzle=rushhour
https://www.ultraboardgames.com/rush-hour/game-rules.php
https://puzzlegenome.org/en/games/rush-hour/
https://en.wikipedia.org/wiki/Rush_Hour_(puzzle)
https://stackoverflow.com/questions/2877724/rush-hour-solving-the-game/2880060
https://db.cs.uni-tuebingen.de/staticfiles/ACM-problems/Rush-Hour.pdf
