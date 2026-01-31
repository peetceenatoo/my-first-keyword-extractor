## Context

The automatic extraction of relevant expressions and keywords from large text corpora is a fundamental task in Natural Language Processing and Information Retrieval, with applications ranging from document indexing and search engines to topic discovery and text summarization. These problems long predate the recent emergence of Large Language Models (LLMs).

In this project, we explore classical, data-driven approaches for identifying meaningful multi-word expressions and keywords from Big Data corpora, without relying on LLMs. By combining statistical cohesion measures, information retrieval techniques, and correlation-based analysis, we aim to uncover both explicit and implicit concepts that characterize document content, providing a structured and interpretable representation of textual information.

## Tools and models

- Text Preprocessing and Corpus Analysis: Tokenization, normalization, stop-word extraction, and frequency analysis.
- Cohesion Metrics for n-grams: Symmetrical Conditional Probability (SCP), Dice coefficient, and Mutual Information (MI).
- Relevant Expressions Extraction (LocalMax): Identification of statistically cohesive multi-word units based on comparisons with sub-grams and super-grams.
- TF-IDF (Information Retrieval): Ranking of candidate expressions and unigrams to extract the most informative Explicit Keywords per document.
- Correlation-Based Implicit Keyword Extraction: Identification of concepts strongly correlated with Explicit Keywords but not explicitly appearing in the document.
- Evaluation Metrics: Precision, Recall and F1-score.

## Main findings

- Statistical cohesion metrics are effective at identifying meaningful multi-word expressions, with SCP offering the best tradeoff and MI providing the highest precision.
- The LocalMax-based approach successfully extracts Relevant Expressions that align well with named entities and domain-specific phrases.
- Low recall in Relevant Expression extraction does not significantly harm Explicit Keyword extraction, as TF-IDF ranking compensates by prioritizing informative terms.
- Correlation-based methods allow the discovery of Implicit Keywords, capturing latent concepts related to a document’s topic even when they do not explicitly appear.

## Acknowledgements

I thank my colleague and friend [Matteo Saterini](https://github.com/Sateeee00) who worked with me on this project.
