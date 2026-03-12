---
name: pokemon-newcomer-rpg-builder
description: Build and finish a polished top-down 2D Pokemon-style village RPG about a newcomer learning the local language through teacher-led lessons, practical quests, and community relationships.
---

# Purpose
Use this skill when the task is to build, repair, complete, or significantly improve the newcomer language-learning village game.

This skill is specifically for a:
- top-down
- 2D
- tile-based
- Pokemon-style exploration game
- with strong narrative progression
- teacher-led language lessons
- practical quests between lessons
- backpack-based item inspection
- celebration ending

# When to use this skill
Use this skill when the user asks for:
- a build from scratch of the language-learning village game
- major repairs to the existing game
- a polished final version instead of a prototype
- narrative or quest restructuring
- clearer visual readability and map design
- inventory/backpack improvements
- teacher-only language progression
- category-based word reveal logic

# Non-goals
Do not add:
- combat
- monster catching
- crafting
- unnecessary minigames
- unrelated systems
- overcomplicated UI

# Core gameplay structure
The game should include:
- player home
- neighbor home
- nonprofit office
- school
- store
- city hall
- central square with elder
- clear outdoor village map
- interiors for all major buildings
- opening scene
- dialogue system
- quest system
- inventory system
- celebration scene
- credits

# Narrative arc
The emotional arc is:
confusion -> support -> survival -> confidence -> friendship -> belonging

The player is a newcomer.
They begin safe but disoriented.
They receive their first support at the nonprofit.
The teacher leads all language progression.
The player uses each lesson to complete a practical quest.
By the end, the elder recognizes their growth and invites them to a celebration.

# Language progression rules
Only the teacher unlocks language.

No passive language learning through walking around.

When the teacher teaches a key word, a whole category may become readable.

Examples:
- bread unlocks food names
- card/document unlocks document names
- place words unlock place signs
- social words unlock more social dialogue

Apply language changes consistently across:
- signs
- dialogue
- inventory item names
- item descriptions
- documents
- map labels where appropriate

# Recommended lesson structure
Use this six-lesson progression unless the user specifies otherwise.

## Lesson 1: greetings and help
Teach:
- hello
- yes
- no
- help
- thank you

Quest:
- return to nonprofit
- greet the Program Specialist
- identify the nonprofit sign

## Lesson 2: food
Teach:
- bread
- water
- tea
- food

Category unlock:
- all food names

Quest:
- go to store
- choose bread
- add bread to backpack

## Lesson 3: places and directions
Teach:
- school
- store
- city hall
- road
- here
- there

Category unlock:
- place names and signs

Quest:
- navigate using signs

## Lesson 4: documents and forms
Teach:
- paper
- card
- name
- write
- form

Category unlock:
- all document names

Quest:
- go to city hall
- identify the correct form or desk
- complete simple civic interaction

## Lesson 5: home and social language
Teach:
- home
- neighbor
- tea
- come in
- friend

Quest:
- visit neighbor
- share tea
- receive tea cup

## Lesson 6: community and belonging
Teach:
- community
- together
- celebration
- today
- welcome

Quest:
- speak to elder in town square
- receive invitation to celebration

# Inventory rules
Use a simple backpack icon on the main screen.

When clicked, it should open a readable item list.

No hotbar.

The backpack should contain meaningful objects collected across the story:
- nonprofit card
- map
- dictionary
- bread
- city hall form
- tea cup
- invitation or final keepsake

Each item should:
- remain available
- be selectable
- be inspectable
- show a clear name
- show a description
- update readability when relevant language categories are unlocked

The backpack must not hide dialogue text.

# Visual standards
Use a top-down 2D tile-based style inspired by classic Pokemon-style RPGs.

## Tile and sprite standards
- prefer a 32x32 tile grid
- use consistent sprite scale
- use 4-direction character sprites
- make buildings visually distinct
- make objects immediately recognizable
- keep paths clear and readable
- place trees and bushes beside paths, not in the middle of them
- keep interiors logically furnished
- ensure important quest objects stand out clearly

## Object readability
The player should never need to guess what an important object is.

Examples:
- bed must look like a bed
- bread must look like bread
- map must look like a map
- dictionary must look like a book
- tea cup must look like a tea cup
- sign must look like a sign

# NPC roles
Use these roles consistently:
- Program Specialist: first support
- Teacher: only source of language progression
- Shopkeeper: practical language test
- Neighbor: warmth and hospitality
- City Hall Clerk: formal system becomes manageable
- Elder: final recognition and celebration invitation

# Dialogue rules
Dialogue should be:
- warm
- short enough to read comfortably
- emotionally grounded
- progressively clearer as lessons are learned

Do not make NPCs feel like exposition machines.

# Ending rules
The elder is the final major conversation.

The elder invites the player to a celebration in the central square.

The celebration includes all major NPCs.

After the celebration, show credits with reflective text about:
- arriving as a newcomer
- learning the language
- receiving help
- making friends
- becoming part of the community

Final screen should show the player together with the townspeople.

# Build and verification behavior
Work non-interactively until the game is playable from start to finish.

Do not stop after a first draft.

Follow this loop:
1. plan briefly
2. implement
3. run a full verification pass
4. fix issues
5. verify again
6. repeat until stable

Before returning control, verify:
- full playable run works
- all lesson and quest steps work
- backpack works
- signs update correctly
- dialogue stays readable
- paths are clear
- celebration and credits work

# Output expectations
When done, return:
1. final code
2. brief verification checklist
3. remaining known issues, if any