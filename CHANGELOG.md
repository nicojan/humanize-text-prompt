# Changelog

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
