# humanize-text-prompt

A research-backed prompt for editing AI-generated text to read more naturally. Paste it into any LLM to rewrite text that sounds like a real person wrote it.

## What this is

`PROMPT.md` is a standalone instruction document you copy into a conversation with any large language model (Claude, ChatGPT, Gemini, Llama, etc.). You paste your text at the bottom, and the LLM edits it following evidence-based rules for reducing detectable AI patterns.

The rules are distilled from peer-reviewed research on how AI-generated text differs from human writing at the lexical, structural, tonal, and psycholinguistic levels.

## What this is not

This is not an AI detection tool. It does not classify text as human or AI. It is an editing guide that makes AI-assisted writing more readable, more engaging, and less formulaic. Where institutional or legal requirements mandate disclosure of AI involvement, this tool should be used alongside disclosure, not instead of it.

## Quick start

1. Open any LLM chat interface.
2. Copy the entire contents of [`PROMPT.md`](PROMPT.md).
3. Paste it into the chat.
4. Replace `[PASTE YOUR TEXT HERE]` at the bottom with your text.
5. Send.

The LLM will return an edited version of your text with AI-correlated patterns reduced.

## What the rules cover

| Layer | What it addresses | Examples |
|---|---|---|
| **Vocabulary** | AI-overrepresented words, nominalization, abstract nouns, adverb deficit, hedging uniformity | "delve" → "explore"; "the implementation of" → "we implemented" |
| **Structure** | Sentence length uniformity, syntactic rigidity, enumeration overuse, dependency distance, punctuation diversity | Vary sentence length from fragments to 25+ words; avoid three-item list stacking |
| **Tone** | Sentiment flattening, readability mismatch, emotional range | Allow frustration, skepticism; match grade level to audience |
| **Discourse** | Formulaic transitions, over-explicit cohesion, coordination vs. subordination | Drop "Furthermore"; use "because" instead of "and" |
| **Texture** | Cognitive load artifacts, self-monitoring traces, domain-specific vocabulary | Self-corrections, uneven idea development, idiomatic language |

## Sources

The rules in this prompt are synthesized from the following peer-reviewed papers, reference documents, and community resources. Citations follow APA 7th edition format.

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

### Underlying theoretical frameworks

The psycholinguistic layer of this prompt draws on Cognitive Load Theory (Sweller, 1988), metacognition and self-monitoring theory (Flavell, 1979), lexical access and retrieval models (Levelt, 1989), and discourse planning and cohesion theory (Grabe & Kaplan, 1996). The mapping of stylometric features to these cognitive processes follows the framework proposed by Opara (2025).

## How the rules were derived

1. **Literature review.** Nine papers spanning 2023–2025 were analyzed for quantitative findings on linguistic differences between human and AI text. The papers cover lexical diversity, POS distribution, syntactic complexity, dependency structure, sentiment analysis, n-gram patterns, and stylometric clustering.

2. **Pattern extraction.** Findings were organized into six layers: vocabulary, structure, tone/sentiment, discourse cohesion, psycholinguistic texture, and anti-patterns. Each finding was cross-referenced across multiple papers to prioritize patterns confirmed by independent research groups.

3. **Rule formulation.** For each confirmed pattern, an actionable rewriting rule was written. Rules specify what to look for, how to change it, and how to apply the change unevenly to avoid creating a new detectable pattern.

4. **Anti-pattern examples.** Before/after examples were created for the most common AI writing patterns, showing concrete transformations rather than abstract advice.

5. **Caveat integration.** Research limitations were incorporated as explicit caveats: ESL sensitivity, genre dependence, model evolution, and the paradox that uniform application of human-patterning rules is itself an AI signal.

## Key research findings behind the rules

**Lexical diversity.** AI text has lower Type-Token Ratios, lower hapax legomenon rates, and fewer unique words than human text (Ardeshirifar, 2025; Muñoz-Ortiz et al., 2024). This motivates the vocabulary diversity rules.

**POS distribution.** AI overuses auxiliary verbs, determiners, coordinating conjunctions, symbols, and numbers. Humans use more nouns, adjectives, proper nouns, adverbs, and punctuation (Muñoz-Ortiz et al., 2024; Ardeshirifar, 2025). This motivates the verb construction and adverb rules.

**Sentence length variance.** Human writers show wider sentence-length distributions with higher standard deviation. AI concentrates around shorter, uniform lengths (Ardeshirifar, 2025; Terčon & Dobrovoljc, 2025). This motivates the burstiness rules.

**Dependency length minimization.** Humans naturally minimize the distance between syntactically linked words; LLMs do this less effectively (Muñoz-Ortiz et al., 2024). This motivates the dependency proximity rules.

**Sentiment neutrality.** AI text skews toward neutral/positive sentiment and suppresses negative emotions like anger, fear, and disgust (Muñoz-Ortiz et al., 2024). This motivates the tone rules.

**Stylometric clustering.** In creative writing, LLM outputs form tight uniform clusters while human texts scatter broadly, as measured by Burrows' Delta (O'Sullivan, 2025). This motivates the overall emphasis on stylistic individuality.

**Discourse markers.** AI uses fewer but more repetitive discourse markers and fewer modal/epistemic markers (Terčon & Dobrovoljc, 2025). This motivates the transition and confidence-level rules.

**Nominalization.** AI text shows higher rates of nominalization (Terčon & Dobrovoljc, 2025). This motivates the verb-led construction rules.

**Readability.** AI produces lower readability scores (higher grade level) than human text for equivalent content types (Terčon & Dobrovoljc, 2025; Opara, 2025). This motivates the readability calibration rules.

## Limitations

- The flagged vocabulary reflects AI tendencies observed in models through 2025 (GPT-3.5, GPT-4, LLaMA, Falcon, Mistral). Newer models may adopt different patterns. Structural and psycholinguistic rules are more durable than lexical ones.
- Detection features degrade under domain shift. Rules tuned for blog posts may misfire on academic text. Ardeshirifar (2025) documented a 34.67 percentage point F1 drop in cross-dataset detection.
- Newer, larger models are converging on human-like lexical distributions while retaining detectability through structural uniformity (O'Sullivan, 2025; Przystalski et al., 2024). Structural and psycholinguistic rules should be weighted higher than lexical substitution for frontier model output.
- Some patterns flagged as AI-correlated (formulaic transitions, neutral tone, standardized grammar) are conventional in certain human writing contexts, particularly academic and journalistic prose.
- These rules describe statistical tendencies, not absolute markers. Text that follows every rule may still be flagged by some detectors. The goal is to shift the probability distribution, not guarantee a particular outcome.

## Contributing

Contributions are welcome. If you find a new research paper on AI text detection patterns, open an issue with the citation and a summary of the relevant findings. If you've found a pattern not covered by the current rules, submit a pull request with the proposed rule text and its research basis.

## License

This work is released under the [MIT License](LICENSE). The underlying research is cited above and belongs to its respective authors.
