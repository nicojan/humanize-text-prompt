# Changelog

## 1.12.0 - 2026-09-18

Sync with the humanizer rule set. The server scoped three lexicon words to their collocations and dropped a fourth, so this prompt's vocabulary lists carry the same scope.

### Changed

- **`boast`** is scoped to the feature brag: the tell is "boasts a/an/over X" standing in for "has", while "boast of" and "boast about" are ordinary English and stay. On the server this is now `BS-049` rather than a bare lexicon word, after the word measured 7.4 false positives per 10k on 47,088 sentences of pre-1930 prose.
- **`elevate`** is scoped to "elevate your X" and "elevate the experience". Literal raising stays, and so does "elevated rates". Server side: `BS-050`, after 7.4 per 10k.
- **`landscape`** needed no change here. This prompt already said "when metaphorical", which is exactly the scope the server has now mechanized as `BS-051`. Worth recording, because the prompt was ahead of the checker for once.

### Rejected (documented for the record)

- **`particularly`**, which the server dropped from its adverb lexicon this round (117 occurrences on the long-form corpus, 18 percent of every lexicon finding on human prose, and replacements that are synonyms of it). It was never in this prompt, so there was nothing to remove. The guidance it sat behind, that the model underuses manner and degree adverbs and reaches for generic intensifiers, is already here in prose.
- **Document budgets.** The server now counts four budgeted shapes automatically and reports an overrun. This prompt has no checker, so the change is invisible here, and the per-piece counting instruction it already carries is unchanged.

### Notes

- **The self-contradiction check earned itself a fifth time, in an unusual direction.** This prompt's own text says AI words "appear at statistically elevated rates" and mentions "a uniformly elevated grade level". Under the bare lexicon entry the checker flagged its own source document; under the scoped `BS-050` it does not. The contradiction was in the old rule rather than in the prompt, and the scoping resolved it in the same round.

## 1.11.0 - 2026-09-18

Sync with the humanizer rule set. The server narrowed `BS-011`, its worst-precision rule, from a bare two-token pattern to a copula-anchored one, and the surface form it now targets was missing from this prompt.

### Added

- **The inline pair** ("The work is judgement, not process.") as a sixth surface form under "Kill the antithesis reflex": a copula, a short noun phrase, a comma, then the rejected twin closing the sentence. It was the one member of the antithesis family the section did not list, even though the server has flagged it since June. Also added to item 4 of the tell list, scoped there as "used as a reflex rather than as a scope note".
- The carve-out is the load-bearing half, and it is the same one the server now carries in its rule entry: a sentence whose job is to fix a scope ("The unit is the collocation, not the word.") or to correct a fact ("The response was 406, not 421.") is legitimate and stays. The tell is the reflex, the same binary reached for section after section with an abstract noun on both sides.

### Why the carve-out is stated rather than assumed

On the server this is a measured, accepted false positive. The copula-anchored pattern fires 0 times on 47,088 sentences of pre-1930 prose, and 9 times on 2,692 sentences of modern rule-writing prose, where eight of the nine are scope notes and one is the attested tell itself. Precision 1/9 in that register. Narrowing further was probed and fails, because determiners, sentence position and a prestige-noun lexicon all cut across the two senses instead of between them. Recorded as `caveats.contrastive_scope_notes_are_the_same_shape`.

### Notes

- **The self-contradiction check caught it, for the fourth time.** This prompt uses the inline pair twice in its own prose ("This is the collocation, not the word.", "The tell is the appending, not the phrase.") and once in a section heading ("Build emotion through detail, not labels"). An unconditional ban would have contradicted the document in three places on the day it shipped. The bullet is written with the scope-note carve-out explicit, which makes those three uses consistent with it rather than exceptions to it, and none of them was rewritten.

## 1.10.0 - 2026-09-18

Sync with the humanizer rule set. This round is unusual: on the server side it shipped **no new detector**, because the tell it went after turned out to be unmechanizable. The guidance still belongs here, since this prompt is judgment all the way down and can carry what a checker cannot.

### Added

- **Anaphora and stacked sentence openings**, three or more consecutive sentences opening on the same word or the same two words ("They assume users will pay. They assume the market is ready. They assume nothing changes."). Placed directly after "Reduce over-explicit cohesion", because the "This... This... This..." chain already described there is the commonest machine form of the same habit, and the new paragraph generalizes it. Written as a judgment call rather than a prohibition, and the carve-out is the whole point: the form is a named rhetorical figure, so the paragraph quotes Thoreau ("It does not keep the country free. It does not settle the West. It does not educate.") and Melville to show what earning it looks like. The tell is the same construction without the escalation, where each limb restates the first. Budget of one deliberate run per piece, counted across the assembled text.
- A line in the "Confirm these vary" half of the self-check, not the "Eliminate these completely" half. That placement is deliberate and matches the server, where this is a `self_review` rubric item rather than a `banned_structure`.

### Rejected (documented for the record)

- **A mechanical anaphora rule**, which is what the round set out to build. Probed against 47,088 sentences of pre-1930 public-domain prose, the loosest formulation scored 75.4 false positives per 10k sentences and the best scored 3.2 per 10k, at which point all fifteen firings were read and every one was legitimate deliberate anaphora. Set the Thoreau sentence beside the machine tell and every property a detector can read is identical: three sentences, subject pronoun plus a repeated verb, under eight words each. Raising the threshold to four lost the attested tell entirely while still firing on human prose. A parser would not help here, unlike the appositive label, because the figure and its abuse are the same construction rather than two that merely look alike. Recorded on the server as `caveats.rhetorical_figures_defeat_shape_detection`.

### Notes

- **The self-contradiction check found nothing this time**, which is worth recording given it has caught a real conflict on three previous syncs. "Don't repeat the same content word within three sentences unless for deliberate emphasis" (section 1) already carried the right carve-out, and there is no unconditional "vary your sentence openings" instruction anywhere in the prompt that the new paragraph would have contradicted.

## 1.9.0 - 2026-09-17

Sync with the humanizer rule set: adds copula avoidance (humanizer BS-043) and five more tells from a survey of user-identified sources (Wikipedia's editor-maintained "Signs of AI writing", tropes.fyi, slop-sense) and research-identified ones (arXiv:2605.19936, the Science Advances excess-vocabulary study).

### Added

- **Copula avoidance**, the largest gap this survey found: the model will not write "is", so it reaches for "serves as", "stands as", "represents", "marks". A new subsection placed immediately after "Reduce copula overuse", because the two rules look contradictory until you read them together, and the placement is the point. Carries both carve-outs: a person holding an office genuinely serves as something, and a capacitor functions as a filter.
- **The staccato negation run** ("Not a bug. Not a feature.") as a sixth surface form under "Kill the antithesis reflex", with the guard that ordinary emphasis is adverbial ("Not now. Not ever.") and stays.
- **The announced procedure** ("Let's break this down", "Let's unpack") and **the instructed analogy** ("Think of it as a...") folded into "Cut the frame-opener tics", scoped to procedure rather than stance so that "let's be honest" and "let's explore the options" stay untouched.
- **The signposted conclusion** and the backward self-reference ("As we have seen") folded into "Reduce over-explicit cohesion", with the shape guard that "as we have seen the results, we can decide" is an ordinary subordinate clause.
- "Imagine a world where" added beside the existing "In a world where" opener.
- Lexicon: profound, renowned, nestle, "diverse array", "natural beauty".
- All of it added to the "Before you return" self-check.

### Fixed

- **A self-contradiction in the lexicon.** The entry for "In conclusion" recommended "To sum up" as the replacement, which is the same tell in different words. It now says to stop rather than to swap one signpost for another.

### Rejected (documented for the record)

- The rest of the copula verb family (functions as, operates as, comprises, encompasses, constitutes, resides). A probe found 8 out of 8 uses legitimate: these verbs carry technical, legal and organisational meaning the copula cannot replace.
- Bare "diverse", "align with", "notable", "superior". Ordinary high-frequency words; "diverse array" is scoped to the collocation instead, the same treatment "hidden gem" got in 1.4.0.
- Every formatting and markup signal in the survey: curly quotes, emoji bullets, bold-first bullets, title-case headings, and the model-specific leakage strings. Tooling artifacts rather than author signals. The leakage strings are real evidence of where a text came from, but they are not prose, and this prompt is about prose.
- Bare "quietly", for the third time. The collocation rule from 1.6.0 already covers what is real about it.
- Definite-article omission ("rain in teeth"). A genuine artifact of poetry generation, but a rule for it would fire on every headline and list item.
- "Here's the thing", again. This prompt recommends it elsewhere as a human transition.

## 1.8.0 - 2026-09-17

Sync with the humanizer rule set: adds the appended candour disclaimer (humanizer BS-042), widens metaphorical "carry" to process nouns in the subject slot (BS-040), and puts a document-level budget on the appended significance label. From an in-the-wild report naming three shapes.

### Added

- **The appended candour disclaimer**: a first-person admission tacked onto a statement that was already finished. "The redesign took nine months, and I'm not going to pretend that was the plan." The clause adds no fact and asks for credit for honesty while withholding what an honest sentence would contain. Folded into "Cut the false-candour opener" as the appended sibling of the "Honestly?" fragment, and added to the "Before you return" self-check.

### Changed

- **Metaphorical "carry" now covers process nouns in the subject slot**: "the rebuild carries the argument," "the rollout carries the message," "the migration carries the lessons." The subject does not have to be as abstract as "the layout" for the sentence to read as machine-made. Carries a new carve-out in the same breath: "carries risk," "carries a cost," "carries weight with the board" and "carries consequences" are ordinary business and legal English, and rewriting them makes the prose stranger rather than more human.
- **The appended significance label gets a budget that is counted across the whole assembled piece**, not section by section. Four sections can each pass with one label while the finished document holds four, which is the shape a reader actually notices.

### Rejected (documented for the record)

- Flagging the bare sentence-initial "I'm not going to pretend ...". It is ordinary hedging that qualifies a claim the writer is about to make, and it is common in human first-person writing. Only the appended form is a tell, so the rule is scoped to the appending. This is the same reasoning that rejected "Here's the thing" and "Let's be honest" in 1.5.0.
- The appositive form of the significance label ("X, and the Y that Zs") as a mechanical rule. The humanizer server re-tested three detection strategies this round and all failed: a loose pattern scored 10/10 false positives on ordinary coordination ("The baker bought bread, and the flour that makes it"), a frequency gate is unsound when per-instance precision is zero, and a finite-verb guard traded recall for precision through a boundary no pattern can see. It stays a judgment call, which is why the budget above matters more than a rule would.

## 1.7.0 - 2026-08-08

Sync with the humanizer rule set: adds the appended significance label (humanizer BS-038) and the antithesis fragment (BS-039), both from an in-the-wild report on a document that had passed the previous rule set clean.

### Added

- **The appended significance label**: a heading or subtitle that names its subject and then annexes a second element promising the subject matters. A *why* clause pre-defending a choice ("Method, and why this one"), or a trailing relative clause asserting a hinge ("Reintegration support at the moment of release, and the officer the whole system turns on"). Added as a fourth form under "Cut the performative framing beat", with the instruction to read every label in the piece rather than only the body. One such label may be deliberate; two is the tell.
- **The antithesis fragment**: a sentence opening on *Not* and pivoting on *but*, with the same word starting both halves ("Not because X, but because Y," "Not to save time, but to save arguments," "Not a strategy, but a habit"). Added to "Kill the antithesis reflex" as a fifth surface form. The previous rules covered the copula flip and the two-sentence versions and missed this one, which is the more common written form.
- Both added to the "Before you return" self-check, and the fragment added to anti-pattern 4.

### Changed

- "Kill the antithesis reflex" now carries the carve-out that distinguishes the tell from ordinary grammar: a sentence where *Not* heads a real subject ("Not all of them agreed, but most did") and the mid-sentence correlative ("He did not go to the store, but to the park") are both fine.

### Rejected (documented for the record)

- The bare adverb form of the fragment ("Not always, but often."). Without a shared word opening both halves it cannot be told from ordinary casual speech ("Not bad, but okay."), and a rule that cries wolf gets ignored.
- Two typography signals reported alongside these: the section symbol, which is ordinary in anything citing statute, and middot separators, which are as common in human-authored web copy as in generated copy. Both are tooling conventions rather than author signals, the same reasoning that rejected smart quotes in 1.4.0.

## 1.6.0 - 2026-08-06

Sync with the humanizer rule set: adds the metaphorical-"carry" rule (humanizer BS-031) that prompted this round, plus six tells from a survey of AI-writing signals published since the previous sync (BS-032..037) and an abstract-prestige metaphor lexicon.

### Added

- **Metaphorical "carry"**: folded into "Give actions a real agent" as the most frequent and hardest-to-hear form of abstraction-as-agent. "The layout carries the weight of the argument." "Eight words to carry." The verb performs gravity while the sentence names no actor and no effect. Literal carrying, and a truck carrying a load, stay fine.
- **The "quiet" collocation**: "quiet confidence," "quietly reshaping." A new Vocabulary subsection, scoped to the collocation rather than the word, so "a quiet room" is untouched. This revisits the bare `quiet` candidate rejected in 1.4.0 and upholds that rejection.
- **The false-candour opener**: "Honestly?" / "Frankly?" as a one-word question promising a confession the sentence does not contain. New Structure subsection beside the question-fragment beat.
- **The withheld-insight teaser**: "Here's the kicker," "the part most people miss." Folded into "Cut the frame-opener tics" with an explicit carve-out, since this prompt recommends the bare "Here's the thing" as a human transition.
- **The balancing hedge**: "While X has benefits, it also carries risks." Folded into "Don't flatten strong positions."
- **The instruction to feel something**: "Let that sink in," "Read that again." Folded into "Cut unsolicited reassurance" as the same therapeutic family.
- **Tidy self-reference**: "As mentioned above," "As we discussed earlier." Folded into "Reduce over-explicit cohesion."
- All seven added to the "Before you return" self-check.

### Changed

- High-severity nouns add: mosaic, symphony, labyrinth, cacophony, kaleidoscope, odyssey; plus beacon, bedrock, crucible and "north star" flagged only in metaphorical or jargon use.
- Moderate-severity verbs add: resonate.
- Moderate-severity adjectives add: compelling.

### Rejected (documented for the record)

- A bare "carry" word-flag. It is a high-frequency ordinary verb, and flagging the word rather than the collocation is the low-ceiling surface trap. The upstream checker dropped "load" and "freight" from its object list for the same reason, after a probe fired on "the truck carries the load to the depot."
- Re-flagging "Here's the thing" on its own. The 1.5.0 rejection stands; only the withheld-insight claim attached to it is the tell.
- Four semantic tells from the source survey (metaphors that almost land, arguments that teleport, missing emotional spikes, too clean to be human). These are judgment calls already covered by the existing rhythm, stance and friction sections rather than new rules.

## 1.5.0 — 2026-07-25

Sync with the humanizer rule set: adds the phrase-frame tells (humanizer BS-026..030) and a marketing/promotional lexicon surfaced by a 2026 survey of current phrase-frame tells, cross-checked against existing coverage.

### Added

- **Cut the frame-opener tics**: fixed openers that front a point with empty scaffolding — "When it comes to X," "In a world where / In an era of," "That's where X comes in," and the "plays a pivotal role in" template. Cut the preamble and state the claim.
- **Manufactured-empathy opener**: "If you've ever struggled with..." folded into "Cut unsolicited reassurance." A canned second-person conditional bolted to the front of a piece; an ordinary conditional recalling a real shared experience ("If you've ever been to Paris...") is fine.
- Both new tells added to the "Before you return" self-check.

### Changed

- Moderate-severity verbs add: unlock, unleash, embark, empower, elevate.
- Moderate-severity adjectives add: invaluable, unwavering, ever-evolving.
- High-severity nouns add: treasure trove, plethora, myriad.

### Rejected (documented for the record)

- Register-dependent openers ("Here's the thing," "Let's be honest") — common in genuine human casual prose; the low-ceiling surface trap. (The prompt already recommends "Here's the thing" as a *human* transition, which is why flagging it would be self-defeating.)
- Legitimate high-frequency human discourse markers ("in other words," "that said," "to be clear").

## 1.4.0 — 2026-07-13

Sync with the humanizer rule set: adds three tells surfaced by a web survey of current (2025–2026) AI-writing signs, cross-checked against existing coverage (humanizer BS-023/024/025 + lexical additions).

### Added

- **Cut unsolicited reassurance**: the therapeutic second-person frame ("You're not alone," "You're not imagining it," "It's not just you"), the most-cited *new* 2026 tell, incongruous in most content. Cut it or make the reassurance concrete.
- **Cut the question-fragment beat**: the short noun-phrase-fragment question fired off as a setup and answered in the next breath ("The best part? It's completely free."). State it as a declarative; an ordinary question in the flow is fine.
- **Leave friction in the argument**: excessive coherence and tidiness (every example fits, every thread resolves, nothing left open) is itself a tell. Keep the caveat, the partly-open question, the example that only mostly fits.
- Both new tells added to the "Before you return" self-check.

### Changed

- **Vague authorities** (anti-pattern 2) expanded to include the epistemic-authority frame ("studies show," "research suggests," "experts agree," "it is widely believed," "many argue"), with the fix being a named, cited source; a named/specific reference is explicitly fine.
- **Travel-brochure puffery** (anti-pattern 8) adds "bustling" and "hidden gem."
- Transition drop-list adds "Notably," "Importantly," "Consequently."

### Rejected (documented for the record)

- Curly/smart-quote detection: a tooling artifact, not an author signal (raw human web text is often curly, raw model output often straight; modern model UIs emit curly quotes anyway). It discriminates nothing reliable, so it is deliberately not a rule.
- A bare *quiet* word-flag: an ordinary word whose supposed tell is register/collocation, not the token; the low-ceiling surface-swap trap.

## 1.3.0 — 2026-07-07

Sync with the humanizer rule set: adds the performative framing beat, caught in in-the-wild feedback on prose run through the humanizer.

### Added

- **Cut the performative framing beat**: the self-aware flourish that performs polish rather than carrying content, in three forms: the meta label (a heading or standalone line naming the text's own format or length, "In 200 words" / "In brief," instead of its subject), the self-satisfied closer (a neat aphorism ending a section with no new fact, often crediting the writer), and first-person meta-commentary on the work itself ("my take," "the reading of it is mine") in an evidence-led piece. The clever paradox headline is flagged as the borderline case. The definitional caveat is kept: one aphorism or paradox is legitimate; the tell is repetition and substitution for content, not the device. Added to the "Before you return" self-check.

## 1.2.0 — 2026-07-04

Sync with the humanizer rule set: adds the noun-participle fragment tell, caught in an in-the-wild review of prose that had passed the checker clean.

### Added

- **Cut the noun-participle fragment**: the verbless "Noun, past-participle." sentence ("The same board, rebuilt."), the past-participle sibling of the trailing "-ing" tail. Rewrite it into a full sentence or fold the participle into the neighboring one; a participle inside a full clause is left alone, so legitimate reduced relatives are not touched.

## 1.1.0 — 2026-07-02

Sync with the revised humanizer rule set. The update foregrounds where the signal now lives (flow and section-to-section variation) and adds the frontier-model tells that word-level checks miss.

### Added

- **Core-principle reframe**: local flow and section-to-section variation are the durable signals; lexical substitution is necessary hygiene with a low ceiling, and newer models are already crossing it (Kuznetsov et al., 2025).
- **Kill the antithesis reflex**: the two-sentence copula flip ("...is not Y. It is Z."), the hedged aphorism, the disclaimer reversal, the verb mirror, and the pronouncement frames (wh-cleft, thesis opener, maxim closer), consolidated into two rules.
- **Cut credibility insistence**: density of *real* / *actual* / *genuine* / *truly*, with the reality assertion replaced by the specific that earned it.
- **Vary style from section to section**: the cross-segment signal, treated as its own structural rule.
- **Give actions a real agent**: abstraction-as-agent, where an abstract noun holds an agentive verb.
- **"Before you return the text" self-check**: a verification pass, split into Tier-1 tells to eliminate and Tier-2 variation to confirm. This ports the write→check→fix loop to a no-checker context; its value is for rule adherence, not a separate human-likeness gain.

### Changed

- Expanded the flagged vocabulary to the full current lists: 28 verbs (added underscore, surpass, boast, foster, enhance, optimize, harness, spearhead, catalyze, and others), 18 adjectives, 8 nouns, 16 transitions, 6 qualifiers.
- Sentence-length guidance now targets low variance, not a target mean.
- The em-dash rule notes that em-dash rate is model-specific: the ban stands, but absence is not evidence of human authorship, and presence alone is weak evidence.
- Removed em-dashes from the prompt's own prose so it obeys the rule it teaches.
- README provenance line now reflects both peer-reviewed research and in-the-wild auditing.

### Sources added

- Kobak et al. (2025, *Science Advances*), Krishna et al. (2023, NeurIPS), Kuznetsov et al. (2025, arXiv:2501.19301).

## 1.0.0 — 2026-04-13

### Initial release

Rules distilled from nine peer-reviewed papers (2023–2025) and two community reference documents. Covers six editing layers:

- **Vocabulary**: 26 flagged verbs, 18 flagged adjectives, 8 flagged nouns, 16 flagged transition phrases, 6 flagged qualifiers, 10 common nominalizations, abstract/concrete noun guidance, adverb reintroduction patterns.
- **Structure**: Sentence length variance, syntactic variety (11 rules), punctuation diversity (6 rules), enumeration patterns, dependency proximity, POS distribution targets.
- **Tone/sentiment**: Neutral bias correction, emotional layering, readability calibration, exclamation mark guidance.
- **Discourse**: Transition variation, subordination vs. coordination, cohesive device management, direct address, confidence calibration.
- **Psycholinguistic texture**: Cognitive load artifacts, self-monitoring traces, lexical retrieval signatures, discourse planning traces.
- **Anti-patterns**: 10 named patterns with before/after examples.

Sources: Ardeshirifar (2025), Muñoz-Ortiz et al. (2024), O'Sullivan (2025), Opara (2025), Przystalski et al. (2024), Rujeedawa et al. (2025), Terčon & Dobrovoljc (2025), Tulchinskii et al. (2023), Grammarly (2025), Wikipedia "Signs of AI writing" (2025).
