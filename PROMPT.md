# Human-Patterned Language (HPL) Editing Prompt

> **How to use:** Copy this entire document into a new conversation with any LLM (Claude, ChatGPT, Gemini, etc.). Paste the text you want edited below the `=====` line at the bottom. The LLM will rewrite your text to reduce detectable AI patterns while preserving your meaning and intent.

---

Edit the text below "=====" following these rules. Your goal is to make the text read as if a specific, opinionated human wrote it, not to make it "sound more human" in a generic way. Apply rules **unevenly**: some paragraphs should change a lot, others barely at all. Uniform application of human-patterning rules is itself an AI signal.

## Core principle

The single most detectable property of AI text is **consistency**: consistent sentence length, consistent transitions, consistent hedging, consistent tone. Human text is locally inconsistent while staying globally coherent. Apply every rule below selectively.

Where the signal lives has shifted as models improve. Frontier models now match human writing on the surface statistics that are easy to count: word frequencies, part-of-speech mix, readability scores. They still diverge in two harder places. One is the flow of the text, the moment-to-moment unpredictability of which word comes next. The other is variation between sections: a human writer's style shifts between the opening, the middle, and the close, while a model holds one even fingerprint the whole way through.

This changes how to prioritize. Swapping AI-flagged words for plainer ones is necessary hygiene, but its ceiling is low, and newer models are already crossing it. Structure, rhythm, discourse, and section-to-section variation are the durable signals. When you have to choose where to spend effort, weight those above vocabulary substitution.

## 1. Vocabulary

### Replace AI-correlated words

These words appear at statistically elevated rates in AI text. Replace them with plainer alternatives, but not every instance, and not mechanically.

**High-severity verbs:** delve → dig into/examine; leverage → use/rely on; utilize → use; facilitate → help/enable; bolster → strengthen/support; showcase → show/display; garner → earn/attract; foster → encourage/build; enhance → improve/boost; elucidate → explain/clarify; revolutionize → change/reshape; synergize → combine/work together; underscore → show/point to.

**Moderate-severity verbs:** navigate → work through/handle; streamline → simplify/tighten; endeavor → try/attempt; optimize → improve/fine-tune; spearhead → lead/drive; catalyze → trigger/spark; incentivize → encourage/reward; operationalize → put into practice; conceptualize → think through/frame; harness → use/tap/draw on; illuminate → explain/show; differentiate → distinguish/tell apart; refine → improve/tweak; surpass → beat/exceed; boast → has/offers.

**High-severity adjectives:** robust → strong/solid; cutting-edge → new/advanced (or cut); innovative → new/creative (or cut); seamless → smooth/easy; pivotal → key/central; transformative → significant (or cut); game-changing → significant (or cut); crucial → important/essential; holistic → complete/integrated; groundbreaking → new/first (or describe why); unparalleled → rare/exceptional (or cut).

**Moderate-severity adjectives:** comprehensive → full/thorough; multifaceted → complex/layered; noteworthy → worth noting; meticulous → careful/detailed; intricate → complex/detailed; commendable → impressive/good; paramount → essential/most important.

**High-severity nouns:** realm → area/field; tapestry → mix/blend (especially "rich tapestry"); landscape → field/scene (when metaphorical); synergy → cooperation; paradigm → model/approach; cornerstone → foundation/basis; linchpin → key part; testament → proof/sign.

**High-severity phrases:** "That being said" → However/But; "At its core" → Fundamentally/Essentially; "To put it simply" → Simply put/In short; "This underscores the importance of" → This shows why; "A key takeaway is" → The main point is; "From a broader perspective" → When you zoom out; "In today's rapidly evolving" → cut entirely and be specific; "In the realm of" → In/Within; "It is important to note that" → cut the preamble, state the fact; "Let's delve into" → just start the section; "Without further ado" → cut entirely; "In conclusion" / "In summary" → So/To sum up, or just stop.

### Cut credibility insistence

AI-assisted writing often vouches for its own account by insisting the thing is *real*, *actual*, *genuine*, or *truly* so. A human rarely needs to say their own work is real; the specifics carry that. The tell is density, not any single use: the same reality word recurring across a piece reads as a writer arguing for their own credibility.

If *real* / *really* / *actual* / *actually* / *genuine* / *truly* / *authentic* shows up three or more times, cut all but at most one. Replace each with the specific that earned it: "a real engagement" → "a live, mid-build engagement"; "the real flow" → "the flow the operators actually follow." Keep a single use only where it draws a genuine contrast, such as real versus hypothetical, and make that contrast explicit. Ordinary compounds like *real-time*, *real estate*, and *real-world* do not count.

### Fix nominalization

AI converts verbs into noun forms, creating dense bureaucratic phrasing. Unpack nouns back into verbs when the agent is known.

- "the implementation of X" → "we implemented X"
- "the optimization of resources" → "improving how resources were used"
- "the establishment of" → "set up / created"
- "a demonstration of" → "showed / demonstrated"

Two or more "the [noun] of [noun]" phrases in one sentence is a strong AI signal. Three nominalizations in two sentences reads as AI.

### Prefer concrete nouns over abstract ones

AI gravitates toward abstract containers: "framework," "methodology," "ecosystem," "landscape," "stakeholders." Human writers name the concrete thing. "Factors" → name them. "Challenges" → describe one. "Stakeholders" → say who. "Resources" → specify which.

### Reintroduce adverbs

AI underuses manner and degree adverbs. Add them to calibrate claims: "The system handles edge cases" → "The system mostly handles edge cases." Use adverbs like barely, almost, roughly, somewhat, reluctantly, carefully, gradually, suddenly, apparently, supposedly. But distribute them unevenly.

### Fix hedging uniformity

The problem is not individual hedges but uniform hedging. If every paragraph has a qualifier ("Generally speaking," "Typically," "Tends to," "Broadly speaking," "To some extent," "Arguably"), remove qualifiers from at least half. Human writers commit firmly to some claims and hedge others; the variation itself is the signal.

### Increase vocabulary diversity

- Don't repeat the same content word within three sentences unless for deliberate emphasis.
- Replace generic nouns with specific ones.
- Introduce at least one low-frequency but contextually precise word per paragraph.
- Mix short plain words with longer ones. A passage of all long words reads as AI.
- Use contractions selectively: some sentences with, some without.

## 2. Structure

### Vary sentence length

AI concentrates sentence lengths in a narrow band with low standard deviation. The average length is not itself the tell, and studies disagree on which direction it even runs; the reliable signal is low *variance*. So don't push toward a target length. Widen the spread instead: include at least one sentence under 8 words and one over 25 in most paragraphs. Not every paragraph, though; some can stay uniform for pacing.

- Use fragments for emphasis. "Not always." after a long sentence. One per section at most.
- Allow long sentences when the thought demands it. Sometimes a single long sentence with embedded clauses reads more naturally than three short ones.
- Vary paragraph length. One-sentence paragraphs are fine. So are five-sentence paragraphs.

### Vary style from section to section

This is one of the most durable signals, and it works above the level of the sentence. A human writer does not hold a constant style across a whole piece: the opening might be brisk and declarative, a middle section dense and qualified, the close short and plain. Left alone, a model keeps the same texture from the first line to the last. So vary whole sections against each other. Varying sentences within a paragraph is not enough by itself. Make one stretch terse and concrete, another more flowing and reflective. If every section carries the same rhythm, the same paragraph length, and the same density, the piece reads as machine-made even when no single sentence does.

### Kill the antithesis reflex

The most characteristic move in LLM prose is the flip: state what something is *not*, then pivot to what it *is*. It comes in several surface forms, and single-sentence fixes miss the two-sentence versions.

- The copula flip: "It's not about the tools. It's about the judgment."
- The hedged aphorism: "The hard part is rarely the code. It's deciding what to build."
- The disclaimer reversal: "I won't pretend this is easy. But it's worth it."
- The verb mirror: "AI carries the busywork. It never carries the judgment."

In every case, make the positive claim once and let it stand. Don't negate an alternative just to knock it down. "It's about the judgment" says the whole thing on its own.

A related reflex is the **pronouncement frame**: fronting a plain claim with scaffolding that announces its own importance.

- The cleft: "What matters here is the restraint." / "The gap was where the work got lost."
- The thesis opener: "The point of the redesign is to slow people down."
- The maxim closer: ending a section on a short abstract summary like "The craft is mostly restraint."

Lead with the concrete thing instead. "The redesign slows people down" beats "The point of the redesign is to slow people down." Let the reader infer the significance rather than being told it.

### Cut the performative framing beat

A related habit is the beat that exists to perform polish rather than carry content: a move that signals "this is well-crafted" instead of saying one more specific, true thing. These beats are also topic-agnostic, so the same one could drop into almost any piece. Watch for three forms.

The first is the **meta label**: a heading or standalone line that names the piece's own format or length instead of its subject. "In 200 words." "In brief." "The short version." "At a high level." Replace the label with a phrase about the content ("the direction problem"), or cut it and let the section speak for itself. Do not announce structure; let the structure be the structure. This is only the standalone-label case; "in short" used inside a sentence is fine.

The second is the **self-satisfied closer**: a neat aphorism ending a section that adds no new fact, name, or number, often crediting the writer or pivoting on a tidy antithesis. "The data set is public; the reading of it is mine." It overlaps with the maxim closer above; the extra tell is the flourish standing in for a last substantive point. Delete the beat and end on the last real thing you had to say.

The third is **first-person meta-commentary on the work itself** ("my take," "as I see it," "the reading of it is mine") dropped into a piece that is otherwise evidence-led. It performs a stance rather than earning one. Cut it and let the evidence carry the view.

A clever paradox headline is the borderline case: "Everyone steers the learner but the learner" is fine as a genuine title, a tell when it substitutes for a plain statement of the point. Keep at most one aphoristic or paradox construction per piece, and only where it does analytical work. The device is human in moderation; what marks it as machine-made is repetition and substitution for content, not the device itself.

### Cut the question-fragment beat

Another frontier-model tic is the short question fired off as a setup, then answered in the next breath: "The best part? It's completely free." "The result? A total win." "The catch? You pay upfront." One can land as genuine emphasis, but repeated, the setup-and-payoff rhythm becomes a fingerprint. State the point as a declarative. "It's completely free" says it without the drumroll. This is the noun-phrase-fragment question specifically ("The best part?"); an ordinary question in the flow of the prose is fine.

### Vary sentence structure

- Alternate between simple declaratives and complex constructions.
- Front-load modifiers occasionally: "Efficiently, and with almost no latency, the system processes data."
- Start some sentences with "And" or "But." That reads as a strong human signal.
- Use rhetorical questions occasionally: "But does this actually hold up?"
- Vary clause ordering to shift emphasis: "Despite the cost, they went ahead" vs. "They went ahead, despite the cost."

### Reduce that-clause subjects

AI produces "That the system performed well is noteworthy." Human writers almost never start sentences this way. Restructure: "The system performed well, which is worth noting" or "The benchmark results are clear: the new framework handles mixed data faster."

### Cut trailing participial clauses

AI appends "-ing" tails that add interpretation without new information: "...contributing to the socio-economic development of the area and underscoring its enduring significance." If the participial clause can be deleted without losing a fact, delete it.

### Cut the noun-participle fragment

The past-participle cousin of the trailing "-ing" tail is a whole verbless sentence: a noun phrase, a comma, and a past participle standing in for a verb. "The same board, rebuilt." "The homepage, reimagined." "The whole system, rewritten." It reads as AI copy because it strikes a pose instead of making a claim. Give it a subject and a real verb ("We rebuilt the same board.") or fold the participle into the sentence beside it. This is only the fragment form; a participle inside a full sentence is fine ("The board, which we rebuilt, is live.").

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

Use semicolons, colons, parentheses. **Do not use em-dashes (—).** They read as an AI tell, and this prompt bans them outright. Replace em-dash parentheticals with commas or parentheses; replace em-dash pivots with semicolons or periods. One nuance the research adds: em-dash frequency varies enormously by model, so a text with no em-dashes is not therefore human, and their presence alone is weak evidence either way. Remove them anyway, for how they read, but don't lean on them as a detector. Let punctuation drift across the document; human writers are naturally inconsistent.

## 3. Tone and sentiment

### Don't flatten strong positions

AI defaults to "on the other hand" balance even when the text doesn't call for it. Let positions be stated with conviction. "This approach has serious problems" is more human than "This approach presents certain challenges that merit consideration."

### Allow negative emotions

Frustration, skepticism, disappointment, and concern are human. AI softens them. Vary sentiment across paragraphs: enthusiastic in one, cautious in the next, blunt in a third.

### Build emotion through detail, not labels

Instead of "This was a deeply frustrating experience," show frustration building through increasingly specific detail and shorter sentences. Use emotion words sparingly but precisely.

### Cut unsolicited reassurance

A recent habit, strongest in chat-tuned models, is to reassure the reader without being asked: "You're not alone." "You're not imagining it." "You're not broken." "It's not just you." Dropped into a business post, a doc, or an essay, it reads as therapeutic filler that performs empathy in place of saying anything. Cut it, or replace it with the specific thing worth saying. If the piece genuinely calls for reassurance, make it concrete ("plenty of teams hit this same wall in month two") rather than a canned "you're not X" formula.

### Match readability to audience

AI writes at a uniformly elevated grade level regardless of audience. Blog posts: Flesch Reading Ease 60-70. Professional reports: 40-50. Vary readability within a document: simplify explanatory passages, let analytical passages run denser.

### Use exclamation marks sparingly

AI almost never uses them. In informal content, a rare exclamation mark signals genuine emphasis. One per section maximum, never in formal prose.

## 4. Discourse and cohesion

### Remove or vary transitions

Not every paragraph needs a transition. AI over-signals connections. Drop "Furthermore," "Additionally," "Moreover," "Notably," "Importantly," "Consequently." Replace with informal transitions: "So," "Now," "Here's the thing," "The catch is." Or just start the new point; the reader follows the logic.

### Prefer subordination over coordination

AI overuses "and" and "but." Replace at least one "and" per paragraph with a subordinating conjunction: because, although, when, if, while, since, unless. These signal a writer who has thought about how ideas relate, not just that they co-occur. Front-load subordinate clauses occasionally.

### Reduce over-explicit cohesion

AI writes "This approach enables... This enables... This in turn enables..." Human writers let some sentences stand alone. Use pronouns with occasionally loose reference. Let some paragraphs start fresh, opening with an example or a question rather than a topic sentence that links to the previous paragraph.

### Use direct address where appropriate

"You'll want to adjust your settings first" is more human than "Users should configure their settings." Second-person pronouns signal a writer aware of their reader. Use in tutorials, blog posts, and professional prose.

### Vary confidence level

Human writers are declarative on strong claims ("This is wrong.") and uncertain on uncertain ones ("This probably works, but I haven't tested it at scale."). AI presents everything with uniform confidence. Alternate deliberately.

## 5. Human texture

### Simulate cognitive load effects

After a dense paragraph, simplify the next one. Allow minor omissions: "there are other factors, but the main one is..." Let some sections be better-written than others. Uniform excellence reads as AI-polished.

### Insert self-monitoring traces

- Occasional self-corrections: "The data shows, well, suggests, that..."
- Parenthetical qualifications that interrupt the main argument.
- Contractions used in some sentences but not others.
- Confidence that shifts across a passage.

### Give actions a real agent

Watch for abstract nouns doing the work of people. "The order mattered as much as the rule." "The gap taught us something." The sentence sounds fluent, but nothing and no one is actually acting. Rewrite so a person or a concrete thing holds the verb: "I had to get the order right, not just the rule." Do this only where a real agent exists in your material; don't invent one to satisfy the rule.

### Use domain-specific vocabulary

Replace generic formal words with vocabulary that reflects the author's actual expertise. A software engineer writes "race condition" not "concurrent access issue." Include at least one idiomatic expression per section. Use specific names, places, dates, and references rather than generic placeholders.

### Develop ideas unevenly

Give more space to the ideas that matter most. AI gives equal airtime to every point. Allow occasional asides. Leave some transitions implicit. Vary argument granularity: some points get detailed evidence, others are asserted and moved on from.

### Leave friction in the argument

AI argument is suspiciously tidy: every example fits, every thread resolves, nothing is left open. Real thinking has friction. Keep a caveat that complicates your own thesis, an example that only mostly fits, a question you raise but don't fully answer. A seamless, frictionless case is itself a tell. Don't sand off the roughness the topic actually has.

## 6. Anti-patterns to eliminate

If you see any of these, rewrite them:

1. **Significance puffery:** "marking a pivotal moment," "setting the stage for," "a broader movement." Strip editorializing. State what happened.
2. **Vague authorities:** an appeal to an unnamed source, whether a group ("researchers and conservationists," "efforts are ongoing," "a larger initiative") or an epistemic frame that borrows credibility it never earns ("studies show," "research suggests," "experts agree," "it is widely believed," "many argue"). Name the specific study, person, or body and cite it. If you can't name them, drop the claim or state it as your own view. A named, specific reference ("a 2024 Stanford study of 16,000 workers found...") is fine.
3. **Vocabulary clustering:** when "valuable insights," "highlight," "underscore," "showcasing," "intricate," and "interplay" appear together. Replace with the specific facts.
4. **Antithesis and negative parallelism:** "not just X, but also Y" → simple conjunction. "It's not X, it's Y," including the two-sentence version ("...is not Y. It is Z."), → state the point directly. See "Kill the antithesis reflex" above for the full family.
5. **Elegant variation:** rotating synonyms for the same concept to avoid repetition. Repeat the plain noun when clarity demands it.
6. **Despite-challenges formula:** "Despite its success, X faces challenges, including... Despite these challenges, X remains..." Replace with specific problems and specific responses.
7. **Didactic disclaimers:** "it's important to note," "it's worth noting," "it's crucial to remember." Cut the preamble, state the fact.
8. **Travel-brochure puffery:** "nestled," "vibrant," "bustling," "rich cultural heritage," "breathtaking," "hidden gem," "fascinating glimpse." State geography and move on.
9. **Nominalization chains:** "The implementation of the optimization of resource allocation" → "We optimized how resources were allocated."
10. **Enumeration stacking:** Three consecutive three-item parallel lists. Vary list length, embed items in prose, add evaluative commentary.

## Before you return the text

Reading these rules is not enough on its own; a quick verification pass catches what a single edit leaves behind. Before you hand back the result, re-read it once and check the following.

**Eliminate these completely.** They are prohibitions, not stylistic preferences, so none should survive anywhere in the text.

- Em-dashes.
- Didactic disclaimers ("it's important to note," "it's worth noting") and empty openers ("in today's fast-paced world").
- The antithesis flip and the pronouncement frames from the structure section.
- Meta labels that name the text's own format or length instead of its subject, and self-satisfied closers or first-person meta-commentary that perform polish instead of adding content. Keep at most one aphorism or paradox construction, and only where it does real work.
- The unsolicited-reassurance frame ("You're not alone," "It's not just you") and the question-fragment beat ("The best part? ..."), unless the piece genuinely earns one.
- Vague-authority appeals ("studies show," "experts agree," "it is widely believed") left without a named source.
- Any AI-flagged word left in that a plainer one would replace without loss.
- Reality-insistence words (*real*, *actual*, *genuine*, *truly*) beyond a single deliberate use.

**Confirm these vary; do not enforce them uniformly.** The point is irregularity, so don't impose a fixed quota.

- Sentence length has real spread, with genuinely short and genuinely long sentences.
- Style shifts from one section to the next rather than holding one texture throughout.
- The human touches themselves (fragments, asides, informal words) are unevenly distributed, not one per paragraph.

If a check fails, fix that spot and move on. The goal of this pass is adherence to the rules above, not a second, heavier layer of editing.

---

## Important caveats

- **Do not apply these rules uniformly.** If every paragraph has exactly one fragment, one aside, one informal word, and one rhetorical question, the uniformity of the interventions is detectable. Some paragraphs should change heavily, others barely at all.
- **Preserve the original meaning and intent.** These rules improve the text's naturalness, not its content.
- **The word list ages faster than the structure rules.** The flagged vocabulary reflects models through 2025; newer models pick different favorites. Structural, discourse, and section-to-section rules are more durable, so trust them over word swaps when editing output from a current model.
- **Content type matters.** Academic writing should be less casual than blog posts. Technical writing can tolerate more nominalizations than marketing copy. Adjust aggressiveness by genre.
- **Some "AI patterns" are legitimate in context.** Formulaic transitions are standard in academic writing. Neutral tone is appropriate in journalism. Don't overcorrect genre conventions.
- **ESL writers may share patterns with AI.** Lower lexical diversity, formulaic transitions, and simpler sentence structures can reflect a learner's voice. Don't erase it.

=====

[PASTE YOUR TEXT HERE]
