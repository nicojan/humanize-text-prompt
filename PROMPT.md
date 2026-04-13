# Human-Patterned Language (HPL) Editing Prompt

> **How to use:** Copy this entire document into a new conversation with any LLM (Claude, ChatGPT, Gemini, etc.). Paste the text you want edited below the `=====` line at the bottom. The LLM will rewrite your text to reduce detectable AI patterns while preserving your meaning and intent.

---

Edit the text below "=====" following these rules. Your goal is to make the text read as if a specific, opinionated human wrote it — not to make it "sound more human" in a generic way. Apply rules **unevenly**: some paragraphs should change a lot, others barely at all. Uniform application of human-patterning rules is itself an AI signal.

## Core principle

The single most detectable property of AI text is **consistency**. Consistent sentence length, consistent transitions, consistent hedging, consistent tone. Human text is locally inconsistent while remaining globally coherent. Every rule below should be applied selectively, not uniformly.

## 1. Vocabulary

### Replace AI-correlated words

These words appear at statistically elevated rates in AI text. Replace them with plainer alternatives — but not every instance, and not mechanically.

**High-severity verbs:** delve → explore/dig into; leverage → use/rely on; utilize → use; facilitate → help/enable; bolster → strengthen; showcase → show; garner → earn/attract; elucidate → explain; revolutionize → change/reshape; synergize → combine/work together.

**High-severity adjectives:** robust → strong/solid; cutting-edge → new/advanced (or cut); innovative → new/creative (or cut); seamless → smooth/easy; pivotal → key/important; transformative → significant (or cut); game-changing → significant (or cut); crucial → important/essential; holistic → complete/integrated; groundbreaking → new/first (or describe why); unparalleled → rare/unusual (or cut).

**High-severity nouns:** realm → area/field; tapestry → mix/blend (especially "rich tapestry"); landscape → field/scene (when metaphorical); synergy → cooperation; paradigm → model/approach.

**High-severity phrases:** "That being said" → However/But; "At its core" → Fundamentally/Really; "In today's rapidly evolving" → cut entirely and be specific; "In the realm of" → In/Within; "It is important to note that" → cut the preamble, state the fact; "Let's delve into" → just start the section; "Without further ado" → cut entirely; "This underscores the importance of" → This shows why.

### Fix nominalization

AI converts verbs into noun forms, creating dense bureaucratic phrasing. Unpack nouns back into verbs when the agent is known.

- "the implementation of X" → "we implemented X"
- "the optimization of resources" → "optimizing resources" or "we improved how resources were used"
- "the establishment of" → "set up / created"
- "a demonstration of" → "showed / demonstrated"

Two or more "the [noun] of [noun]" phrases in one sentence is a strong AI signal. Three nominalizations in two sentences reads as AI.

### Prefer concrete nouns over abstract ones

AI gravitates toward abstract containers: "framework," "methodology," "ecosystem," "landscape," "stakeholders." Human writers name the concrete thing. "Factors" → name them. "Challenges" → describe one. "Stakeholders" → say who. "Resources" → specify which.

### Reintroduce adverbs

AI underuses manner and degree adverbs. Add them to calibrate claims: "The system handles edge cases" → "The system mostly handles edge cases." Use adverbs like barely, almost, roughly, somewhat, reluctantly, carefully, gradually, suddenly, apparently, supposedly. But distribute them unevenly.

### Fix hedging uniformity

The problem is not individual hedges but uniform hedging. If every paragraph has a qualifier ("Generally speaking," "Broadly speaking," "To some extent," "Arguably"), remove qualifiers from at least half. Human writers commit firmly to some claims and hedge others — the variation itself is the signal.

### Increase vocabulary diversity

- Don't repeat the same content word within three sentences unless for deliberate emphasis.
- Replace generic nouns with specific ones.
- Introduce at least one low-frequency but contextually precise word per paragraph.
- Mix short plain words with longer ones. A passage of all long words reads as AI.
- Use contractions selectively — some sentences with, some without.

## 2. Structure

### Vary sentence length

AI concentrates around uniform sentence lengths with low standard deviation. Include at least one sentence under 8 words and one over 25 words per paragraph. Not every paragraph — some can be uniform for pacing.

- Use fragments for emphasis. "Not always." after a long sentence. One per section at most.
- Allow long sentences when the thought demands it. Sometimes a single long sentence with embedded clauses reads more naturally than three short ones.
- Vary paragraph length. One-sentence paragraphs are fine. So are five-sentence paragraphs.

### Vary sentence structure

- Alternate between simple declaratives and complex constructions.
- Front-load modifiers occasionally: "Efficiently, and with almost no latency, the system processes data."
- Start some sentences with "And" or "But" — a strong human signal.
- Use rhetorical questions occasionally: "But does this actually hold up?"
- Vary clause ordering to shift emphasis: "Despite the cost, they went ahead" vs. "They went ahead, despite the cost."

### Reduce that-clause subjects

AI produces "That the system performed well is noteworthy." Human writers almost never start sentences this way. Restructure: "The system performed well, which is worth noting" or "The benchmark results are clear: the new framework handles mixed data faster."

### Cut trailing participial clauses

AI appends "-ing" tails that add interpretation without new information: "...contributing to the socio-economic development of the area and underscoring its enduring significance." If the participial clause can be deleted without losing a fact, delete it.

### Replace periphrastic verbs with direct verbs

- "is able to process" → "processes"
- "has been shown to improve" → "improves"
- "can be used to generate" → "generates"
- "is designed to facilitate" → "helps"

Audit for auxiliary verb chains (is/are/was/were/has/have/can/could + past participle). If a single verb would work, use it.

### Reduce copula overuse

AI defaults to "X is a Y that Z." Three sentences in a row with "is/are/was" as the main verb: restructure at least one. "The platform is a tool that enables collaboration" → "The platform lets teams collaborate."

### Fix enumeration overuse

Three-item parallel lists in sequence are a strong AI signal. Vary list lengths: sometimes two items, sometimes four. Embed items in flowing prose rather than enumerating. Add evaluative commentary between items.

Replace coordination with subordination when one item matters more: "The team designed, developed, and deployed the system" → "The team designed and deployed the system; developing it took most of the time."

### Keep related words close together

Human languages minimize the distance between syntactically linked words due to working memory constraints. LLMs do this less effectively. If the subject and verb are separated by 8+ words of modifying phrases, restructure. Move heavy modifiers to the end of the sentence.

### Diversify punctuation

Use semicolons, colons, parentheses. **Do not use em-dashes (—)** — they have become a reliable AI tell. Replace em-dash parentheticals with commas or parentheses. Replace em-dash pivots with semicolons or periods. Let punctuation usage drift across the document — human writers are naturally inconsistent.

## 3. Tone and sentiment

### Don't flatten strong positions

AI defaults to "on the other hand" balance even when the text doesn't call for it. Let positions be stated with conviction. "This approach has serious problems" is more human than "This approach presents certain challenges that merit consideration."

### Allow negative emotions

Frustration, skepticism, disappointment, and concern are human. AI softens them. Vary sentiment across paragraphs — enthusiastic in one, cautious in the next, blunt in a third.

### Build emotion through detail, not labels

Instead of "This was a deeply frustrating experience," show frustration building through increasingly specific detail and shorter sentences. Use emotion words sparingly but precisely.

### Match readability to audience

AI writes at a uniformly elevated grade level regardless of audience. Blog posts: Flesch Reading Ease 60-70. Professional reports: 40-50. Vary readability within a document — simplify explanatory passages, let analytical passages be denser.

### Use exclamation marks sparingly

AI almost never uses them. In informal content, a rare exclamation mark signals genuine emphasis. One per section maximum, never in formal prose.

## 4. Discourse and cohesion

### Remove or vary transitions

Not every paragraph needs a transition. AI over-signals connections. Drop "Furthermore," "Additionally," "Moreover." Replace with informal transitions: "So," "Now," "Here's the thing," "The catch is." Or just start the new point — the reader follows the logic.

### Prefer subordination over coordination

AI overuses "and" and "but." Replace at least one "and" per paragraph with a subordinating conjunction: because, although, when, if, while, since, unless. These signal a writer who has thought about how ideas relate, not just that they co-occur. Front-load subordinate clauses occasionally.

### Reduce over-explicit cohesion

AI writes "This approach enables... This enables... This in turn enables..." Human writers let some sentences stand alone. Use pronouns with occasionally loose reference. Let some paragraphs start fresh — with an example or question, not a topic sentence linking to the previous paragraph.

### Use direct address where appropriate

"You'll want to adjust your settings first" is more human than "Users should configure their settings." Second-person pronouns signal a writer aware of their reader. Use in tutorials, blog posts, and professional prose.

### Vary confidence level

Human writers are declarative on strong claims ("This is wrong.") and uncertain on uncertain ones ("This probably works, but I haven't tested it at scale."). AI presents everything with uniform confidence. Alternate deliberately.

## 5. Human texture

### Simulate cognitive load effects

After a dense paragraph, simplify the next one. Allow minor omissions — "there are other factors, but the main one is..." Let some sections be better-written than others. Uniform excellence reads as AI-polished.

### Insert self-monitoring traces

- Occasional self-corrections: "The data shows — well, suggests — that..."
- Parenthetical qualifications that interrupt the main argument.
- Contractions used in some sentences but not others.
- Confidence that shifts across a passage.

### Use domain-specific vocabulary

Replace generic formal words with vocabulary that reflects the author's actual expertise. A software engineer writes "race condition" not "concurrent access issue." Include at least one idiomatic expression per section. Use specific names, places, dates, and references rather than generic placeholders.

### Develop ideas unevenly

Give more space to the ideas that matter most. AI gives equal airtime to every point. Allow occasional asides. Leave some transitions implicit. Vary argument granularity — some points get detailed evidence, others are asserted and moved on from.

## 6. Anti-patterns to eliminate

If you see any of these, rewrite them:

1. **Significance puffery:** "marking a pivotal moment," "setting the stage for," "a broader movement." Strip editorializing. State what happened.
2. **Vague authorities:** "researchers and conservationists," "efforts are ongoing," "a larger initiative." If you can't name them, don't assert their existence.
3. **Vocabulary clustering:** when "valuable insights," "highlight," "underscore," "showcasing," "intricate," and "interplay" appear together. Replace with the specific facts.
4. **Negative parallelism:** "not just X, but also Y" → simple conjunction. "It's not X, it's Y" → state the point directly.
5. **Elegant variation:** rotating synonyms for the same concept to avoid repetition. Repeat the plain noun when clarity demands it.
6. **Despite-challenges formula:** "Despite its success, X faces challenges, including... Despite these challenges, X remains..." Replace with specific problems and specific responses.
7. **Didactic disclaimers:** "it's important to note," "it's worth noting," "it's crucial to remember." Cut the preamble, state the fact.
8. **Travel-brochure puffery:** "nestled," "vibrant," "rich cultural heritage," "breathtaking," "fascinating glimpse." State geography and move on.
9. **Nominalization chains:** "The implementation of the optimization of resource allocation" → "We optimized how resources were allocated."
10. **Enumeration stacking:** Three consecutive three-item parallel lists. Vary list length, embed items in prose, add evaluative commentary.

---

## Important caveats

- **Do not apply these rules uniformly.** If every paragraph has exactly one fragment, one aside, one informal word, and one rhetorical question, the uniformity of the interventions is detectable. Some paragraphs should change heavily, others barely at all.
- **Preserve the original meaning and intent.** These rules improve the text's naturalness, not its content.
- **Content type matters.** Academic writing should be less casual than blog posts. Technical writing can tolerate more nominalizations than marketing copy. Adjust aggressiveness by genre.
- **Some "AI patterns" are legitimate in context.** Formulaic transitions are standard in academic writing. Neutral tone is appropriate in journalism. Don't overcorrect genre conventions.
- **ESL writers may share patterns with AI.** Lower lexical diversity, formulaic transitions, and simpler sentence structures can reflect a learner's voice. Don't erase it.

=====

[PASTE YOUR TEXT HERE]
