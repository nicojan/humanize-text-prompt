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

**Moderate-severity verbs:** navigate → work through/handle; streamline → simplify/tighten; endeavor → try/attempt; optimize → improve/fine-tune; spearhead → lead/drive; catalyze → trigger/spark; incentivize → encourage/reward; operationalize → put into practice; conceptualize → think through/frame; harness → use/tap/draw on; illuminate → explain/show; differentiate → distinguish/tell apart; refine → improve/tweak; surpass → beat/exceed; boast → has/offers; nestle ("nestled in the heart of") → sits/stands/is; resonate → land/stick/ring true; unlock → open up/make possible; unleash → release/set off; embark → start/begin; empower → let/enable/help; elevate → raise/lift/improve.

**High-severity adjectives:** robust → strong/solid; cutting-edge → new/advanced (or cut); innovative → new/creative (or cut); seamless → smooth/easy; pivotal → key/central; transformative → significant (or cut); game-changing → significant (or cut); crucial → important/essential; holistic → complete/integrated; groundbreaking → new/first (or describe why); unparalleled → rare/exceptional (or cut).

**Moderate-severity adjectives:** profound → deep/far-reaching/serious; renowned → well-known/respected; comprehensive → full/thorough; multifaceted → complex/layered; noteworthy → worth noting; meticulous → careful/detailed; intricate → complex/detailed; commendable → impressive/good; paramount → essential/most important; compelling → convincing/strong; invaluable → valuable/a big help; unwavering → steady/firm; ever-evolving → changing/shifting (or cut).

**High-severity nouns:** realm → area/field; tapestry → mix/blend (especially "rich tapestry"); landscape → field/scene (when metaphorical); synergy → cooperation; paradigm → model/approach; cornerstone → foundation/basis; linchpin → key part; testament → proof/sign; treasure trove → wealth/goldmine; "diverse array" → range/mix (bare "diverse" is an ordinary word and stays); "natural beauty" → name what is actually there; plethora → plenty/many; myriad → many/countless; mosaic → mix/patchwork; symphony → combination/interplay; labyrinth → maze/tangle; cacophony → noise/din; kaleidoscope → shifting mix; odyssey → journey/long haul. Three more are flagged only when metaphorical: beacon → example/signal; bedrock → foundation/basis; crucible → test/proving ground. And "north star" → goal/priority, in the strategy-jargon sense.

**High-severity phrases:** "That being said" → However/But; "At its core" → Fundamentally/Essentially; "To put it simply" → Simply put/In short; "This underscores the importance of" → This shows why; "A key takeaway is" → The main point is; "From a broader perspective" → When you zoom out; "In today's rapidly evolving" → cut entirely and be specific; "In the realm of" → In/Within; "It is important to note that" → cut the preamble, state the fact; "Let's delve into" → just start the section; "Without further ado" → cut entirely; "In conclusion" / "In summary" / "To sum up" / "All in all" → just stop. The reader can see the piece ending; announcing it spends a sentence on navigation. Do not swap one signpost for another.

### Watch the "quiet" collocation

A recent habit is to make everything quietly something. "Quiet confidence." "Quiet rebellion." "The quiet truth." "Quietly reshaping the industry." The modifier borrows gravity without supplying evidence, and it attaches to abstract qualities and transformation verbs rather than to sound. Cut it and say what happened: not "she led with quiet confidence" but "she said little in the meeting and rewrote the roadmap that week." This is the collocation, not the word. A quiet room, a quiet street, closing a door quietly: all fine.

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
- The staccato run: "Not a bug. Not a feature. A fundamental design flaw." Two or three clipped negations stacked before the resolution. What marks it is the noun phrase after *Not*: ordinary emphasis is adverbial ("Not now. Not ever." "Not bad. Not great.") and is fine.
- The fragment: "Not because the person stopped mattering, but because the officer is reachable." A sentence that opens on *Not* and pivots on *but*, with the same word starting both halves ("Not because... but because," "Not to save time, but to save arguments," "Not a strategy, but a habit").

In every case, make the positive claim once and let it stand. Don't negate an alternative just to knock it down. "It's about the judgment" says the whole thing on its own, and "The officer is the reachable point in the system" says it without the rejected half, which usually answers a charge nobody made. Two ordinary constructions look similar and are fine: a sentence where *Not* heads a real subject ("Not all of them agreed, but most did") and the mid-sentence correlative ("He did not go to the store, but to the park"). What marks the tell is the sentence opening on *Not* with both halves starting on the same word.

A related reflex is the **pronouncement frame**: fronting a plain claim with scaffolding that announces its own importance.

- The cleft: "What matters here is the restraint." / "The gap was where the work got lost."
- The thesis opener: "The point of the redesign is to slow people down."
- The maxim closer: ending a section on a short abstract summary like "The craft is mostly restraint."

Lead with the concrete thing instead. "The redesign slows people down" beats "The point of the redesign is to slow people down." Let the reader infer the significance rather than being told it.

### Cut the frame-opener tics

A cluster of fixed openers front a point with empty scaffolding instead of stating it. "When it comes to X, ..." announces a topic and says nothing about it; cut the preamble and make the claim, so "When it comes to pricing, we keep it simple" becomes "Our pricing is simple." "In a world where...", "In an era of..." and the imperative version, "Imagine a world where...", open on a sweeping generalization to sound weighty; open on the specific instead. "That's where X comes in" stages a reveal before naming a product; say what it does directly. And "plays a pivotal role in" (or "a key role in," "a central role in") pads a plain verb, so "Monitoring plays a pivotal role in catching problems" becomes "Monitoring catches problems early." Two more in the same family announce a procedure or hand the reader a comparison instead of doing the work. "Let's break this down." "Let's unpack what this means." "Let's dive into the details." The next paragraph is the breakdown; saying it is coming adds a sentence and no information, so delete the announcement and start. And "Think of it as a Swiss Army knife for your workflow" tells the reader to hold an analogy rather than showing why it fits, and the analogy is usually generic enough to drop into any topic. Give the comparison a job by making the mapping explicit, or describe the thing plainly. Note the scope here, because the neighbouring phrasings are ordinary: "let's be honest" and "let's explore the options" are stance and collaboration, not procedure, and they stay. These sit at the start of a sentence or follow a fixed template, so they are easy to catch once you watch the opening words.

A related move spends a sentence announcing that an insight is coming: "Here's the kicker." "Here's the part most people miss." "What nobody tells you is..." The setup promises a payoff the payoff rarely earns. Lead with the insight itself; if it is genuinely counterintuitive, the reader will notice. Note the narrow scope: the bare marker "Here's the thing" is ordinary casual speech and is recommended elsewhere in this prompt as a human transition. What marks this one is the withheld-insight claim bolted onto it.

### Cut the performative framing beat

A related habit is the beat that exists to perform polish rather than carry content: a move that signals "this is well-crafted" instead of saying one more specific, true thing. These beats are also topic-agnostic, so the same one could drop into almost any piece. Watch for four forms.

The first is the **meta label**: a heading or standalone line that names the piece's own format or length instead of its subject. "In 200 words." "In brief." "The short version." "At a high level." Replace the label with a phrase about the content ("the direction problem"), or cut it and let the section speak for itself. Do not announce structure; let the structure be the structure. This is only the standalone-label case; "in short" used inside a sentence is fine.

The second is the **self-satisfied closer**: a neat aphorism ending a section that adds no new fact, name, or number, often crediting the writer or pivoting on a tidy antithesis. "The data set is public; the reading of it is mine." It overlaps with the maxim closer above; the extra tell is the flourish standing in for a last substantive point. Delete the beat and end on the last real thing you had to say.

The third is **first-person meta-commentary on the work itself** ("my take," "as I see it," "the reading of it is mine") dropped into a piece that is otherwise evidence-led. It performs a stance rather than earning one. Cut it and let the evidence carry the view.

The fourth is the **appended significance label**: a heading or subtitle that names its subject and then annexes a second element whose only job is to promise the subject matters. Sometimes it is a *why* clause pre-defending a choice the body has not made yet, as in "Method, and why this one" (a section called Method was always going to defend its method). Sometimes it is a trailing relative clause asserting a hinge, as in "Reintegration support at the moment of release, and the officer the whole system turns on." Read every label in the piece and ask whether the part after the comma adds a fact or only tells the reader this is important. If it is the second, cut it and let the section earn it. "Method" does the job. One such label may be deliberate; two in one piece is the tell, because a repeated rhetorical shape reads as machine-made even when the words differ. Count that budget across the whole assembled piece rather than section by section. Four sections can each pass with one label while the finished document holds four, which is the shape a reader actually notices.

A clever paradox headline is the borderline case: "Everyone steers the learner but the learner" is fine as a genuine title, a tell when it substitutes for a plain statement of the point. Keep at most one aphoristic or paradox construction per piece, and only where it does analytical work. The device is human in moderation; what marks it as machine-made is repetition and substitution for content, not the device itself.

### Cut the question-fragment beat

Another frontier-model tic is the short question fired off as a setup, then answered in the next breath: "The best part? It's completely free." "The result? A total win." "The catch? You pay upfront." One can land as genuine emphasis, but repeated, the setup-and-payoff rhythm becomes a fingerprint. State the point as a declarative. "It's completely free" says it without the drumroll. This is the noun-phrase-fragment question specifically ("The best part?"); an ordinary question in the flow of the prose is fine.

### Cut the false-candour opener

A one-word question used as an opener promises candour and then delivers a platitude: "Honestly? Most people never follow up." "Frankly? It was never going to work." "Truthfully? Consistency beats talent." The fragment advertises a confession the sentence does not contain. Delete it and state the claim. If the point genuinely is contrarian, it will read as contrarian without the drumroll.

The same performance also arrives appended to the end of a sentence, as a first-person admission tacked onto a statement that was already finished: "The redesign took nine months, and I'm not going to pretend that was the plan." "It shipped late, and I won't pretend otherwise." The clause adds no fact. It asks for credit for honesty while withholding the thing an honest sentence would contain. Cut it and let the statement stand, or replace it with what you are declining to pretend about: "It shipped six weeks late, and the cause was ours." Note the carve-out, because it decides most cases. Starting a sentence with the same words is ordinary hedging and perfectly human: "I'm not going to pretend I understand the tax code" qualifies a claim the writer is about to make. The tell is the appending, not the phrase.

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

### Don't dodge the copula either

The rule above is about sentence shape, not about the word "is." The fix for "X is a Y that Z" is to give the sentence a real verb ("The platform lets teams collaborate"), never to swap "is" for a statelier linking verb. Models do exactly that, and it is one of the most reliable tells there is: "serves as," "stands as," "represents," "marks," "embodies." "The report serves as a guide" is "The report is a guide." "The building stands as a monument to the era" is "The building is a monument to the era," or better, say what it does now. When the plain copula is the honest verb, use it.

Two carve-outs. A person holding an office genuinely "serves as" something ("she serves as chair of the committee"), and several near neighbours carry real meaning the copula cannot: a capacitor functions as a filter, a clinic operates as a registered charity, a board comprises seven members. Keep the substitute wherever it says something "is" would not. The test is whether "is" or "has" would do the same work.

The inflating variant pairs the substitute verb with an abstract noun that asserts importance: "It represents a shift in how the team works." "The award marks a milestone." Nothing in either sentence is checkable. Say what changed and for whom: "The team now reviews before merging, which it did not do in March."

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

The fixed form of this is the balancing hedge: "While automation has benefits, it also carries risks." Both sides get stated, nothing gets concluded, and no one pays a cost. If the trade-off is real, name the specific cost and who bears it: "Automation cut our deploy time in half and broke two rollbacks in the first month." If it isn't, pick the claim you actually want to make.

### Allow negative emotions

Frustration, skepticism, disappointment, and concern are human. AI softens them. Vary sentiment across paragraphs: enthusiastic in one, cautious in the next, blunt in a third.

### Build emotion through detail, not labels

Instead of "This was a deeply frustrating experience," show frustration building through increasingly specific detail and shorter sentences. Use emotion words sparingly but precisely.

### Cut unsolicited reassurance

A recent habit, strongest in chat-tuned models, is to reassure the reader without being asked: "You're not alone." "You're not imagining it." "You're not broken." "It's not just you." Dropped into a business post, a doc, or an essay, it reads as therapeutic filler that performs empathy in place of saying anything. Cut it, or replace it with the specific thing worth saying. If the piece genuinely calls for reassurance, make it concrete ("plenty of teams hit this same wall in month two") rather than a canned "you're not X" formula.

A close relative opens on a manufactured shared struggle: "If you've ever struggled with slow deploys, you know the pain." It fakes relatability with a canned second-person conditional before it has earned any. Lead with the concrete stake instead ("Slow deploys waste hours every week"). An ordinary conditional that recalls a real shared experience ("If you've ever been to Paris, you know the traffic") is fine; the tell is the empathy-hook opener bolted to the front of a piece.

The same family includes the instruction to feel something: "Let that sink in." "Read that again." "Do you want to sit with that for a while?" "Are you ready to go deeper?" These ask for weight instead of supplying it. Delete them. If the point deserves weight, give it a fact or a consequence: "Only three of the twelve shipped" needs no instruction after it.

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

The same tidiness shows up as constant self-reference: "As mentioned above." "As we discussed earlier." "As noted previously." "As we have seen." "As we established earlier." Cut them, or restate the point in three words. A long reference document sometimes needs a genuine back-pointer; a piece of prose almost never needs one every other paragraph. Watch the shape rather than the words: the tell is a cross-reference standing on its own before a comma, so "as we have seen the results, we can decide" is an ordinary subordinate clause and is fine.

The closing move is the same habit pointed forward: "In conclusion." "To sum up." "In summary." "All in all." The reader can see the piece ending. Cut the signpost and state the last point; if the closing paragraph needs an announcement to read as closing, it is not closing anything. This one is genuinely conventional in academic and formal report writing, so it is a judgment call there rather than a prohibition.

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

Metaphorical "carry" is the most frequent version of this and the hardest to hear, because it sounds like craft. "The layout carries the weight of the argument." "The silence carried the room." "Eight words to carry." The verb performs gravity while the sentence names no actor and no effect. Say what the thing actually does: "the layout is what makes the argument land," or, for the label form, "eight words, and they have to do the whole job." Literal carrying is fine, and so is a truck carrying a load; the tell is an abstraction carrying an abstraction. The subject does not have to be as abstract as "the layout" for this to read as machine-made. A process or a project in the subject slot does it too: "the rebuild carries the argument," "the rollout carries the message," "the migration carries the lessons from the last one." Name who made the argument, or say where it actually sits. One carve-out worth knowing: "carries risk," "carries a cost," "carries weight with the board" and "carries consequences" are ordinary business and legal English, not tells, and rewriting them makes the prose stranger rather than more human.

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
4. **Antithesis and negative parallelism:** "not just X, but also Y" → simple conjunction. "It's not X, it's Y," including the two-sentence version ("...is not Y. It is Z.") and the fragment ("Not because X, but because Y."), → state the point directly. See "Kill the antithesis reflex" above for the full family.
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
- Appended significance labels: a heading or subtitle that names its subject and then annexes a clause promising the subject matters ("Method, and why this one," "..., and the officer the whole system turns on"). Check every label, not just the body, and count them across the assembled piece rather than one section at a time.
- The antithesis fragment: a sentence opening on *Not* and pivoting on *but* with the same word starting both halves ("Not because X, but because Y").
- The unsolicited-reassurance frame ("You're not alone," "It's not just you") and the question-fragment beat ("The best part? ..."), unless the piece genuinely earns one.
- The frame-opener tics ("When it comes to X," "In a world where," "That's where X comes in," "plays a pivotal role in"), the manufactured-empathy opener ("If you've ever struggled with..."), and the withheld-insight teaser ("Here's the kicker," "the part most people miss").
- Metaphorical "carry" with an abstract subject ("carries the weight," "carries the burden," "words to carry") or a process in the subject slot ("the rebuild carries the argument"), and the "quiet X" / "quietly reshaping" collocation. "Carries risk" and "carries a cost" are ordinary English and stay.
- The false-candour opener ("Honestly?" "Frankly?"), the instruction to feel something ("Let that sink in"), and the balancing hedge ("While X has benefits, it also carries risks").
- Copula dodges: "serves as," "stands as," "represents a shift," "marks a milestone" where "is" would do. Keep the substitute only where it says something "is" cannot ("she serves as chair," "the board comprises seven members").
- The signposted conclusion ("In conclusion," "To sum up," "All in all") and the self-reference that points backward ("As we have seen"). Both spend a sentence on navigation.
- The staccato negation run ("Not a bug. Not a feature."), the instructed analogy ("Think of it as a..."), and the announced procedure ("Let's break this down," "Let's unpack").
- The appended candour disclaimer: a first-person admission tacked onto a finished statement ("..., and I'm not going to pretend that was the plan"). Starting a sentence that way is ordinary hedging; appending it is the tell.
- Tidy self-reference ("as mentioned above," "as we discussed earlier") outside a genuine reference document.
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
