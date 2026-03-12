# AGENTS.md

## Project goal
Build a stable, polished top-down 2D village RPG inspired by classic Pokemon-style exploration.

The game is about a newcomer learning the local language through teacher-led lessons, practical village quests, and growing relationships with the people in town.

## Working style
Work non-interactively until the game is complete enough to hand off as a playable build.

Do not stop after a first draft.
Do not return control after a partial implementation unless there is a specific blocker.

Treat this as a production handoff, not a prototype pass.

## Core build rules
- Build from scratch only if the current build is beyond repair; otherwise improve the existing code.
- Prefer a simple, stable top-down 2D tile-based architecture over unnecessary complexity.
- Keep the code organized, readable, and commented.
- Prioritize correctness, stability, and playability over flashy extras.
- Do not add combat, monster catching, crafting, or unrelated systems.
- Do not add unnecessary UI clutter.

## Definition of done
The game is done only when all of the following are true:

1. The game launches locally without manual fixes.
2. The player can complete a full run from opening scene to final celebration and credits.
3. All required maps, buildings, NPCs, lessons, quests, signs, items, and endings work.
4. The village is readable and navigable.
5. Paths are not blocked by trees, bushes, furniture, or poor placement.
6. Objects are clearly recognizable and correctly scaled.
7. The backpack/inventory works as specified.
8. Dialogue remains readable and is never hidden by inventory UI.
9. Teacher-only language progression works correctly.
10. Category-based word reveals work correctly.
11. The final build is coherent, stable, and playable.

## Required workflow
1. Plan briefly.
2. Implement the game.
3. Run a full verification pass.
4. Fix all issues found.
5. Re-run verification.
6. Repeat until the acceptance criteria are met or a specific blocker is reached.

## Game structure requirements
The game must be:
- top-down
- 2D
- tile-based
- visually close in structure and readability to classic Pokemon-style village RPGs

The game must include:
- player home
- neighbor home
- nonprofit office
- school
- store
- city hall
- central square with elder
- opening scene
- lesson/quest progression
- backpack icon that opens a simple item list
- item inspection
- map
- dictionary
- celebration ending
- credits

## Narrative rules
The emotional arc is:
confusion -> support -> survival -> confidence -> friendship -> belonging

The ending is not about perfect fluency.
It is about becoming part of the community.

## Language rules
Only the teacher unlocks language.

No passive language unlocking from exploration alone.

When a key word is taught, a whole category may become readable.

Examples:
- bread unlocks food names
- document/card unlocks document names
- place words unlock place signs

Apply language updates consistently across:
- signs
- item names
- dialogue
- documents
- backpack items
- map labels where appropriate

## Inventory rules
Use a backpack icon on the main screen.

Clicking the backpack opens a simple readable inventory list.

No hotbar.

All important items should remain in the backpack permanently unless there is a strong story reason otherwise.

Items should be selectable and inspectable.

Important items include:
- nonprofit card
- map
- dictionary
- bread
- city hall form
- tea cup
- invitation or final keepsake

The backpack UI must never cover critical dialogue text.

## Visual rules
The art should be polished, highly readable, top-down 2D tile-based art inspired by classic Pokemon-style RPGs.

Requirements:
- all important objects must be immediately recognizable
- scaling must be consistent
- paths must be clear
- trees, bushes, benches, flower pots, and signs must not block main routes
- decorative objects belong beside paths, near buildings, or around the square
- buildings must be visually distinct
- signs must be easy to see
- interiors must be logically furnished
- the central square must feel like the heart of the village

## Controls and usability
Include a simple help/controls screen.

Suggested controls:
- arrow keys or WASD to move
- space or enter to interact
- click backpack icon to open inventory
- escape to close open panels

## Verification checklist before returning control
Before returning control, verify all of the following:

- game launches
- opening scene works
- player home tutorial works
- nonprofit encounter works
- map is received
- school can be found
- all teacher lessons trigger correctly
- every post-lesson quest can be completed
- bread/store quest works
- city hall quest works
- neighbor quest works
- elder conversation works
- celebration triggers
- credits display
- backpack opens and items can be inspected
- dialogue remains readable
- signs update correctly
- category unlocks work
- paths are clear
- no major path-blocking objects exist in the village
If a run is interrupted or disconnected, first repair the project to a runnable state before attempting any new feature work.

## Final handoff format
When finished, provide:
1. the final code
2. a short checklist of what was verified
3. any remaining known issues, if any