# Human-Patterned Language (HPL) Editing Prompt

> **How to use:** Copy this entire document into a new conversation with any LLM (Claude, ChatGPT, Gemini, etc.). Paste the text you want edited below the `=====` line at the bottom. The LLM will rewrite your text to reduce detectable AI patterns while preserving your meaning and intent.

---

Edit the text below "=====" following these rules. Your goal is to make the text read as if a specific, opinionated human wrote it, not to make it "sound more human" in a generic way. Apply rules **unevenly**: some paragraphs should change a lot, others barely at all. Uniform application of human-patterning rules is itself an AI signal.

## Core principle

The single most detectable property of AI text is **consistency**, and it shows most as a repeated shape: the same closer, the same contrast, the same transition in every section. Human text is locally inconsistent while staying globally coherent. Apply every rule below selectively.

Where the signal lives has shifted as models improve. Frontier models now match human writing on the surface statistics that are easy to count: word frequencies, part-of-speech mix, readability scores. They still diverge in two harder places. One is the flow of the text, the moment-to-moment unpredictability of which word comes next. The other is variation between sections: a human writer's style shifts between the opening, the middle, and the close, while a model holds one even fingerprint the whole way through.

This changes how to prioritize. Swapping AI-flagged words for plainer ones is necessary hygiene, but its ceiling is low, and newer models are already crossing it. The stock structural shapes (closers, contrast pairs, framing beats) and the habits of discourse are the durable signals, followed by tone. When you have to choose where to spend effort, weight those above vocabulary substitution, and add nothing to the text just to make it look human.

## Facts come from the user or the source

These rules change how a text is written, never what it says. When you rewrite, keep every claim, name, number, date, quotation and stance. Add no fact, and neither soften nor harden a claim, so a hedge the source has stays and a firm claim stays firm. If a rule below cannot be applied to a passage without changing its meaning, skip that rule there.

The same holds when you draft text that will be read as fact about a real person, organisation, product or source (a cover letter, a bio, a case study, a report, a citation). Every name, number, date, quotation and first-person experience in it comes from the user or the source. When the piece needs one that is missing, leave a marked placeholder such as [number] so the draft still arrives, and ask only when the draft cannot stand without it. Never invent one to make the text feel specific. Fiction, and requests that ask for an invented example, are exempt.

## 1. Vocabulary

### Replace AI-correlated words

These words appear at statistically elevated rates in AI text. Replace them with plainer alternatives, but not every instance, and not mechanically.

**High-severity verbs:** delve → dig into/examine; leverage → use/rely on; utilize → use; facilitate → help/enable; bolster → strengthen/support; showcase → show/display; garner → earn/attract; foster → encourage/build; enhance → improve/boost; elucidate → explain/clarify; revolutionize → change/reshape; synergize → combine/work together; underscore → show/point to.

**Moderate-severity verbs:** navigate → work through/handle; streamline → simplify/tighten; endeavor → try/attempt; optimize → improve/fine-tune; spearhead → lead/drive; catalyze → trigger/spark; incentivize → encourage/reward; operationalize → put into practice; conceptualize → think through/frame; harness → use/tap/draw on; illuminate → explain/show; differentiate → distinguish/tell apart; refine → improve/tweak; surpass → beat/exceed; boast → has/offers (the tell is "boasts a/an/over X" as a feature brag; "boast of" and "boast about" are ordinary English and stay); nestle ("nestled in the heart of") → sits/stands/is; resonate → land/stick/ring true; unlock → open up/make possible; unleash → release/set off; embark → start/begin; empower → let/enable/help; elevate → raise/lift/improve (the tell is "elevate your X" and "elevate the experience"; literal raising, and "elevated rates", stay).

**High-severity adjectives:** robust → strong/solid; cutting-edge → new/advanced (or cut); innovative → new/creative (or cut); seamless → smooth/easy; pivotal → key/central (inside "plays a pivotal role," rewrite the verb instead; see the frame-opener tics); transformative → significant (or cut); game-changing → significant (or cut); crucial → important/essential; holistic → complete/integrated; groundbreaking → new/first (or describe why); unparalleled → rare/exceptional (or cut).

**Moderate-severity adjectives:** renowned → well-known/respected; comprehensive → full/thorough; multifaceted → complex/layered; noteworthy → worth noting; meticulous → careful/detailed; intricate → complex/detailed; commendable → impressive/good; paramount → essential/most important; compelling → convincing/strong; invaluable → valuable/a big help; unwavering → steady/firm; ever-evolving → changing/shifting (or cut); palpable → obvious/thick (or name what people could see or hear: "the tension was palpable" is the usual offender); unspoken → say what was left unsaid, or cut.

**High-severity nouns:** realm → area/field; tapestry → mix/blend (especially "rich tapestry"); landscape → field/scene (when metaphorical); synergy → cooperation; paradigm → model/approach; cornerstone → foundation/basis; linchpin → key part; testament → proof/sign; treasure trove → wealth/goldmine; "diverse array" → range/mix (bare "diverse" is an ordinary word and stays); "natural beauty" → name what is actually there; plethora → plenty/many; myriad → many/countless; mosaic → mix/patchwork; symphony → combination/interplay; labyrinth → maze/tangle; cacophony → noise/din; kaleidoscope → shifting mix; odyssey → journey/long haul. Three more are flagged only when metaphorical: beacon → example/signal; bedrock → foundation/basis; crucible → test/proving ground. And "north star" → goal/priority, in the strategy-jargon sense. Two lower-severity nouns that some models produce at over a hundred times the human rate: camaraderie → friendship/the way they worked together; unease → worry/nerves ("uneasiness" is a different, older word and is fine).

**High-severity phrases:** "That being said" → However/But; "At its core" → Fundamentally/Essentially; "To put it simply" → cut the preamble and say it simply; "This underscores the importance of" → This shows why; "A key takeaway is" → One lesson is, or state the lesson; "From a broader perspective" → When you zoom out; "In today's rapidly evolving" → cut entirely and be specific; "In the realm of" → In/Within; "It is important to note that" → cut the preamble, state the fact; "Let's delve into" → just start the section; "Without further ado" → cut entirely; "In conclusion" / "In summary" / "To sum up" / "All in all" → just stop. The reader can see the piece ending; announcing it spends a sentence on navigation. Do not swap one signpost for another.

### Watch the "quiet" collocation

A recent habit is to make everything quietly something. "Quiet confidence." "Quiet rebellion." "The quiet truth." "Quietly reshaping the industry." The modifier borrows gravity without supplying evidence, and it attaches to abstract qualities and transformation verbs rather than to sound. Cut it and say what happened: not "she led with quiet confidence" but "she said little in the meeting and rewrote the roadmap that week." This is the collocation, not the word. A quiet room, a quiet street, closing a door quietly: all fine.

### Cut credibility insistence

AI-assisted writing often vouches for its own account by insisting the thing is *real*, *actual*, *genuine*, or *truly* so. A human rarely needs to say their own work is real; the specifics carry that. The tell is density, not any single use: the same reality word recurring across a piece reads as a writer arguing for their own credibility.

If *real* / *really* / *actual* / *actually* / *genuine* / *truly* / *authentic* shows up three or more times, cut all but at most one. Replace each with the specific that earned it: "a real engagement" → "a live, mid-build engagement"; "the real flow" → "the flow the operators actually follow." Keep a single use only where it draws a contrast, such as real versus hypothetical, and make that contrast explicit. Ordinary compounds like *real-time*, *real estate*, and *real-world* do not count.

### Fix nominalization

AI converts verbs into noun forms, creating dense bureaucratic phrasing. Unpack nouns back into verbs when the agent is known.

- "the implementation of X" → "we implemented X"
- "the optimization of resources" → "improving how resources were used"
- "the establishment of" → "set up / created"
- "a demonstration of" → "showed / demonstrated"

Two or more "the [noun] of [noun]" phrases in one sentence is a strong AI signal. Three nominalizations in two sentences reads as AI.

### Prefer concrete nouns over abstract ones

AI gravitates toward abstract containers: "framework," "methodology," "ecosystem," "landscape," "stakeholders." Human writers name the concrete thing. "Factors" → name them. "Challenges" → describe one. "Stakeholders" → say who. "Resources" → specify which.

### Keep the adverbs that calibrate a claim

Many models underuse manner and degree adverbs, but not all: GPT-4o overuses "barely" and "nearly" while Llama models avoid them, so the tell is an adverb that carries no judgment, whatever the count. Where the source says how far a claim holds ("mostly," "barely," "roughly"), keep that adverb, because it carries the writer's assessment. Don't add one the source lacks, since that softens or hardens the claim. Generic intensifiers such as "significantly" and "effectively" carry no judgment; cut them, or give the figure the source has. Three adverbs this prompt flags elsewhere are never the fix: "quietly" (the "quiet" collocation), "actually" (credibility insistence) and "honestly" (the false-candour opener).

### Fix hedging uniformity

A single hedge is ordinary; uniform hedging is the tell. If every paragraph carries a stock qualifier ("Generally speaking," "Typically," "Tends to," "Broadly speaking," "To some extent," "Arguably"), the text reads as AI. Keep each hedge the source has, because it marks how sure the writer is, and dropping it hardens the claim. Swap a stock wording for a plain one that marks the same limit, so "Typically" becomes "Usually," and cut a qualifier only where it marks no limit the source states. Where several stack on one claim, keep the one that marks the source's limit.

### Use the same word for the same thing

- Use the same word for the same thing. Rotating synonyms to avoid a repeat is its own tell (see "Elegant variation" below).
- Replace generic nouns with specific ones.
- Don't reach for a rare word for its own sake. Whether AI text is less lexically diverse than human text depends on the model (some current models score higher), so diversity is not a target. What reads as machine-made is the same marked expression recurring; a low count of distinct words does not.
- Mix short plain words with longer ones. A passage of all long words reads as AI.
- Keep the source's contractions where they are. Uneven use is normal, so don't even it out or manufacture it.

## 2. Structure

### Let sentence length follow the content

AI concentrates sentence lengths in a narrow band. The average length is not itself the tell, and studies disagree on which direction it even runs. Don't aim for an average or a spread. A sentence runs as long as the thought it carries, so don't plan a mix of short and long sentences for each paragraph; some paragraphs will read evenly, and that is fine.

- Keep a fragment only where the content calls for one, such as the answer to a question someone asked, or speech. A fragment placed after a long sentence to create a beat reads as performed rhythm, and so does a one-line question added for effect. Fold either into the sentence before it.
- Allow long sentences when the thought demands it. Sometimes a single long sentence with embedded clauses reads more naturally than three short ones.
- Let paragraph length follow the content too. A point that needs one sentence gets a one-sentence paragraph, and a point that needs six sentences gets six. Don't set a single line apart for impact when its point belongs in the paragraph before.
- When a run of sentences sounds flat, look for one shape repeated, and recombine or split those sentences by meaning. Adding short sentences to break up the run does not fix it.

### Let each section read the way its job needs

This works above the level of the sentence. Different parts of a piece do different jobs, and a human writer's prose follows them. An introduction reads more easily because its reader needs the way in, a technical core runs denser, and a set of instructions can stay short and uniform. Left alone, a model keeps the same texture from the first line to the last, and the most visible sign is one shape repeated: the same closer, the same contrast, the same transition in every section. Fix the repeated shape, and let each section's texture follow its job. Don't make sections differ just to show contrast; variation added for its own sake is as mechanical as none.

### Kill the antithesis reflex

The most characteristic move in LLM prose is the flip: state what something is *not*, then pivot to what it *is*. It comes in several surface forms, and single-sentence fixes miss the two-sentence versions.

- The copula flip: "It's not about the tools. It's about the judgment." It comes contracted or not ("It isn't a tool. It's a partner." "It is not a feature; it is a platform."), closed by a period or a semicolon. Count it across the whole piece. One can be an ordinary correction ("It isn't Tuesday. It's Wednesday."); two or more is the reflex, even when each looks reasonable where it stands.
- The hedged aphorism: "The hard part is rarely the code. It's deciding what to build."
- The disclaimer reversal: "I won't pretend this is easy. But it's worth it."
- The verb mirror: "AI carries the busywork. It never carries the judgment."
- The staccato run: "Not a bug. Not a feature. A fundamental design flaw." Two or three clipped negations stacked before the resolution. What marks it is the noun phrase after *Not*: ordinary emphasis is adverbial ("Not now. Not ever." "Not bad. Not great.") and is fine.
- The inline pair: "The work is judgement, not process." A copula, a short noun phrase, a comma, then the rejected twin closing the sentence. Watch the reflex rather than the single instance. One contrast is ordinary writing, and a sentence whose job is to fix a scope ("The unit is the collocation, not the word.") or correct a fact ("The response was 406, not 421.") is legitimate and stays. What marks the tell is reaching for the same binary in section after section, usually with an abstract noun on both sides and nothing concrete in either.
- The graded contrast: "The role is less like a manager and more like a translator." "It's less about speed and more about trust." A plain description recast as a correction of a view nobody stated. Say what the thing is: "Most of the job is translating between the two teams." One "less about X, more about Y" is ordinary writing; reaching for it twice in one piece is the tic. The "less like ... more like" form is the stronger tell, at up to a hundred times the human rate in one current model.
- The fragment: "Not because the person stopped mattering, but because the officer is reachable." A sentence that opens on *Not* and pivots on *but*, with the same word starting both halves ("Not because... but because," "Not to save time, but to save arguments," "Not a strategy, but a habit").

In every case, make the positive claim once and let it stand. Don't negate an alternative just to knock it down. "It's about the judgment" says the whole thing on its own, and "The officer is the reachable point in the system" says it without the rejected half, which usually answers a charge nobody made. Two ordinary constructions look similar and are fine: a sentence where *Not* heads a real subject ("Not all of them agreed, but most did") and the mid-sentence correlative ("He did not go to the store, but to the park"). What marks the tell is the sentence opening on *Not* with both halves starting on the same word.

A related reflex is the **pronouncement frame**: fronting a plain claim with scaffolding that announces its own importance.

- The cleft: "What matters here is the restraint." / "The gap was where the work got lost."
- The thesis opener: "The point of the redesign is to slow people down."
- The maxim closer: ending a section on a short abstract summary like "The craft is mostly restraint." Its balanced twin is "Gardening is as much about patience as technique."
- The importance flag: "This distinction matters because...", "Knowing which type you have matters more than most beginners realize", or a heading "Why this matters". It announces that a point matters instead of showing the consequence. Give the consequence: "Teams mix the two up, and then the audit fails."

Lead with the concrete thing instead. "The redesign slows people down" beats "The point of the redesign is to slow people down." Let the reader infer the significance rather than being told it.

### Cut the frame-opener tics

A cluster of fixed openers front a point with empty scaffolding instead of stating it. "When it comes to X, ..." announces a topic and says nothing about it; cut the preamble and make the claim, so "When it comes to pricing, we keep it simple" becomes "Our pricing is simple." "In a world where...", "In an era of..." and the imperative version, "Imagine a world where...", open on a sweeping generalization to sound weighty; open on the specific instead. "That's where X comes in" stages a reveal before naming a product; say what it does directly. And "plays a pivotal role in" (or "a key role in," "a central role in") pads a plain verb, so "Monitoring plays a pivotal role in catching problems" becomes "Monitoring catches problems early." Two more in the same family announce a procedure or hand the reader a comparison instead of doing the work. "Let's break this down." "Let's unpack what this means." "Let's dive into the details." The next paragraph is the breakdown; saying it is coming adds a sentence and no information, so delete the announcement and start. And "Think of it as a Swiss Army knife for your workflow" tells the reader to hold an analogy rather than showing why it fits, and the analogy is usually generic enough to drop into any topic. Give the comparison a job by making the mapping explicit, or describe the thing plainly. Note the scope here, because the neighbouring phrasings are ordinary: "let's be honest" and "let's explore the options" are stance and collaboration, not procedure, and they stay. These sit at the start of a sentence or follow a fixed template, so they are easy to catch once you watch the opening words.

A related move spends a sentence announcing that an insight is coming: "Here's the kicker." "Here's the part most people miss." "What nobody tells you is..." The setup promises a payoff the payoff rarely earns. Lead with the insight itself; if it is counterintuitive, the reader will notice. The target here is the withheld-insight claim. The bare marker "Here's the thing" is ordinary casual speech, so leave it where the writer used it, and don't add it as a transition either (see "Cut stock transitions" under Discourse).

### Cut the performative framing beat

A related habit is the beat that exists to perform polish rather than carry content: a move that signals "this is well-crafted" instead of saying one more specific, true thing. These beats are also topic-agnostic, so the same one could drop into almost any piece. Watch for four forms.

The first is the **meta label**: a heading or standalone line that names the piece's own format or length instead of its subject. "In 200 words." "In brief." "The short version." "At a high level." Replace the label with a phrase about the content ("the direction problem"), or cut it and let the section speak for itself. Do not announce structure; let the structure be the structure. This is only the standalone-label case; "in short" used inside a sentence is fine.

The second is the **self-satisfied closer**: a neat aphorism ending a section that adds no new fact, name, or number, often crediting the writer or pivoting on a tidy antithesis. "The data set is public; the reading of it is mine." It overlaps with the maxim closer above; the extra tell is the flourish standing in for a last substantive point. Delete the beat and end on the last real thing you had to say. Short copy (worksheet cells, captions, bullet notes) has two compressed versions. One is the clipped verdict, a noun phrase plus "stays" or "remains" and a full stop that performs a decision: "Tutoring stays." "The Scouts books and the tutoring stay." Say who decided: "I am keeping the Scouts books and the tutoring." The other is the stance closer that points back at a number already given: "Seven to eight hours of sleep, and I want to keep it there." Replace it with the next concrete fact. "The car stays in the garage" is ordinary English, because the sentence goes on to say where. Captions have a numeric version, a verbless pair that sets one against many: "One count, four moments." "Three sizes, all the same height." "One app, every chat." Say what the picture shows: "The badge turns red when a message arrives and grey once you've seen it." The same shape is ordinary in terse practical writing ("Two tablets, every four hours." "Two adults, one child."), so judge it by whether it is selling something. A maxim that hands the verdict to someone else is the closer again: "A design that ignores the build comes back, and the developer is right to send it back."

The third is **first-person meta-commentary on the work itself** ("my take," "as I see it," "the reading of it is mine") dropped into a piece that is otherwise evidence-led. It performs a stance rather than earning one. Cut it and let the evidence carry the view.

The fourth is the **appended significance label**: a heading or subtitle that names its subject and then annexes a second element whose only job is to promise the subject matters. Sometimes it is a *why* clause pre-defending a choice the body has not made yet, as in "Method, and why this one" (a section called Method was always going to defend its method). Sometimes it is a trailing relative clause asserting a hinge, as in "Reintegration support at the moment of release, and the officer the whole system turns on." Read every label in the piece and ask whether the part after the comma adds a fact or only tells the reader this is important. If it is the second, cut it and let the section earn it. "Method" does the job. One such label may be deliberate; two in one piece is the tell, because a repeated rhetorical shape reads as machine-made even when the words differ. Count that budget across the whole assembled piece rather than section by section. Four sections can each pass with one label while the finished document holds four, which is the shape a reader actually notices.

A clever paradox headline is the borderline case: "Everyone steers the learner but the learner" is fine as a genuine title, a tell when it substitutes for a plain statement of the point. Keep at most one aphoristic or paradox construction per piece, and only where it does analytical work. The device is human in moderation; what marks it as machine-made is repetition and substitution for content, not the device itself.

### Cut the question-fragment beat

Another frontier-model tic is the short question fired off as a setup, then answered in the next breath: "The best part? It's completely free." "The result? A total win." "The catch? You pay upfront." One can land as genuine emphasis, but repeated, the setup-and-payoff rhythm becomes a fingerprint. State the point as a declarative. "It's completely free" says it without the drumroll. This is the noun-phrase-fragment question specifically ("The best part?"); an ordinary question in the flow of the prose is fine.

### Cut the false-candour opener

A one-word question used as an opener promises candour and then delivers a platitude: "Honestly? Most people never follow up." "Frankly? It was never going to work." "Truthfully? Consistency beats talent." The fragment advertises a confession the sentence does not contain. Delete it and state the claim. If the point genuinely is contrarian, it will read as contrarian without the drumroll.

The same performance also arrives appended to the end of a sentence, as a first-person admission tacked onto a statement that was already finished: "The redesign took nine months, and I'm not going to pretend that was the plan." "It shipped late, and I won't pretend otherwise." The clause adds no fact. It asks for credit for honesty while withholding the thing an honest sentence would contain. Cut it and let the statement stand, or replace it with what you are declining to pretend about: "It shipped six weeks late, and the cause was ours." Note the carve-out, because it decides most cases. Starting a sentence with the same words is ordinary hedging and perfectly human: "I'm not going to pretend I understand the tax code" qualifies a claim the writer is about to make. The tell is the appending, not the phrase.

### End on the last fact, not a forecast

Expert readers name the ending as one of their leading clues to AI text: model endings are "repetitive and overly optimistic summaries," while human ones stop more abruptly. The fixed forms sit in the final paragraph: "As the field continues to evolve, ...", "Looking ahead, ...", "One thing is clear: ...", "The future of X looks bright." End on the last concrete fact ("The council votes in March.") and cut the forecast unless it names a concrete time: a date, a number, a weekday, or "tonight" or "tomorrow" ("Looking ahead, the forecast calls for rain through Thursday" is a weather report, not a summary). The same phrases in the body of a piece, where they introduce a plan, are fine, and so is a neutral open question at the end of a news story ("It remains to be seen whether the Senate will take up the bill"): the tell is the upbeat summary, not the open ending.

### Vary sentence structure

- Choose the construction the thought needs, simple or complex. A run of sentences built the same way is the tell, whatever their length.
- Start a sentence with "And" or "But" where it joins on to the one before. Don't add one for effect.
- Order clauses so the emphasis falls where the point is. "Despite the cost, they went ahead" stresses the decision; "They went ahead, despite the cost" stresses the cost.

### Reduce that-clause subjects

AI produces "That the system performed well is noteworthy." Human writers almost never start sentences this way. Restructure it as "The system performed well, which is worth noting," or state the fact and stop ("The system performed well.").

### Cut trailing participial clauses

AI appends "-ing" tails that add interpretation without new information: "...contributing to the socio-economic development of the area and underscoring its enduring significance." If the participial clause can be deleted without losing a fact, delete it.

### Cut the noun-participle fragment

The past-participle cousin of the trailing "-ing" tail is a whole verbless sentence: a noun phrase, a comma, and a past participle standing in for a verb. "The same board, rebuilt." "The homepage, reimagined." "The whole system, rewritten." It reads as AI copy because it strikes a pose instead of making a claim. Give it a subject and a real verb ("We rebuilt the same board.") or fold the participle into the sentence beside it. This is only the fragment form; a participle inside a full sentence is fine ("The board, which we rebuilt, is live.").

### Cut the cause-to-benefit "so" tail

Product and portfolio copy picks up a brochure habit: state a mechanism, then append ", so" and the payoff it promises the reader. "Quip updates itself, so a fix reached people within a day of shipping." "Only the width changes, so the window stays under the menu-bar icon and nothing jumps away from the pointer." The second half exists to tell you the first half was good. Keep one half, usually the fact or what the user actually sees, and cut the sales pitch. Keep the "so" when the reader needs the causal link to follow the argument ("The server was down, so the backup ran from the laptop."). Starting a sentence with "So," as a transition is fine too; that is one of the plain bridges under "Cut stock transitions."

### Replace periphrastic verbs with direct verbs

- "is able to process" → "processes"
- "has been shown to improve" → "improves"
- "can be used to generate" → "generates"
- "is designed to facilitate" → "helps"

Audit for auxiliary verb chains (is/are/was/were/has/have/can/could + past participle). If a single verb would work, use it.

### Reduce copula overuse

AI defaults to "X is a Y that Z." "The platform is a tool that enables collaboration" → "The platform lets teams collaborate." Not every copula should go. When three sentences in a row use "is/are/was" as the main verb, check whether one of them has a stronger verb available.

### Don't dodge the copula either

The rule above is about sentence shape, not about the word "is." The fix for "X is a Y that Z" is to give the sentence a real verb ("The platform lets teams collaborate"), never to swap "is" for a statelier linking verb. Models do exactly that, and it is one of the most reliable tells there is: "serves as," "stands as," "represents," "marks," "embodies." "The report serves as a guide" is "The report is a guide." "The building stands as a monument to the era" is "The building is a monument to the era," or better, say what it does now. When the plain copula is the honest verb, use it.

Two carve-outs. A person holding an office genuinely "serves as" something ("she serves as chair of the committee"), and several near neighbours carry real meaning the copula cannot: a capacitor functions as a filter, a clinic operates as a registered charity, a board comprises seven members. Keep the substitute wherever it says something "is" would not. The test is whether "is" or "has" would do the same work.

The inflating variant pairs the substitute verb with an abstract noun that asserts importance: "It represents a shift in how the team works." "The award marks a milestone." Nothing in either sentence is checkable. Say what changed and for whom: "The team now reviews before merging, which it did not do in March."

### Fix enumeration overuse

Three-item parallel lists in sequence are a strong AI signal. Vary list lengths: sometimes two items, sometimes four. Embed items in flowing prose rather than enumerating, and where the source ranks them, say so.

Replace coordination with subordination when one item matters more: "The team designed, developed, and deployed the system" → "The team designed and deployed the system; developing it took most of the time."

### Keep related words close together

Human languages minimize the distance between syntactically linked words due to working memory constraints. LLMs do this less effectively. If the subject and verb are separated by 8+ words of modifying phrases, restructure. Move heavy modifiers to the end of the sentence.

### Punctuate for the sentence

**Do not use em-dashes (—).** They read as an AI tell, and this prompt bans them outright. Replace an em-dash parenthetical with commas or parentheses. Where a dash joins two clauses, use a period, or a semicolon when the clauses are closely joined; a bare comma there is a splice. If the dash staged a reveal, put the point first instead of moving the reveal to a colon. Em-dash frequency varies enormously by model, so a text with no em-dashes is not therefore human, and their presence alone is weak evidence either way. Remove them anyway, for how they read, but don't lean on them as a detector.

Choose the other marks for the sentence in front of them. A colon introduces a list or a definition ("Bring three things: a pen, your ID and the signed form."); never use one to stage a reveal, where the words before it only set up the point after it. Where the source makes different valid choices in different places (an Oxford comma here, none there), keep them, and don't add variety to text that has none.

## 3. Tone and sentiment

### Don't flatten strong positions

AI defaults to "on the other hand" balance even when the text doesn't call for it. Let positions be stated with conviction. "This approach has serious problems" is more human than "This approach presents certain challenges that merit consideration."

The fixed form of this is the balancing hedge: "While automation has benefits, it also carries risks." Both sides get stated, nothing gets concluded, and no one pays a cost. If the trade-off is real, name the specific cost and who bears it: "Automation cut our deploy time in half and broke two rollbacks in the first month." If it isn't, pick the claim you actually want to make.

### Keep negative emotions

Frustration, skepticism, disappointment, and concern are human. AI softens them. Keep the negative sentiment the source has, at the strength it has it, and let the tone shift where the content shifts. Don't give a paragraph a mood for variety.

### Build emotion through detail, not labels

Instead of "This was a deeply frustrating experience," show frustration building through increasingly specific detail and shorter sentences. Use emotion words sparingly but precisely.

Two fiction habits are the same failure in miniature. One names a feeling as an inventory: "She felt a mix of pride and sadness," "a strange blend of relief and dread," "the weight of the unspoken." Show the two feelings through what the person does or says. The other reaches for the stock phrases nearly every current model over-produces: "her voice barely above a whisper," "his heart hammering against his ribs," "the air thick with the scent of," "a smile playing on her lips," "eyes never leaving her face," "casting long shadows." Two more from the same lists, "couldn't shake the feeling" and "a profound sense of," are everyday English outside fiction, so treat them as tells only in a story. Replace each with what this character in this scene would actually do or notice. Rename a character called Elara or Kael, and don't let a model's default names (Emily, Sarah, Dr. Chen) through unless the source gave them. And don't explain what a line has already shown: "He slammed the door. He was angry." loses nothing when the second sentence goes.

### Cut unsolicited reassurance

A recent habit, strongest in chat-tuned models, is to reassure the reader without being asked: "You're not alone." "You're not imagining it." "You're not broken." "It's not just you." Dropped into a business post, a doc, or an essay, it reads as therapeutic filler that performs empathy in place of saying anything. Cut it, or replace it with the specific thing worth saying. If the piece genuinely calls for reassurance, make it concrete ("plenty of teams hit this same wall in month two") rather than a canned "you're not X" formula.

A close relative opens on a manufactured shared struggle: "If you've ever struggled with slow deploys, you know the pain." It fakes relatability with a canned second-person conditional before it has earned any. Lead with the concrete stake instead ("Slow deploys waste hours every week"). An ordinary conditional that recalls a real shared experience ("If you've ever been to Paris, you know the traffic") is fine; the tell is the empathy-hook opener bolted to the front of a piece. Its cousin is "If this sounds familiar, take heart" (or "you're not alone", "don't worry"). A callback is fine: "If this sounds familiar, it's because I wrote about it last week."

The same family includes the instruction to feel something: "Let that sink in." "Read that again." "Do you want to sit with that for a while?" "Are you ready to go deeper?" These ask for weight instead of supplying it. Delete them. If the point deserves weight, give it a fact or a consequence: "Only three of the twelve shipped" needs no instruction after it.

### Don't narrate your own backstory or praise your own habits

In bios, About pages, résumés and cover letters, drafts tell the writer's history as a tidy sequence and describe their habits approvingly. "Ten years of teaching neurodivergent and multilingual learners came first, and so did the habit of watching where people get stuck." "Before them came two web tools for English learners." "I design the screens, build them in code, and keep the Figma files behind them tidy." "People I've never met use it." Each one performs modesty or craft instead of stating something. Give the fact with its date or number ("Teaching neurodivergent and multilingual learners since 2016.") and drop the adjective about yourself. A first-person position is still welcome (see "Use the plain defaults"); the tell is the voice admiring its own work.

### Write product copy for someone who has never used the product

Case studies, landing pages and release notes are read by strangers. Ask of each sentence whether someone who has never opened the product would follow it on first read. Three failures recur. The first explains the mechanism in a chain of clauses instead of saying what the user gets: "Show them in every space and they stay at the top of the sidebar, with one sign-in and one unread count, while the rest of the list changes." One subordinate clause is fine (see "Prefer subordination over coordination"); three stacked onto a mechanism is the problem. The second uses the product's own internal words, or verbs users never say: "cut across all of them," "filing a GIF" (nobody files GIFs). This is not the same as domain vocabulary. Use a real term of the field, such as "notification fatigue," where it is the right word, and define any product concept before you use it. The third is a slogan whose second half is clever and impossible to picture: "Every chat and inbox in one Mac window, and only what's new turns red." Also cut vague casual counts ("a dozen or so testers"), run-in labels ("The worst bug:"), and release-by-release history ("first release 13 July").

### Match readability to audience

AI writes at a uniformly elevated grade level regardless of audience. Write for the reader the piece is for. A blog post or a marketing page should read more easily than a professional report, and a report more easily than a research paper. Within a document, let the difficulty of a passage follow its job, so explanation stays simple and analysis can run denser.

### Use exclamation marks sparingly

AI almost never uses them. In informal content, keep an exclamation mark the source has where it marks emphasis the writer meant. Don't add them, and don't use them in formal prose.

## 4. Discourse and cohesion

### Cut stock transitions

Not every paragraph needs a transition. AI over-signals connections. Drop "Furthermore," "Additionally," "Moreover," "Notably," "Importantly," "Consequently." Usually the fix is to start the next point; the reader follows the logic. Where a bridge is needed, use a plain one, such as "So," "But" or "Then."

### Prefer subordination over coordination

AI overuses "and" and "but." Use a subordinating conjunction where the relation between two clauses is causal, temporal, conditional or concessive (because, since, when, if, unless, although). It shows that the writer has judged how the ideas relate. Not every "and" needs replacing, but three coordinated clauses in a row is a pattern to break.

### Reduce over-explicit cohesion

AI writes "This approach enables... This enables... This in turn enables..." Human writers let some sentences stand alone, and let some paragraphs start fresh, opening on an example instead of a topic sentence that links to the previous paragraph.

That chain is the commonest machine form of a wider habit: three or more consecutive sentences opening on the same word or the same two words. "They assume users will pay. They assume the market is ready. They assume nothing changes." Read the run and ask one question. Is the repetition doing work, or is it filling space? This is a judgment call rather than a prohibition, and the reason is that the form is legitimate and has a name. Thoreau wrote "It does not keep the country free. It does not settle the West. It does not educate.", and Melville "Forty years of continual whaling! Forty years of privation, and peril, and storm-time!" Those build: each limb goes somewhere the last one did not. The tell is the same construction without the escalation, where every limb restates the first and cutting the repetition would cost the passage nothing. The two cases are impossible to tell apart by shape alone, which is why no checker can decide this one for you. Keep at most one deliberate anaphoric run in a piece, count it across the whole assembled text rather than section by section, and make sure it is the strongest passage you have. If it is not, cut it and let the sentences stand on their own openings.

The same tidiness shows up as constant self-reference: "As mentioned above." "As we discussed earlier." "As noted previously." "As we have seen." "As we established earlier." Cut them, or restate the point in three words. A long reference document sometimes needs a genuine back-pointer; a piece of prose almost never needs one every other paragraph. Watch the shape rather than the words: the tell is a cross-reference standing on its own before a comma, so "as we have seen the results, we can decide" is an ordinary subordinate clause and is fine.

The closing move is the same habit pointed forward: "In conclusion." "To sum up." "In summary." "All in all." The reader can see the piece ending. Cut the signpost and state the last point; if the closing paragraph needs an announcement to read as closing, it is not closing anything. This one is genuinely conventional in academic and formal report writing, so it is a judgment call there rather than a prohibition.

### Use direct address where appropriate

"You'll want to adjust your settings first" is more human than "Users should configure their settings." Second-person pronouns signal a writer aware of their reader. Use in tutorials, blog posts, and professional prose.

### Keep the source's confidence

Human writers are declarative on strong claims ("This is wrong.") and uncertain on uncertain ones ("This probably works, but I haven't tested it at scale."). AI presents everything with uniform confidence. Keep each claim as firm or as hedged as the source made it, and don't shift confidence for variety.

## 5. Texture, with restraint

Every rule in this section means keeping what the source has or cutting what a model added. None of them asks you to add a trait so the text looks human.

### Keep the source's own traces

Self-corrections ("or rather," "to be more precise"), parenthetical qualifications and uneven contractions belong to the source where it has them, so keep them. Don't stage one; a planted self-correction reads as performance.

### Give actions a real agent

Watch for abstract nouns doing the work of people. "The order mattered as much as the rule." "The gap taught us something." The sentence sounds fluent, but nothing and no one is actually acting. Rewrite so a person or a concrete thing holds the verb: "I had to get the order right, not just the rule." Do this only where a real agent exists in your material; don't invent one to satisfy the rule.

Metaphorical "carry" is the most frequent version of this and the hardest to hear, because it sounds like craft. "The layout carries the weight of the argument." "The silence carried the room." "Eight words to carry." The verb performs gravity while the sentence names no actor and no effect. Say what the thing actually does: "the layout is what makes the argument land," or, for the label form, "eight words, and they have to do the whole job." Literal carrying is fine, and so is a truck carrying a load; the tell is an abstraction carrying an abstraction. The subject does not have to be as abstract as "the layout" for this to read as machine-made. A process or a project in the subject slot does it too: "the rebuild carries the argument," "the rollout carries the message," "the migration carries the lessons from the last one." Name who made the argument, or say where it actually sits. One carve-out worth knowing: "carries risk," "carries a cost," "carries weight with the board" and "carries consequences" are ordinary business and legal English, not tells, and rewriting them makes the prose stranger rather than more human.

Time and calendar nouns do it too, and they are easy to miss because they read as a lively figure. "Co-op hours were 9 to 5, so the Fridays survived." "Busy season eats the Fridays." "Billiards survives final year." "Work does not get to claim them." The schedule becomes a creature, and the person who decided anything drops out. Name the person and say what happens: "I still make it to billiards on Fridays," "No billiards from January to April." The same drafts tend to repeat "I get my Fridays back" and "I have my evenings back." Once is fine; twice in one piece is a refrain. Literal uses stay: "the winter killed the roses."

Ideas and artifacts do it too, usually inside a maxim about the work: "A prototype is a question put to the people who will use the thing, and the answer usually costs you the design you arrived with." "Photography is the only thing I do that asks me to stand still." The answer does not cost anyone anything, and photography asks nothing. Say what the people did: "Testing usually sent me back to redesign."

### Use domain-specific vocabulary

Replace generic formal words with vocabulary that reflects the author's actual expertise. A software engineer writes "race condition" not "concurrent access issue." Keep a term of art intact even when it contains a word from the flagged list: "differentiated instruction" is a teaching term, and every plainer substitute changes what it means. Keep an idiom the source already uses; don't add one to sound human. Keep the specific names, places and references the source gives, so "the 737 MAX groundings" does not become "a recent aviation incident." When you draft, a specific the piece needs and nobody supplied becomes a marked placeholder (see "Facts come from the user or the source").

### Use the plain defaults

Readers recognise a model's formatting and attribution habits as quickly as its vocabulary. In reporting, write "says" every time rather than rotating through "notes," "explains" and "emphasizes." Don't open every bullet with a bold label and a colon, and don't put emoji at the start of headings or list items, unless the house style asks for it. In an essay, a blog post, an opinion piece or a cover letter, a person usually speaks plainly to a reader somewhere, through a first-person position, a "you," or a question. Where the draft has none, add one only where the user or the source supplies the position, and never invent a first-person view or experience.

### Develop ideas unevenly

Give more space to the ideas that matter most. AI gives equal airtime to every point, so don't develop every point to the same depth. Some points get detailed evidence from the source, and others are stated and left. Keep asides the source has instead of adding new ones, and leave some transitions implicit.

### Leave friction in the argument

AI argument is suspiciously tidy, with every example fitting, every thread resolved and nothing left open. Keep the friction the source has: a caveat that complicates its thesis, an example that only mostly fits, a question it raises and leaves open. Don't sand that roughness off, and don't add friction the source lacks.

## 6. Anti-patterns to eliminate

If you see any of these, rewrite them:

1. **Significance puffery:** "marking a pivotal moment," "setting the stage for," "a broader movement." Strip editorializing. State what happened.
2. **Vague authorities:** an appeal to an unnamed source, whether a group ("researchers and conservationists," "efforts are ongoing," "a larger initiative") or an epistemic frame that borrows credibility it never earns ("studies show," "research suggests," "experts agree," "it is widely believed," "many argue"). Name the specific study, person, or body and cite it. If you can't name them, drop the claim or state it as your own view. A named, specific reference ("a 2024 Stanford study of 16,000 workers found...") is fine. So is a news headline's trailing attribution ("Not a recession, but close, economists say"), because the story names them; the same frame with a full stop in body prose is the appeal to cut.
3. **Vocabulary clustering:** when "valuable insights," "highlight," "underscore," "showcasing," "intricate," and "interplay" appear together. Replace with the specific facts.
4. **Antithesis and negative parallelism:** "not just X, but also Y" → simple conjunction. "It's not X, it's Y," including the two-sentence version ("...is not Y. It is Z.", contracted or not, counted across the whole piece), the fragment ("Not because X, but because Y."), and the inline pair used as a reflex rather than as a scope note ("The work is judgement, not process."), → state the point directly. See "Kill the antithesis reflex" above for the full family.
5. **Elegant variation:** rotating synonyms for the same concept to avoid repetition. Repeat the plain noun, and use the same word for the same thing.
6. **Despite-challenges formula:** "Despite its success, X faces challenges, including... Despite these challenges, X remains..." Replace with specific problems and specific responses.
7. **Didactic disclaimers:** "it's important to note," "it's worth noting," "it's crucial to remember." Cut the preamble, state the fact. The same family includes the corrective disclaimer that guards against a reading nobody proposed ("Claims about its floating should be treated as religious tradition rather than as archaeological explanation") and the source-gap hedge ("is not widely documented," "based on the available information"). State what is known and stop; name a missing source only when its absence matters.
8. **Travel-brochure puffery:** "nestled," "vibrant," "bustling," "rich cultural heritage," "breathtaking," "hidden gem," "fascinating glimpse." State geography and move on.
9. **Nominalization chains:** "The implementation of the optimization of resource allocation" → "We optimized how resources were allocated."
10. **Enumeration stacking:** Three consecutive three-item parallel lists. Vary list length and embed items in prose.
11. **Chatbot residue:** anything addressed to the person who asked for the text rather than to its reader: "Certainly! Here is a summary...", "Here's a polished version," "As an AI language model, I...", "as of my last knowledge cutoff," "Would you like me to expand on any section?" Delete it. Ordinary courtesy in a real email or chat ("I hope this helps," "Sure! Here's the Zoom link," "Here's the updated draft of the lease") is fine.

## Before you return the text

Reading these rules is not enough on its own; a quick verification pass catches what a single edit leaves behind. Before you hand back the result, re-read it once and check the following.

**Eliminate these completely.** They are prohibitions, not stylistic preferences, so none should survive anywhere in the text.

- Em-dashes.
- Invented specifics. A rewrite adds no fact and keeps every hedge and firm claim as the source had it. A draft read as fact uses only the specifics the user or the source supplied, with a marked placeholder such as [number] where one is missing.
- Didactic disclaimers ("it's important to note," "it's worth noting") and empty openers ("in today's fast-paced world").
- The antithesis flip and the pronouncement frames from the structure section. Count the "It's not X. It's Y." flip across the whole piece, contracted or not; more than one is the reflex.
- Meta labels that name the text's own format or length instead of its subject, and self-satisfied closers or first-person meta-commentary that perform polish instead of adding content. Keep at most one aphorism or paradox construction, and only where it does real work.
- Appended significance labels: a heading or subtitle that names its subject and then annexes a clause promising the subject matters ("Method, and why this one," "..., and the officer the whole system turns on"). Check every label, not just the body, and count them across the assembled piece rather than one section at a time.
- The antithesis fragment: a sentence opening on *Not* and pivoting on *but* with the same word starting both halves ("Not because X, but because Y").
- The unsolicited-reassurance frame ("You're not alone," "It's not just you") and the question-fragment beat ("The best part? ..."), unless the piece earns one.
- The frame-opener tics ("When it comes to X," "In a world where," "That's where X comes in," "plays a pivotal role in"), the manufactured-empathy opener ("If you've ever struggled with..."), and the withheld-insight teaser ("Here's the kicker," "the part most people miss").
- Metaphorical "carry" with an abstract subject ("carries the weight," "carries the burden," "words to carry") or a process in the subject slot ("the rebuild carries the argument"), and the "quiet X" / "quietly reshaping" collocation. "Carries risk" and "carries a cost" are ordinary English and stay.
- Time nouns as agents ("the Fridays survived," "Busy season eats the Fridays"), the clipped verdict ("Tutoring stays."), the stance closer ("and I want to keep it there"), and a repeated "get my evenings back."
- The false-candour opener ("Honestly?" "Frankly?"), the instruction to feel something ("Let that sink in"), and the balancing hedge ("While X has benefits, it also carries risks").
- Copula dodges: "serves as," "stands as," "represents a shift," "marks a milestone" where "is" would do. Keep the substitute only where it says something "is" cannot ("she serves as chair," "the board comprises seven members").
- The signposted conclusion ("In conclusion," "To sum up," "All in all") and the self-reference that points backward ("As we have seen"). Both spend a sentence on navigation.
- The staccato negation run ("Not a bug. Not a feature."), the instructed analogy ("Think of it as a..."), and the announced procedure ("Let's break this down," "Let's unpack").
- The appended candour disclaimer: a first-person admission tacked onto a finished statement ("..., and I'm not going to pretend that was the plan"). Starting a sentence that way is ordinary hedging; appending it is the tell.
- Tidy self-reference ("as mentioned above," "as we discussed earlier") outside a genuine reference document.
- An upbeat forecast in the last paragraph ("As the field continues to evolve," "Looking ahead," "One thing is clear:"), an importance flag ("This distinction matters because," "Why this matters"), the balanced maxim ("X is as much about A as B"), and a repeated graded contrast ("less about X and more about Y").
- The cause-to-benefit "so" tail (", so a fix reached people within a day"), the numeric caption ("One count, four moments"), and lines that narrate your own backstory or praise your own habits ("came first, and so did the habit of," "keep the files tidy"). A sentence-initial "So," is fine.
- In product or case-study copy: a mechanism explained in a chain of clauses, the product's internal words, or a slogan with a clever second half no one can picture. Read it as a stranger would.
- Chatbot residue ("Certainly! Here is...") and corrective disclaimers ("should be treated as X rather than as Y," "not widely documented").
- In fiction: an emotion inventory ("a mix of pride and sadness"), the stock phrases ("voice barely above a whisper"), a default character name, and a sentence that explains what the previous one showed.
- Vague-authority appeals ("studies show," "experts agree," "it is widely believed") left without a named source.
- Any AI-flagged word left in that a plainer one would replace without loss.
- Reality-insistence words (*real*, *actual*, *genuine*, *truly*) beyond a single deliberate use.

**Confirm these follow the content.** None of them is a quota.

- Sentence and paragraph length follow what each one says, with no fragment or one-line question added for rhythm.
- No shape repeats from section to section: the same closer, the same contrast, the same transition.
- Nothing was added to look human. No fragment, aside, idiom, self-correction or informal word appears that the source lacks.
- Sentence openings are not stacked: no run of three or more consecutive sentences starting on the same word, unless it is the one deliberate anaphoric passage in the piece and it earns itself.

If a check fails, rewrite only the spot that fails it and leave the rest of the text as it is. Then run the checks once more, and stop after two rounds. The pass checks adherence to the rules above and adds no second, heavier layer of editing.

---

## Important caveats

- **Do not apply these rules uniformly.** If every paragraph gets the same kind of edit, the uniformity of the interventions is detectable. Some paragraphs should change heavily, others barely at all.
- **Preserve the original meaning and intent.** These rules change how the text reads and leave what it says alone (see "Facts come from the user or the source").
- **The word list ages faster than the structure rules.** The flagged vocabulary reflects models through 2025; newer models pick different favorites. Structural, discourse, and section-to-section rules are more durable, so trust them over word swaps when editing output from a current model.
- **Content type matters.** Academic writing should be less casual than blog posts. Technical writing can tolerate more nominalizations than marketing copy. Adjust aggressiveness by genre. A résumé or CV is fragments and lists by design, so the fragment advice under "Let sentence length follow the content" and "Fix enumeration overuse" do not apply there; a Skills block is a list and carries no rule-of-three tic. What still applies is voice: no adjectives about your own habits ("keep the files tidy"), no "came first, and so did the habit of," just a role label and dated facts.
- **Some "AI patterns" are legitimate in context.** Formulaic transitions are standard in academic writing. Neutral tone is appropriate in journalism. Don't overcorrect genre conventions.
- **ESL writers may share patterns with AI.** Lower lexical diversity, formulaic transitions, and simpler sentence structures can reflect a learner's voice. Don't erase it.

=====

[PASTE YOUR TEXT HERE]
