# Spanish Dialogue Guide for Newcomer Game

## Purpose

This file is the exact source of truth for the game’s:
- story arc
- lesson structure
- dialogue tree
- character identities
- character voices
- character visual presentation
- bilingual display rules
- bilingual voice parsing rules
- internal thought rules
- practice vs test rules

Codex should treat this file as the exact dialogue and content spec.
It should not improvise new dialogue when this file already provides exact phrasing.

---

# Source of Truth Rules

## 1. This file is exact
This file contains:
- exact story logic
- exact lesson order
- exact scene flow
- exact dialogue wording
- exact voice behavior
- exact character presentation rules

If this file gives exact dialogue, Codex should implement that dialogue exactly.

## 2. Preserve the current game
This file is not a command to redesign the game.

The current game’s:
- map
- controls
- movement
- music
- general art style
- backpack structure
- overall UI layout

should be preserved unless a specific logic or dialogue update requires a very small technical change.

## 3. Practice vs test
This is one of the most important rules in the game.

### Allison
Allison is the formal teacher.
She teaches, explains, reviews, and tests.

### Everyone else
Kate, Alyssa, Cameron, Supriya, Gwendolyn, Joe, Evan, and Nancy are for **practice conversations**, not formal tests.

That means:
- Zach chooses plausible response lines
- the NPC replies naturally
- the scene should feel like conversation practice
- it should not feel like a quiz app

## 4. Internal thoughts
Internal thoughts belong only to Zach.

Internal thoughts must:
- appear in *italics*
- be silent
- never be spoken aloud
- never appear under another character’s name

If an italic line is Zach’s thought, it must be displayed as Zach’s internal thought, not as Kate’s or anyone else’s dialogue.

---

# Character Specs

## Zach
- Role: player character
- Gender presentation: male-presenting
- Voice gender: male
- English voice: male English browser voice
- Spanish voice: male Spanish browser voice
- Tone: thoughtful, cautious at first, gradually more confident

## Kate
- Role: Global Cleveland worker
- Gender presentation: female-presenting
- Voice gender: female
- English voice: female English browser voice
- Spanish voice: female Spanish browser voice
- Tone: warm, calm, practical, reassuring

## Allison
- Role: teacher
- Gender presentation: female-presenting
- Voice gender: female
- English voice: female English browser voice
- Spanish voice: female Spanish browser voice
- Tone: patient, practical, encouraging, clear, natural

## Alyssa
- Role: shopkeeper
- Gender presentation: female-presenting
- Voice gender: female
- English voice: female English browser voice
- Spanish voice: female Spanish browser voice
- Tone: brisk, competent, practical, helpful

## Cameron
- Role: city hall helper
- Gender presentation: male-presenting
- Voice gender: male
- English voice: male English browser voice
- Spanish voice: male Spanish browser voice
- Tone: formal, readable, welcoming, steady

## Supriya
- Role: clinic staff / doctor
- Gender presentation: female-presenting
- Voice gender: female
- English voice: female English browser voice
- Spanish voice: female Spanish browser voice
- Tone: calm, caring, efficient

## Joe
- Role: elder
- Gender presentation: male-presenting
- Voice gender: male
- English voice: male English browser voice
- Spanish voice: male Spanish browser voice
- Tone: observant, kind, calm, understated

## Evan
- Role: neighbor
- Gender presentation: male-presenting
- Voice gender: male
- English voice: male English browser voice
- Spanish voice: male Spanish browser voice
- Tone: friendly, grounded, local

## Nancy
- Role: villager
- Gender presentation: female-presenting
- Voice gender: female
- English voice: female English browser voice
- Spanish voice: female Spanish browser voice
- Tone: warm, casual, friendly

## Gwendolyn
- Role: warm local host / friendly community member
- Gender presentation: female-presenting
- Voice gender: female
- English voice: female English browser voice
- Spanish voice: female Spanish browser voice
- Tone: welcoming, gentle, thoughtful, socially warm

---

# Optional Voice Variation Rule

If browser voices allow for it, different English female voices may be assigned to different women for flavor, as long as:
1. the correct language is always respected
2. the correct gender is respected
3. the character stays consistent during the session

Example:
- Kate may use a British English female voice if available
- Allison may use a different English female voice
- Alyssa, Supriya, Nancy, and Gwendolyn may also use distinct female English voices if available

The same principle may apply to Spanish voices if multiple suitable female Spanish voices are available.

---

# Adaptation Progress

The progress bar should be called:

**Adaptation Progress Bar**

Not “language progress.”

This game is about:
- comfort
- orientation
- confidence
- participation
- belonging

---

# Sign and Building Rules

## Signs
Do not use `???`.

All major location signs should be visible in Spanish from the start:
- GLOBAL CLEVELAND
- ESCUELA
- TIENDA
- AYUNTAMIENTO
- CLÍNICA

After the corresponding lesson, English can appear in parentheses:
- ESCUELA (School)
- TIENDA (Store)
- AYUNTAMIENTO (City Hall)
- CLÍNICA (Clinic)

Spanish remains primary.

## Locked buildings
Buildings may remain locked by quest state.

If Zach reaches a locked building too early, use only neutral lines like:
- “I can’t go in here yet.”
- “It’s not time to go here yet.”
- “I should finish my current task first.”

Do not reveal what the building is through the lock text.

---

# Door Rule

If the game uses a door portal tile:
- the trigger should be exactly **one tile directly in front of the door**
- not offset oddly
- not too low
- not to the side

Preserve current visuals.

---

# Bilingual Display and Voice Rules

These rules are extremely important.

## 1. Two dialogue modes

### Lesson Mode
Use for Allison’s classroom scenes.

In Lesson Mode:
- Spanish teaching phrase is spoken aloud in the correct Spanish voice
- English explanation is spoken aloud in the correct English voice
- mixed lines must be split into language segments exactly
- on-screen text may show both Spanish and English

### Conversation Practice Mode
Use for all non-teacher conversations.

In Conversation Practice Mode:
- NPC speaks in Spanish
- English translation appears on screen in parentheses
- the English translation is **not voiced**
- Zach’s selected response is spoken in Spanish if the response is in Spanish
- this keeps town conversations cleaner and more natural

## 2. Entire English lines
If a line is fully English:
- it must be spoken entirely in the correct gendered English browser voice

Example:
- “Let’s start with a few phrases you can use right away.”
  - Allison = female English voice

## 3. Entire Spanish lines
If a line is fully Spanish:
- it must be spoken entirely in the correct gendered Spanish browser voice

Example:
- “Buenos días.”
  - Allison = female Spanish voice

## 4. Mixed lesson lines
If a teaching line contains both Spanish and English, it must be split by language segment.

Example:
- hola means hello

Speech:
1. hola -> Spanish female Allison voice
2. means hello -> English female Allison voice

Example:
- “sí” means “yes”

Speech:
1. sí -> Spanish female Allison voice
2. means yes -> English female Allison voice

Example:
- “no” means “no”

Speech:
1. first “no” in quotes -> Spanish female Allison voice
2. means -> English female Allison voice
3. second “no” in quotes or English explanation -> English female Allison voice if it is the English word no

## 5. Quoted Spanish words are still Spanish
Words in quotes are still Spanish if they are Spanish words:
- “sí”
- “no”
- “hola”
- “gracias”
- “buenos días”
- “buenas tardes”
- “por favor”

These must be spoken in the Spanish voice.

## 6. Parenthetical translations
In classroom teaching:
- Spanish phrase may be voiced in Spanish
- English translation may be voiced in English

In normal town conversations:
- Spanish line is voiced in Spanish
- English translation in parentheses is shown on screen only
- English translation is not voiced

Example:
- Ve con calma. Ella te va a entender. (Go slowly. She will understand you.)
  - Spanish part voiced in Spanish
  - English parentheses shown silently

## 7. Proper nouns and mixed tokens
Do not assign language voice by naive token guessing.

Examples:
- “Global Cleveland” is an English proper noun and should not be split into random Spanish/English voice tokens
- single letters like “a” should not be automatically read in Spanish voice unless they are truly part of a Spanish segment

Voice parsing should happen by **authored language segment**, not by isolated token guesswork.

### 8A. Zach’s on-screen Spanish and English in conversation scenes

In normal conversation practice scenes, when Zach selects a Spanish response:

- the Spanish line must appear on screen
- the English translation must also appear on screen in parentheses
- the Spanish line should be spoken aloud in Zach’s Spanish male voice
- the English translation should not be spoken aloud during normal conversations

Example:

Spoken:
- Necesito ayuda con un documento.

On-screen:
- Necesito ayuda con un documento.
- (I need help with a document.)

This rule should apply in conversation scenes with:
- Kate
- Alyssa
- Cameron
- Supriya
- Gwendolyn
- Joe
- Evan
- Nancy

This keeps Zach’s dialogue fully readable:
- the player sees the Spanish
- the player sees the English support
- the player hears the Spanish
- the voice system does not awkwardly read both languages in ordinary town conversations

Exception:
In Allison’s classroom lesson mode, mixed Spanish + English instructional lines may still be spoken in both languages as part of teaching.

## 8B. NPC on-screen Spanish and English in conversation scenes

In normal conversation practice scenes, when an NPC speaks a Spanish line:

- the Spanish line must appear on screen
- the English translation must also appear on screen in parentheses
- the Spanish line should be spoken aloud in the NPC’s Spanish voice
- the English translation should not be spoken aloud during normal conversations

Example:

Spoken:
- Bienvenido al pueblo.

On-screen:
- Bienvenido al pueblo.
- (Welcome to town.)

This rule should apply to:
- Kate
- Alyssa
- Cameron
- Supriya
- Gwendolyn
- Joe
- Evan
- Nancy

This ensures that normal town conversations consistently show:
- Spanish text on screen
- English support on screen
- Spanish spoken aloud
- no awkward double-voicing of the English translation

## 9. Voice priority
Voice selection priority:
1. correct language
2. correct gender
3. stable consistency for the character

## 10. Voice speed
If possible, the settings menu should include a **voice speed slider** that changes browser speech playback rate.

---

# Full Story Arc

There are **5 lessons total**.

Each lesson includes:
1. Allison classroom scene
2. review or test
3. practice element
4. mini quest or quest chain
5. emotional beat

The five lessons are:

1. Welcome phrases and introductions
2. Places and directions
3. Store and daily needs
4. Documents and medical care
5. Invitation phrases and belonging

---

# Opening Scene

## Opening card
Display on screen:

“You are Zach.  
You are new here.  
You do not know the town yet.  
You do not know the language well.  
But you have one note, a few belongings, and one place to start.”

## Internal thought
*I’m new here. I don’t know the town yet, and I barely know the language. But I have to start somewhere.*

## First task
“Open your backpack and read the note.”

---

# Scene: Kate at Global Cleveland

## Exact dialogue

### Kate
**Spoken EN-F Kate**  
“Hi there. You look a little lost.”

### Zach choices
1. “Hi.”
2. “I’m new here.”
3. “I need help.”

### Kate response
If 2 or 3:
**Spoken EN-F Kate**  
“That’s okay. You came to the right place.”

**Spoken EN-F Kate**  
“My name is Kate. I work here at Global Cleveland.”

**Spoken EN-F Kate**  
“We help people get settled, find resources, and figure out where to start.”

**Spoken EN-F Kate**  
“I’m going to give you a map.”

**Spoken EN-F Kate**  
“But first, I want you to go to school and learn a few phrases you can use right away.”

**Spoken EN-F Kate**  
“Then come back and try them with me.”

**Spoken EN-F Kate**  
“And later, once you start getting your documents together, I want you to come back and tell me how it goes.”

**Spoken EN-F Kate**  
“Good luck. I’ll be here when you get back.”

---

# LESSON 1 — Welcome Phrases and Introductions

## Allison opening
**Spoken EN-F Allison**  
“Welcome, Zach.”

**Spoken EN-F Allison**  
“Kate told me you’d be visiting.”

**Spoken EN-F Allison**  
“I’m glad you made it here.”

**Spoken EN-F Allison**  
“Let’s start with a few phrases you can use right away.”

**Spoken EN-F Allison**  
“You don’t need many words to begin.”

**Spoken EN-F Allison**  
“A greeting, a thank you, and a simple introduction can take you a long way.”

## Taught phrases
These must all be explicitly taught before the test.

### 1
**Spoken ES-F Allison**  
“Hola.”

**Spoken EN-F Allison**  
“That means hello.”

**On-screen**  
hola — hello

### 2
**Spoken ES-F Allison**  
“Buenos días.”

**Spoken EN-F Allison**  
“That means good morning.”

**On-screen**  
buenos días — good morning

### 3
**Spoken ES-F Allison**  
“Buenas tardes.”

**Spoken EN-F Allison**  
“That means good afternoon.”

**On-screen**  
buenas tardes — good afternoon

### 4
**Spoken ES-F Allison**  
“Gracias.”

**Spoken EN-F Allison**  
“That means thank you.”

**On-screen**  
gracias — thank you

### 5
**Spoken ES-F Allison**  
“Sí.”

**Spoken EN-F Allison**  
“That means yes.”

**On-screen**  
sí — yes

### 6
**Spoken ES-F Allison**  
“No.”

**Spoken EN-F Allison**  
“That means no.”

**On-screen**  
no — no

### 7
**Spoken ES-F Allison**  
“Por favor.”

**Spoken EN-F Allison**  
“That means please.”

**On-screen**  
por favor — please

### 8
**Spoken ES-F Allison**  
“Necesito ayuda.”

**Spoken EN-F Allison**  
“That means I need help.”

**On-screen**  
necesito ayuda — I need help

### 9
**Spoken ES-F Allison**  
“Me llamo Zach.”

**Spoken EN-F Allison**  
“That means my name is Zach.”

**On-screen**  
me llamo Zach — my name is Zach

### 10
**Spoken ES-F Allison**  
“¿Cómo te llamas?”

**Spoken EN-F Allison**  
“That means what is your name?”

**On-screen**  
¿cómo te llamas? — what is your name?

### 11
**Spoken ES-F Allison**  
“Mucho gusto.”

**Spoken EN-F Allison**  
“That means nice to meet you.”

**On-screen**  
mucho gusto — nice to meet you

## Lesson 1 test
Examples of exact natural prompts:
- Which phrase means good morning?
- How do you say thank you?
- How do you say my name is Zach?
- How do you ask someone what their name is?
- Which phrase means I need help?
- How do you say yes?
- How do you say no?
- Which phrase would you use in the afternoon?
- How do you politely say please?
- Which phrase means nice to meet you?

## Allison closing
**Spoken ES-F Allison**  
“Muy bien.”

**Spoken EN-F Allison**  
“Now let’s use those words with real people.”

**Spoken EN-F Allison**  
“First, go back to Kate and try a few of these phrases with her.”

**Spoken EN-F Allison**  
“Then introduce yourself to one of your neighbors.”

**Spoken EN-F Allison**  
“You do not need a long conversation. Just say hello, say your name, and ask theirs.”

---

# Scene: Kate practice conversation

This is **practice**, not a test.

## Kate opening
**Spoken ES-F Kate**  
“Hola, Zach.”  
**On-screen translation**  
(Hello, Zach.)

## Zach choice
1. **Spoken ES-M Zach** “Hola, Kate.”
2. **Spoken ES-M Zach** “Buenos días.”
3. **Spoken ES-M Zach** “Buenas tardes.”

## Kate response examples
If 1:
**Spoken ES-F Kate**  
“Hola. Qué bueno verte otra vez.”  
**On-screen translation**  
(Hello. It’s good to see you again.)

If 2:
**Spoken ES-F Kate**  
“Buenos días. Suena bien.”  
**On-screen translation**  
(Good morning. That sounds good.)

If 3:
**Spoken ES-F Kate**  
“Buenas tardes. Muy bien.”  
**On-screen translation**  
(Good afternoon. Very good.)

## Kate follow-up
**Spoken ES-F Kate**  
“¿Cómo estás?”  
**On-screen translation**  
(How are you?)

## Zach choice
1. **Spoken ES-M Zach** “Bien, gracias.”
2. **Spoken ES-M Zach** “Estoy un poco nervioso.”
3. **Spoken ES-M Zach** “Necesito ayuda.”

## Kate response
**Spoken ES-F Kate**  
“No pasa nada. Poco a poco.”  
**On-screen translation**  
(It’s okay. Little by little.)

**Spoken ES-F Kate**  
“Ya suenas más seguro.”  
**On-screen translation**  
(You already sound more confident.)

**Spoken EN-F Kate**  
“When you’re ready, try introducing yourself to one of your neighbors too.”

**Spoken EN-F Kate**  
“You don’t need to say much. Just enough to begin.”

**Spoken EN-F Kate**  
“Good luck. I’ll see you again.”

## Internal thought
*That felt better than I expected.*  
*Maybe I really can do this one step at a time.*

---

# Mini Quest — Introduce yourself to Gwendolyn

## Gwendolyn first meeting
**Spoken ES-F Gwendolyn**  
“Hola.”  
**On-screen translation**  
(Hello.)

## Zach choice
1. **Spoken ES-M Zach** “Hola.”
2. **Spoken ES-M Zach** “Buenos días.”
3. **Spoken ES-M Zach** “Buenas tardes.”

## Gwendolyn
**Spoken ES-F Gwendolyn**  
“¿Cómo te llamas?”  
**On-screen translation**  
(What is your name?)

## Zach choice
1. **Spoken ES-M Zach** “Me llamo Zach.”
2. **Spoken ES-M Zach** “Soy Zach.”

## Gwendolyn
**Spoken ES-F Gwendolyn**  
“Mucho gusto. Me llamo Gwendolyn.”  
**On-screen translation**  
(Nice to meet you. My name is Gwendolyn.)

## Zach choice
1. **Spoken ES-M Zach** “Mucho gusto.”
2. **Spoken ES-M Zach** “Gracias.”

## Gwendolyn close
**Spoken ES-F Gwendolyn**  
“Bienvenido.”  
**On-screen translation**  
(Welcome.)

**Spoken ES-F Gwendolyn**  
“Nos vemos por el barrio.”  
**On-screen translation**  
(I’ll see you around the neighborhood.)

## Internal thought
*That was short, but it mattered.*  
*I introduced myself to someone for the first time.*

---

# LESSON 2 — Places and Directions

## Allison opening
**Spoken EN-F Allison**  
“You came back.”

**Spoken EN-F Allison**  
“And you really used the phrases.”

**Spoken EN-F Allison**  
“I knew you could do it.”

**Spoken EN-F Allison**  
“Now let’s make the town itself easier to understand.”

## Part 1 — Places
**Spoken EN-F Allison**  
“Let’s start with places.”

**Spoken EN-F Allison**  
“Before you can ask where something is, you need to know what it’s called.”

Teach:
- escuela — school
- tienda — store
- ayuntamiento — city hall
- clínica — clinic
- plaza — square

## Part 2 — Directions
**Spoken EN-F Allison**  
“Good. Now directions.”

**Spoken EN-F Allison**  
“Knowing the places helps, but you also need to know how to move through town.”

Teach:
- arriba — up
- abajo — down
- izquierda — left
- derecha — right
- aquí — here
- allí — there
- arriba de — above
- abajo de — below
- a la izquierda de — to the left of
- a la derecha de — to the right of
- ¿Dónde está...? — Where is...?

## Example sentences
Each of these should be spoken in female Spanish voice first, then female English voice.

- La tienda está abajo de Global Cleveland. — The store is below Global Cleveland.
- La clínica está a la derecha de la escuela. — The clinic is to the right of the school.
- El ayuntamiento está arriba de la plaza. — City hall is above the square.
- La escuela está a la izquierda de la clínica. — The school is to the left of the clinic.

## Exact natural questions
- How do you say “here” in Spanish?
- How do you say “there” in Spanish?
- If you need to ask where something is, how would you start your question?
- Which word means left?
- Which word means down?
- Which sentence says the clinic is to the right of the school?
- Which phrase means below?
- Which word means square?
- Which word means city hall?
- Which sentence says the school is to the left of the clinic?

## Allison closing
**Spoken ES-F Allison**  
“Muy bien.”

**Spoken EN-F Allison**  
“Now go out into town and read the signs.”

**Spoken EN-F Allison**  
“Then come back and we’ll keep going.”

---

# Sign-reading Quest

Zach reads:
- GLOBAL CLEVELAND
- ESCUELA
- TIENDA
- AYUNTAMIENTO
- CLÍNICA

After lesson completion, English can appear in parentheses.

## Internal thought
*I’m starting to recognize these places.*  
*I feel more oriented now.*

---

# LESSON 3 — Store and Daily Needs

## Allison opening
**Spoken EN-F Allison**  
“You did well.”

**Spoken EN-F Allison**  
“You found the signs and paid attention to where things are.”

**Spoken EN-F Allison**  
“That’s going to help.”

**Spoken EN-F Allison**  
“Now let’s work on daily needs.”

## Teach these words
All quoted Spanish words must be female Spanish voice.
All English explanations must be female English voice.

- pan — bread
- agua — water
- leche — milk
- arroz — rice
- fruta — fruit
- verduras — vegetables
- té — tea
- queso — cheese
- huevos — eggs
- comida — food
- quiero — I want
- por favor — please

## Important order
1. Teach the food words
2. Test the food words
3. Tell Zach a grocery list is going into his bag
4. Zach checks the grocery list after class

## Exact natural questions
- How do you say bread?
- How do you say water?
- How do you say fruit?
- How do you ask for things politely in the store?
- Which word means cheese?
- Which word means rice?
- How do you say tea?
- Which phrase means I want?
- Which word means vegetables?
- Which word means eggs?

## Allison closing
**Spoken ES-F Allison**  
“Muy bien.”

**Spoken EN-F Allison**  
“Now I’m putting a grocery list in your bag.”

**Spoken EN-F Allison**  
“Look at it before you leave.”

**Spoken EN-F Allison**  
“Then go into town, ask someone where the store is, and do your shopping.”

## Grocery list
- pan
- agua
- fruta

---

# Mini Quest — Ask for directions to the store

Joe or Nancy can answer, but Zach must ask first.

## Example with Nancy

**Spoken ES-F Nancy**  
“Hola.”  
**On-screen translation**  
(Hello.)

## Zach choice
1. **Spoken ES-M Zach** “Hola.”
2. **Spoken ES-M Zach** “Buenos días.”
3. **Spoken ES-M Zach** “¿Dónde está la tienda?”

If 3:
**Spoken ES-F Nancy**  
“La tienda está abajo de Global Cleveland.”  
**On-screen translation**  
(The store is below Global Cleveland.)

**Spoken ES-F Nancy**  
“Luego, un poco a la derecha.”  
**On-screen translation**  
(Then, a little to the right.)

**Spoken ES-F Nancy**  
“Que tengas buen día.”  
**On-screen translation**  
(Have a good day.)

## Internal thought
*Wow. I got over some of my fear.*  
*I asked for directions for the first time.*

---

# Scene — Alyssa at the store

This is conversation practice, not a quiz.

## Alyssa opening
**Spoken ES-F Alyssa**  
“Hola. ¿Cómo estás?”  
**On-screen translation**  
(Hello. How are you?)

## Zach choice
1. **Spoken ES-M Zach** “Bien, gracias.”
2. **Spoken ES-M Zach** “Un poco nervioso.”
3. **Spoken ES-M Zach** “Bien. ¿Y tú?”

## Alyssa
**Spoken ES-F Alyssa**  
“¿En qué te ayudo?”  
**On-screen translation**  
(How can I help you?)

## Zach choice
1. **Spoken ES-M Zach** “Tengo una lista.”
2. **Spoken ES-M Zach** “Quiero comprar comida.”
3. **Spoken ES-M Zach** “Necesito pan.”

Best flow:
1

## Alyssa
**Spoken ES-F Alyssa**  
“Muy bien. Vamos con calma.”  
**On-screen translation**  
(Very good. We’ll go slowly.)

## Internal thought
*Okay. I need to tell her what I want.*

### Item 1
**Spoken ES-M Zach**  
“Quiero pan, por favor.”

**Spoken ES-F Alyssa**  
“Sí. Aquí tienes.”  
**On-screen translation**  
(Yes. Here you go.)

### Item 2
**Spoken ES-M Zach**  
“Quiero agua, por favor.”

**Spoken ES-F Alyssa**  
“Claro.”  
**On-screen translation**  
(Of course.)

### Item 3
**Spoken ES-M Zach**  
“Quiero fruta, por favor.”

**Spoken ES-F Alyssa**  
“Muy bien.”  
**On-screen translation**  
(Very good.)

## Alyssa closing
**Spoken ES-F Alyssa**  
“Lo hiciste bien.”  
**On-screen translation**  
(You did well.)

**Spoken ES-F Alyssa**  
“Gracias. Vuelve pronto.”  
**On-screen translation**  
(Thank you. Come back soon.)

## Internal thought
*I did that on my own.*  
*I’m feeling more confident.*

---

# LESSON 4 — Documents and Medical Care

## Allison opening
**Spoken EN-F Allison**  
“You handled that well.”

**Spoken EN-F Allison**  
“You asked for directions, found the store, and bought what you needed.”

**Spoken EN-F Allison**  
“That’s a real step forward.”

**Spoken EN-F Allison**  
“Now let’s work on forms, appointments, and getting help.”

**Spoken EN-F Allison**  
“Sometimes one place sends you somewhere else first.”

**Spoken EN-F Allison**  
“That can be frustrating, but it’s normal.”

**Spoken EN-F Allison**  
“Today we’re learning the language that helps you get through that.”

## Teach these words and phrases
- documento — document
- papel — paper
- formulario — form
- firma — signature
- nombre — name
- cita — appointment
- clínica — clinic
- doctor / doctora — doctor
- médico / médica — physician / doctor
- ayuntamiento — city hall
- ayuda — help
- dolor — pain
- cabeza — head
- estómago — stomach
- me duele la cabeza — my head hurts
- me duele el estómago — my stomach hurts
- no me duele — it does not hurt
- me siento bien — I feel well
- necesito una cita — I need an appointment
- necesito ayuda con un documento — I need help with a document

## Exact natural questions
- How do you ask for help with a document?
- How do you say appointment?
- How do you say doctor?
- How do you say my head hurts?
- How do you say my stomach hurts?
- How do you say I feel well?
- Which word means form?
- Which word means signature?
- Which place is city hall?
- Which place is the clinic?
- How do you say I need an appointment?
- Which word means paper?

## Allison closing
**Spoken EN-F Allison**  
“Now you’re going to use this in real life.”

**Spoken EN-F Allison**  
“Start at city hall.”

**Spoken EN-F Allison**  
“If they send you to the clinic first, that’s okay.”

**Spoken EN-F Allison**  
“Just follow the next step and come back.”

---

# Scene — Cameron at city hall

## Cameron opening
**Spoken ES-M Cameron**  
“Buenos días.”  
**On-screen translation**  
(Good morning.)

**Spoken ES-M Cameron**  
“Bienvenido al pueblo. Nos alegra tenerte aquí.”  
**On-screen translation**  
(Welcome to town. We’re glad to have you here.)

## Zach choice
1. **Spoken ES-M Zach** “Buenos días.”
2. **Spoken ES-M Zach** “Necesito ayuda con un documento.”
3. **Spoken ES-M Zach** “Necesito un formulario.”

Best flow:
1 then 2, or 2 directly.

## Cameron response
**Spoken ES-M Cameron**  
“Claro. Déjame ver.”  
**On-screen translation**  
(Of course. Let me see.)

**Spoken ES-M Cameron**  
“Para este documento, primero necesitas una cita en la clínica con la doctora.”  
**On-screen translation**  
(For this document, you first need an appointment at the clinic with the doctor.)

**Spoken ES-M Cameron**  
“Después vuelve aquí con el papel.”  
**On-screen translation**  
(Then come back here with the paper.)

**Spoken ES-M Cameron**  
“Con eso podré firmarlo.”  
**On-screen translation**  
(With that, I’ll be able to sign it.)

**Spoken ES-M Cameron**  
“Buena suerte.”  
**On-screen translation**  
(Good luck.)

---

# Scene — Supriya at the clinic

## Supriya opening
**Spoken ES-F Supriya**  
“Hola. Bienvenido al pueblo.”  
**On-screen translation**  
(Hello. Welcome to town.)

**Spoken ES-F Supriya**  
“¿Tienes una cita?”  
**On-screen translation**  
(Do you have an appointment?)

## Zach choice
1. **Spoken ES-M Zach** “Sí, necesito una cita.”
2. **Spoken ES-M Zach** “Vengo del ayuntamiento.”
3. **Spoken ES-M Zach** “Necesito ayuda.”

## Supriya
**Spoken ES-F Supriya**  
“Muy bien. Vamos a hacer una revisión breve.”  
**On-screen translation**  
(Very good. We’re going to do a brief checkup.)

### Checkup
**Spoken ES-F Supriya**  
“¿Te duele la cabeza?”  
**On-screen translation**  
(Does your head hurt?)

**Choice**
1. **Spoken ES-M Zach** “No, no me duele la cabeza.”
2. **Spoken ES-M Zach** “Sí, me duele un poco.”

**Spoken ES-F Supriya**  
“¿Te duele el estómago?”  
**On-screen translation**  
(Does your stomach hurt?)

**Choice**
1. **Spoken ES-M Zach** “No, no me duele el estómago.”
2. **Spoken ES-M Zach** “No, me siento bien.”

## Supriya closing
**Spoken ES-F Supriya**  
“Muy bien.”  
**On-screen translation**  
(Very good.)

**Spoken ES-F Supriya**  
“Aquí está tu papel.”  
**On-screen translation**  
(Here is your paper.)

**Spoken ES-F Supriya**  
“Ahora puedes volver al ayuntamiento.”  
**On-screen translation**  
(Now you can go back to city hall.)

**Spoken ES-F Supriya**  
“Cuídate.”  
**On-screen translation**  
(Take care.)

---

# Scene — Cameron returns the finished document

**Spoken ES-M Cameron**  
“Ya volviste.”  
**On-screen translation**  
(You’re back.)

**Choice**
- **Spoken ES-M Zach** “Aquí está el papel.”

**Spoken ES-M Cameron**  
“Perfecto. Ahora sí.”  
**On-screen translation**  
(Perfect. Now yes.)

**Spoken ES-M Cameron**  
“Voy a firmarlo.”  
**On-screen translation**  
(I’m going to sign it.)

**Spoken ES-M Cameron**  
“Listo.”  
**On-screen translation**  
(Done.)

**Spoken ES-M Cameron**  
“Llévalo a Kate.”  
**On-screen translation**  
(Take it to Kate.)

---

# Mini Quest — Flowers for Kate

## Internal thought
*Kate has helped me so much.*  
*I should thank her before I go back.*  
*I should get her flowers.*

## Scene — Alyssa for flowers
**Spoken ES-F Alyssa**  
“Hola otra vez.”  
**On-screen translation**  
(Hello again.)

**Choice**
1. **Spoken ES-M Zach** “Necesito flores, por favor.”
2. **Spoken ES-M Zach** “Quiero comprar un regalo para Kate.”

Best flow:
1

**Spoken ES-F Alyssa**  
“¿Flores para Kate?”  
**On-screen translation**  
(Flowers for Kate?)

**Choice**
1. **Spoken ES-M Zach** “Sí. Quiero darle las gracias.”
2. **Spoken ES-M Zach** “Sí. Ella me ayudó mucho.”

**Spoken ES-F Alyssa**  
“Entonces elige un ramo bonito.”  
**On-screen translation**  
(Then choose a nice bouquet.)

**Spoken ES-F Alyssa**  
“Eso le va a gustar.”  
**On-screen translation**  
(She’ll like that.)

**Spoken ES-F Alyssa**  
“Aquí tienes.”  
**On-screen translation**  
(Here you go.)

**Spoken ES-F Alyssa**  
“Buena suerte.”  
**On-screen translation**  
(Good luck.)

---

# Scene — Kate receives the document and flowers

**Spoken ES-F Kate**  
“Volviste.”  
**On-screen translation**  
(You’re back.)

## Zach choice
1. **Spoken ES-M Zach** “Sí. Aquí está el documento.”
2. **Spoken ES-M Zach** “Y esto es para ti.”

If giving flowers:

**Spoken ES-F Kate**  
“¿Para mí?”  
**On-screen translation**  
(For me?)

**Spoken ES-F Kate**  
“Zach… gracias.”  
**On-screen translation**  
(Zach… thank you.)

**Spoken ES-F Kate**  
“Eso es muy amable.”  
**On-screen translation**  
(That is very kind.)

Then:

**Spoken EN-F Kate**  
“You really did all of that.”

**Spoken EN-F Kate**  
“You went to city hall, got sent to the clinic, came back, and brought me the finished document.”

**Spoken EN-F Kate**  
“That’s a lot.”

**Spoken EN-F Kate**  
“I’m proud of you.”

**Spoken EN-F Kate**  
“And I’m glad you came here first.”

## Internal thought
*I didn’t just get through it.*  
*I handled it.*

---

# LESSON 5 — Invitation Phrases and Belonging

## Allison opening
**Spoken EN-F Allison**  
“I knew you could do it.”

**Spoken EN-F Allison**  
“You handled city hall, the clinic, and all that paperwork.”

**Spoken EN-F Allison**  
“And then you went back to thank Kate.”

**Spoken EN-F Allison**  
“That says a lot about you.”

**Spoken EN-F Allison**  
“Now let’s learn the language of invitations.”

## Teach
- fiesta — party
- invitación — invitation
- vienes — are you coming
- te espero — I’ll be waiting for you
- regalo — gift
- gracias por venir — thanks for coming
- nos vemos allí — see you there

## Test prompts
- How do you say party?
- How do you say invitation?
- How do you ask if someone is coming?
- How do you say gift?
- Which phrase means see you there?
- How do you thank someone for coming?

## Allison closing
**Spoken ES-F Allison**  
“Muy bien.”

**Spoken EN-F Allison**  
“Now use it for real.”

**Spoken EN-F Allison**  
“Invite the people who helped you.”

---

# Invitation Arc

## Hints to the party
Add light hints throughout later scenes:
- the square seems busier than usual
- Alyssa mentions people preparing
- Nancy or Evan mention the square
- Gwendolyn hints something is happening later

Do not fully reveal the party until the end.

---

## Invite Kate

**Spoken ES-F Kate**  
“Hola, Zach.”  
**On-screen translation**  
(Hello, Zach.)

## Internal thought
*Take a breath. Start simply.*

**Choice**
- **Spoken ES-M Zach** “Kate, hay una fiesta en la plaza. ¿Quieres venir?”

**Spoken ES-F Kate**  
“Claro que sí.”  
**On-screen translation**  
(Of course.)

**Spoken ES-F Kate**  
“Gracias por invitarme.”  
**On-screen translation**  
(Thank you for inviting me.)

---

## Invite Cameron

**Spoken ES-M Cameron**  
“Buenos días.”  
**On-screen translation**  
(Good morning.)

## Internal thought
*Okay. This is getting easier.*

**Choice**
- **Spoken ES-M Zach** “Cameron, hay una fiesta en la plaza esta noche. ¿Vienes?”

**Spoken ES-M Cameron**  
“Sí. Iré cuando termine aquí.”  
**On-screen translation**  
(Yes. I’ll go when I finish here.)

---

## Invite Supriya

**Choice**
- **Spoken ES-M Zach** “Supriya, me gustaría invitarte a la fiesta en la plaza.”

**Spoken ES-F Supriya**  
“Gracias. Iré si termino a tiempo.”  
**On-screen translation**  
(Thank you. I’ll go if I finish in time.)

---

## Scene — Gwendolyn tea and invitation

Because Zach already introduced himself earlier, this is now a warmer follow-up.

**Spoken ES-F Gwendolyn**  
“Hola otra vez, Zach.”  
**On-screen translation**  
(Hello again, Zach.)

**Spoken ES-F Gwendolyn**  
“Qué bueno verte.”  
**On-screen translation**  
(It’s good to see you.)

**Spoken ES-F Gwendolyn**  
“Pasa, por favor.”  
**On-screen translation**  
(Come in, please.)

Tea scene:

**Spoken ES-F Gwendolyn**  
“Me alegra ver que te estás adaptando.”  
**On-screen translation**  
(I’m glad to see that you’re settling in.)

## Internal thought
*I’m starting to feel welcome here.*

**Spoken ES-F Gwendolyn**  
“¿Harás algo esta noche?”  
**On-screen translation**  
(Are you doing anything tonight?)

## Zach choice
1. **Spoken ES-M Zach** “Sí. Quiero invitarte a una fiesta en la plaza.”
2. **Spoken ES-M Zach** “¿Quieres venir a la fiesta esta noche?”

**Spoken ES-F Gwendolyn**  
“Claro que sí.”  
**On-screen translation**  
(Of course.)

**Spoken ES-F Gwendolyn**  
“Me alegra verte así.”  
**On-screen translation**  
(I’m glad to see you like this.)

---

## Scene — Invite Evan

**Spoken ES-M Evan**  
“Hola, Zach.”  
**On-screen translation**  
(Hello, Zach.)

## Choice
- **Spoken ES-M Zach** “Evan, hay una fiesta en la plaza esta noche. ¿Vienes?”

**Spoken ES-M Evan**  
“Sí. Gracias por invitarme.”  
**On-screen translation**  
(Yes. Thanks for inviting me.)

---

## Scene — Invite Nancy

**Spoken ES-F Nancy**  
“Hola.”  
**On-screen translation**  
(Hello.)

## Choice
- **Spoken ES-M Zach** “Nancy, hay una fiesta en la plaza. ¿Quieres venir?”

**Spoken ES-F Nancy**  
“Claro. Nos vemos allí.”  
**On-screen translation**  
(Of course. See you there.)

---

## Scene — Alyssa and Joe’s gift

**Spoken ES-F Alyssa**  
“Hola otra vez.”  
**On-screen translation**  
(Hello again.)

## Choice
- **Spoken ES-M Zach** “Alyssa, hay una fiesta en la plaza. ¿Quieres venir?”

**Spoken ES-F Alyssa**  
“Sí, claro.”  
**On-screen translation**  
(Yes, of course.)

## Internal thought
*I shouldn’t arrive empty-handed.*  
*I should get Joe a gift as a thank you for inviting me.*

**Spoken ES-F Alyssa**  
“Si es para Joe, entonces necesitas un regalo de verdad.”  
**On-screen translation**  
(If it’s for Joe, then you need a proper gift.)

Gift selection happens here.

---

## Scene — Final return to Joe

**Spoken ES-M Joe**  
“Volviste.”  
**On-screen translation**  
(You came back.)

## Choice
- **Spoken ES-M Zach** “Sí. Y traje esto para ti.”

Joe receives the gift.

**Spoken ES-M Joe**  
“Gracias, Zach.”  
**On-screen translation**  
(Thank you, Zach.)

**Spoken ES-M Joe**  
“Ven. La plaza te está esperando.”  
**On-screen translation**  
(Come. The square is waiting for you.)

---

# Final Party Reveal

When Zach enters the square:
- tree is decorated
- balloons / festive decorations are visible
- fireworks or spark effects if practical
- all major characters are present

Characters present:
- Kate
- Allison
- Alyssa
- Cameron
- Supriya
- Gwendolyn
- Evan
- Nancy
- Joe

The celebration must happen **before** credits.

## Sample celebratory lines

### Kate
**Spoken ES-F Kate**  
“Mírate ahora.”  
**On-screen translation**  
(Look at you now.)

### Allison
**Spoken ES-F Allison**  
“Has trabajado mucho para llegar aquí.”  
**On-screen translation**  
(You’ve worked hard to get here.)

### Alyssa
**Spoken ES-F Alyssa**  
“Sabía que lo lograrías.”  
**On-screen translation**  
(I knew you’d make it.)

### Gwendolyn
**Spoken ES-F Gwendolyn**  
“Me alegra que estés aquí con nosotros.”  
**On-screen translation**  
(I’m glad you’re here with us.)

### Joe
**Spoken ES-M Joe**  
“Ahora sí. Bienvenido.”  
**On-screen translation**  
(Now then. Welcome.)

## Final internal thought
*When I arrived, this place felt closed to me.*  
*Now it feels like I have a place in it.*  
*I’m still learning. But I’m not outside anymore.*

Then the celebration holds briefly.  
Then credits begin.

## Credits rule
If the player exits the celebration scene early, the credits must still remain accessible and should not break.

---

# Final Tone Rule

The game should feel less like a chain of quizzes and more like this:

**Zach arrives unsure of the town, the language, and the people.  
Step by step, through support, practice, errands, paperwork, care, and conversation, the town becomes more understandable.  
By the end, Zach is no longer standing outside the life of the town. He is part of it.**