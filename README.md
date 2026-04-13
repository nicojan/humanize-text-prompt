# humanize-text-prompt

A prompt you paste into any LLM to make AI-generated text sound like a person wrote it. Every rule traces back to peer-reviewed research.

## What this is

`PROMPT.md` is a standalone document. You copy it into a conversation with Claude, ChatGPT, Gemini, Llama, or whatever you use. Paste your text at the bottom, hit send. The model edits your writing based on evidence about how AI text differs from human text at the word, sentence, tone, and cognitive levels.

## What this is not

This is not a detector. It does not classify text as human or AI.

It is an editing guide. The goal is writing that reads better: more varied, more specific, less formulaic. If your institution or jurisdiction requires you to disclose AI involvement, use this tool alongside that disclosure.

## Quick start

1. Open any LLM chat interface.
2. Copy the full contents of [`PROMPT.md`](PROMPT.md).
3. Paste it into the chat.
4. Replace `[PASTE YOUR TEXT HERE]` at the bottom with your text.
5. Send.

You get back an edited version with AI-correlated patterns reduced.

## What the rules cover

| Layer | What it addresses | Examples |
|---|---|---|
| **Vocabulary** | AI-overused words, nominalization, abstract nouns, adverb gaps, uniform hedging | "delve" becomes "explore"; "the implementation of" becomes "we implemented" |
| **Structure** | Sentence length sameness, syntactic rigidity, too many lists, dependency distance, punctuation variety | Lengths from fragments to 25+ words; no three-item list stacking |
| **Tone** | Flattened sentiment, readability mismatch, narrow emotional range | Allow frustration and skepticism; match grade level to the audience |
| **Discourse** | Formulaic transitions, over-explicit cohesion, coordination vs. subordination | Drop "Furthermore"; use "because" instead of "and" |
| **Texture** | Cognitive load artifacts, self-monitoring traces, domain vocabulary | Self-corrections, uneven idea development, idiomatic language |

## Sources

The rules draw on the following peer-reviewed papers, reference documents, and community resources. Citations follow APA 7th edition format.

### Peer-reviewed research

Ardeshirifar, S. (2025). Comparing handcrafted and deep learning approaches for detecting AI-generated text: Performance, generalization, and linguistic insights. *AI and Ethics*, *5*, 4197–4209. https://doi.org/10.1007/s43681-025-00700-2

Muñoz-Ortiz, A., Gómez-Rodríguez, C., & Vilares, D. (2024). Contrasting linguistic patterns in human and LLM-generated news text. *Artificial Intelligence Review*, *57*(10), 265. https://doi.org/10.1007/s10462-024-10903-2

O'Sullivan, J. (2025). Stylometric comparisons of human versus AI-generated creative writing. *Humanities and Social Sciences Communications*, *12*, 1708. https://doi.org/10.1057/s41599-025-05986-3

Opara, C. (2025). Distinguishing AI-generated and human-written text through psycholinguistic analysis. *arXiv preprint*, arXiv:2505.01800. https://doi.org/10.48550/arXiv.2505.01800

Przystalski, K., Argasiński, J. K., Grabska-Gradzińska, I., & Ochab, J. K. (2024). Stylometry recognizes human and LLM-generated texts in short samples. *Expert Systems with Applications*, *296*, 129001. https://doi.org/10.1016/j.eswa.2025.129001

Rujeedawa, T., et al. (2025). Unmasking AI-generated texts using linguistic and stylistic features. [Preprint].

Terčon, L., & Dobrovoljc, K. (2025). Linguistic characteristics of AI-generated text: A survey. [Preprint].

Tulchinskii, E., Kuznetsov, K., Kushnareva, L., Cherniavskii, D., Barannikov, S., Piontkovskaya, I., Nikolenko, S., & Burnaev, E. (2023). Intrinsic dimension estimation for robust detection of AI-generated texts. *arXiv preprint*, arXiv:2306.04723. https://doi.org/10.48550/arXiv.2306.04723

### Reference documents

Grammarly. (2025). Common words and phrases in AI-generated text. https://www.grammarly.com/blog/ai-writing/common-ai-words/

### Community resources

Wikipedia contributors. (2025). Wikipedia:Signs of AI writing. In *Wikipedia, The Free Encyclopedia*. Retrieved April 13, 2026, from https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing

### Underlying theory

The psycholinguistic layer builds on Cognitive Load Theory (Sweller, 1988), metacognition and self-monitoring (Flavell, 1979), lexical access models (Levelt, 1989), and discourse planning (Grabe & Kaplan, 1996). Opara (2025) maps stylometric features to these cognitive processes; that mapping shaped how the texture rules work.

## How the rules were built

Nine papers from 2023 to 2025 provided the quantitative foundation. They cover lexical diversity, part-of-speech distribution, syntactic complexity, dependency structure, sentiment, n-gram patterns, and stylometric clustering.

Findings were sorted into six layers: vocabulary, structure, tone, discourse, texture, and anti-patterns. Patterns confirmed by more than one independent research group got priority.

For each confirmed pattern, we wrote an actionable rewriting rule. Each rule says what to look for, how to change it, and, critically, how to apply the change unevenly. Uniform "humanizing" is itself an AI signal.

The anti-pattern examples show concrete before-and-after transformations rather than abstract advice. The caveats section spells out where the rules break down: ESL contexts, genre differences, model evolution, and the paradox of consistent inconsistency.

## Key research findings

**Lexical diversity.** AI text has lower Type-Token Ratios, fewer hapax legomena, and fewer unique words than human text (Ardeshirifar, 2025; Muñoz-Ortiz et al., 2024). That is the basis for the vocabulary diversity rules.

**Part-of-speech distribution.** AI overuses auxiliary verbs, determiners, coordinating conjunctions, symbols, and numbers. Humans use more nouns, adjectives, proper nouns, adverbs, and punctuation (Muñoz-Ortiz et al., 2024; Ardeshirifar, 2025).

**Sentence length variance.** Human writers show wider sentence-length distributions with higher standard deviation. AI clusters around shorter, uniform lengths (Ardeshirifar, 2025; Terčon & Dobrovoljc, 2025). This is why the burstiness rules exist.

**Dependency length.** Humans naturally keep syntactically linked words close together; LLMs do this less well (Muñoz-Ortiz et al., 2024).

**Sentiment neutrality.** AI skews neutral-to-positive and suppresses negative emotions: anger, fear, disgust (Muñoz-Ortiz et al., 2024). The tone rules push back against that flattening.

**Stylometric clustering.** In creative writing, LLM outputs form tight, uniform clusters while human texts scatter broadly, as measured by Burrows' Delta (O'Sullivan, 2025). This is the strongest argument for stylistic individuality over rule-following.

**Discourse markers.** AI uses fewer but more repetitive discourse markers and fewer modal or epistemic markers (Terčon & Dobrovoljc, 2025).

**Nominalization.** AI text shows higher nominalization rates (Terčon & Dobrovoljc, 2025). The verb-led construction rules address this directly.

**Readability.** AI produces text at a higher grade level than human text for the same content type (Terčon & Dobrovoljc, 2025; Opara, 2025). The readability calibration rules bring this back in line.

## Limitations

The flagged vocabulary reflects models through 2025: GPT-3.5, GPT-4, LLaMA, Falcon, Mistral. Newer models will adopt different word preferences. Structural and psycholinguistic rules should hold up longer than lexical ones.

Detection features break down under domain shift. Rules tuned for blog posts may misfire on academic prose. Ardeshirifar (2025) found a 34.67 percentage point F1 drop in cross-dataset testing.

Newer, larger models are converging on human-like word distributions while staying detectable through structural uniformity (O'Sullivan, 2025; Przystalski et al., 2024). Weight structural and psycholinguistic rules higher than word substitution when editing frontier model output.

Some patterns flagged here as AI-correlated are normal in certain human contexts, particularly academic and journalistic writing. Formulaic transitions, neutral tone, and standardized grammar are conventions in those genres, not AI tells.

These rules describe statistical tendencies. Text that follows every rule can still be flagged. The goal is to shift the probability distribution, not to guarantee any particular outcome.

## Contributing

Found a new paper on AI text detection patterns? Open an issue with the citation and a summary. Spotted a pattern the rules miss? Submit a pull request with the proposed rule and its research basis.

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for details.

## Licence

Released under the [MIT Licence](LICENSE). The underlying research belongs to its respective authors and is cited above.
