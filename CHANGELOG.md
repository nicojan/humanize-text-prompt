# Changelog

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
