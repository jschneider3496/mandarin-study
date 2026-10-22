# Practice-First Lesson Design

This document is the source of truth for creating, rewriting, and reviewing lessons in this repository. It is written primarily for LLMs and maintainers generating lesson content.

The objective is not merely to expose the learner to vocabulary. A successful lesson repeatedly moves vocabulary from recognition into independent reading and speech.

## Priority order

When requirements compete, use this order:

1. **Learner production:** the learner must answer, transform, translate, create, and speak.
2. **Repeated contextual use:** important vocabulary must recur in varied, natural sentences.
3. **Retrieval before support:** ask the learner to recall language before showing pinyin, English, or answers.
4. **Connected speech:** favor multi-sentence answers and follow-up questions over isolated words.
5. **Controlled-to-open progression:** provide a bridge from examples to independent conversation.
6. **Spaced recycling:** bring earlier vocabulary back on later days and in new situations.
7. **Readable, natural Mandarin:** repetition must not make dialogues mechanical or unnatural.
8. **Clear self-correction:** keep support and answer material separate from the first attempt.
9. **Practical communication:** practice should resemble things the learner may actually say.
10. **Repository consistency:** files, schedules, answer keys, and tutor instructions must agree.

Do not maximize vocabulary breadth at the cost of practice depth. Fewer well-recycled patterns are more valuable than many one-time examples.

## Stable learning constraints

- Use simplified Chinese.
- Provide tone-mark pinyin in support material.
- Focus on reading and speaking; do not add handwriting drills.
- Assume the learner often answers through speech-to-text.
- Keep the stated difficulty of the unit unless a change is explicitly requested.
- Preserve an existing unit's vocabulary targets when rewriting that unit.
- Treat `vocab.md` as the source of truth for target spelling, pinyin, meaning, priority, and numbering.
- Extra words are allowed when a dialogue needs them, but keep them simple and list them in a mini glossary.
- Prefer high-frequency, conversationally reusable Mandarin over literal English-shaped sentences.

## Unit file contract

Each practice-first unit contains exactly two files: `vocab.md` and `lessons.md`. The repository also provides one shared top-level `tutor.md`.

### `vocab.md`

- The numbered target vocabulary list.
- Priority labels and useful collocations.
- A short bank of functional “must-say” sentences.
- Existing vocabulary must not be silently removed, renamed, or renumbered during a lesson rewrite.

### `lessons.md`

- Six complete daily lessons.
- A short daily method at the top of the file.
- Target allocation, recycling goals, required output, and completion criteria at the start of each day.
- Characters-first input and all learner-facing exercises.
- Retrieval, comprehension, controlled production, translation, original sentences, and roleplay.
- A collapsed answer/support panel immediately after every numbered section.
- Natural model responses for retrieval, quick-production, original-sentence, and roleplay sections.
- Hanzi, tone-mark pinyin, and English for every answer and model, including single-word answers.

This is the unit's complete learner-facing practice workbook. Do not create separate `reading.md`, `schedule.md`, `answer-key.md`, or per-unit `tutor.md` files for a practice-first unit.

Use HTML `<details>` and `<summary>` elements for each answer panel so support is nearby but hidden during the first attempt. Acknowledge that open-ended prompts can have many correct answers and give one natural model rather than implying it is the only possible response.

## Shared top-level `tutor.md`

- One repository-level protocol for interactive practice with every unit.
- Require production before revealing a model.
- Ask one prompt at a time.
- Track errors and vocabulary the learner recognizes but avoids using.
- Retest weak language later in a different context.
- Do not create a per-unit `tutor.md`; unit-specific scenarios and complications belong in `lessons.md`.

## Six-day progression

For a 40-target existing unit, use this default allocation:

| Day | Main purpose | Vocabulary load |
|---|---|---|
| 1 | Establish the basic situation and core functions | Targets #1–#10 |
| 2 | Add a second communicative function | Targets #11–#20; recycle Day 1 |
| 3 | Add explanation, contrast, or sequencing | Targets #21–#30; recycle Days 1–2 |
| 4 | Add problem-solving or social follow-up | Targets #31–#40; recycle earlier days |
| 5 | Introduce or report about another person/situation | Cumulative retrieval and recombination |
| 6 | Sustain a flexible capstone conversation | Cumulative performance with a complication |

The semantic groupings in `vocab.md` may justify a different split. If so, preserve all targets and document the changed allocation in each day header in `lessons.md`.

Days 1–4 should introduce language. Days 5–6 should primarily test recombination, recall, and conversational flexibility rather than add another large vocabulary set.

## Required daily lesson shape

Days 1–4 should normally contain all sections below. Days 5–6 may combine sections to emphasize cumulative performance.

### 1. Targets and functional patterns

List:

- New targets
- Recycled targets
- Two or three functional patterns

Patterns should express useful functions such as asking a choice, giving a reason, making a request, comparing options, or proposing a next step.

### 2. Retrieval warm-up

Give two or three spoken prompts before the learner rereads earlier material.

Good prompts require a complete thought:

- “Say where you live now and where you lived before.”
- “Name two interests and say which one you prefer.”
- “Ask a choice question, then answer it.”

Avoid prompts that merely ask the learner to recite a vocabulary list.

### 3. Characters-first dialogue

- Use approximately eight turns.
- Build one coherent, plausible situation.
- Use the day's target language naturally.
- Reuse earlier targets where the context supports them.
- Withhold pinyin and English until the collapsed support panel immediately after the dialogue.
- Add a mini glossary of no more than about five necessary non-target items.

Do not print the same dialogue three times in different formats. That creates visual volume without creating a new retrieval event.

### 4. Dialogue questions

Provide five questions. A useful mix is:

- Three concrete comprehension questions
- One inference, comparison, or explanation question
- One personalized response or learner-created follow-up question

Require full Mandarin sentences. On selected days, require a target word in every answer.

Questions should make the learner reconstruct meaning. Do not make every answer a single noun copied directly from the preceding line.

### 5. Varied model sentences

Show the target vocabulary in contexts beyond the dialogue.

- Use approximately five short sentences per day.
- Change subject, time, polarity, question form, or collocation.
- Ask the learner to read them aloud and alter one detail.
- Distinguish easily confused targets through contrast, such as `兴趣` versus `爱好` or `比较` versus `更`.

Repetition is only useful when the surrounding meaning changes enough to build flexible use.

### 6. Controlled production

Include several of the following:

- Fill in a target word
- Choose between confusable targets
- Combine two short ideas with a connector
- Transform a statement into a question
- Change present information into completed or future information
- Correct an intentionally flawed sentence
- Rephrase the same meaning with a different pattern

These exercises form the bridge between recognizing examples and creating speech independently.

### 7. English → Mandarin

Include about five prompts per day:

1. One close to the dialogue
2. One testing a functional pattern
3. One recombining targets from the current day
4. One recycling an earlier target
5. One natural transfer sentence not memorized from the reading

Translation exists here as a production and diagnostic exercise. Avoid unnatural word-for-word English mappings. The answer key should provide a natural model and accept other correct phrasing.

### 8. Original production

Require at least three original outputs. Use specific constraints, for example:

- “Create one sentence with `来自` and a different sentence with `从…来`.”
- “Describe your routine using `平时`, `一般`, and `经常`.”
- “Give an opinion, one reason, and one next step.”

“Use this word in a sentence” is acceptable only when paired with a function or context. The learner should make a meaning choice, not merely insert a word into a memorized frame.

### 9. Roleplay and exit ticket

End with a practical roleplay. Later days should add a complication such as:

- The first proposed time is unavailable.
- The requested item is unavailable.
- The other speaker disagrees.
- A plan changes.
- The learner must clarify a misunderstanding.

Finish with one short task performed without notes. The exit ticket should test the day's main communicative outcome, not vocabulary recognition.

## Vocabulary repetition standard

A vocabulary label, glossary entry, or answer-panel appearance does not count as a meaningful encounter.

A meaningful encounter occurs when a target is used in a natural Mandarin sentence that the learner must understand, manipulate, or produce.

For each target, aim for at least:

- One occurrence in a dialogue or short reading
- One occurrence in a different model sentence
- One controlled production prompt
- One original, translation, or roleplay production opportunity
- One later-day retrieval or cumulative reuse opportunity

Core words should appear more often than situational words. Across a unit, a core target should normally receive six or more meaningful encounters and at least two independent production demands.

Do not satisfy the standard by repeating an identical sentence. Vary the speaker, situation, grammatical form, or communicative purpose.

## Reading and support policy

The learner's first pass should be characters only. This encourages actual reading instead of automatic dependence on pinyin or English.

Place these in the collapsed support panel immediately after the matching section in `lessons.md`:

- Line-by-line Hanzi, tone-mark pinyin, and concise English meaning
- Controlled exercise answers in Hanzi, tone-mark pinyin, and English
- Suggested factual comprehension answers in Hanzi, tone-mark pinyin, and English

When writing pinyin:

- Use tone marks, not tone numbers.
- Keep neutral tones unmarked.
- Be consistent about names and place names.
- Check tone changes and pronunciation notes already established in `vocab.md`.

## Tutor behavior

The tutor extends the lesson; it should not replace the learner's independent attempt.

The tutor should:

1. Begin with retrieval.
2. Ask one question at a time.
3. Wait for production before providing a model.
4. Correct concisely and ask the learner to try a nearby example.
5. Track the top recurring errors.
6. Track target words the learner understands but avoids producing.
7. Retest weak language two or three turns later with changed information.
8. Add one complication during roleplay.
9. End by testing three words without displaying them in Mandarin.

Simply repeating the tutor's corrected sentence does not count as independent production. The learner must later use the same language with new content.

## LLM workflow for creating or rewriting a unit

### 1. Gather constraints

Read:

- `README.md`
- This design document
- The unit's `vocab.md`
- The previous unit's grammar and difficulty level, when one exists
- Existing files in the unit being rewritten

If rewriting, inventory the exact numbered targets before drafting.

### 2. Build a coverage map

Before writing prose, map every target to:

- Introduction day
- Dialogue or reading
- Varied model sentence
- Controlled exercise
- Productive prompt
- Later review day

Do not rely on memory to distribute 40 targets.

### 3. Design the six scenarios

Create a coherent progression in which later situations naturally reuse earlier language. The capstone should combine several earlier functions rather than introduce an unrelated setting.

### 4. Draft `lessons.md`

Write the characters-first material and exercises first. Do not place visible answers inside the exercise itself.

### 5. Add collapsed answer panels

After each numbered section, add a collapsed panel containing its support or model responses. Verify every answer against the exact prompt. For every answer or model, include Hanzi, tone-mark pinyin, and English. Add support only after the Mandarin dialogue is stable.

### 6. Align the unit and global tutor

Confirm that each `lessons.md` day header states its targets, recycling, output, and completion criteria. Update the top-level `tutor.md` only when the reusable session protocol changes; keep unit-specific content in `lessons.md`.

### 7. Audit before completion

Check all of the following:

- The vocabulary list itself was preserved when preservation was required.
- All target words appear in meaningful learner-facing contexts.
- Every day has retrieval and independent production.
- Every day has dialogue questions.
- Every day has English→Mandarin production or a cumulative equivalent.
- Pinyin and English remain collapsed during the first attempt and accompany every answer or model.
- Answer numbering matches exercise numbering.
- Day titles, target ranges, exercises, and embedded answers agree across the two unit files.
- Roleplays become less controlled over the six days.
- The capstone includes an interaction problem or change of plan.
- Markdown passes `git diff --check`.

## Common failure modes

Avoid these patterns:

- Three visual copies of the same dialogue presented as three separate activities
- Forty words introduced but only a small subset used in sentences
- Comprehension questions that can all be answered with one copied word
- A single broad “speak about the topic” prompt with no scaffolding
- Translation only in the earliest units
- “Use at least four words” without a meaningful communicative objective
- New words added to solve every writing problem instead of reusing known language
- Answer keys placed directly beneath exercises
- Tutor instructions that reveal the answer before eliciting an attempt
- Schedules whose target numbers no longer match `vocab.md`
- Difficulty increases caused only by longer sentences rather than richer learner decisions

## Definition of done

A lesson is complete when a learner can use it without an LLM and gain additional value with an LLM.

The static files must provide enough structure for retrieval, comprehension, correction, and independent production. The tutor should add adaptivity, follow-up questions, personalized correction, and conversational pressure—not supply practice that the lesson forgot to include.
