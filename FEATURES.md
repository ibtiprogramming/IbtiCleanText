# CleanText features

## Text segmentation

Choose sentence, line, or blank-line segmentation. Each resulting segment is treated as a document for the analysis views.

## Tokenization

Text is lowercased, curly apostrophes are normalized, and Unicode letters and numbers are extracted as tokens.

## Stop-word filtering and negation protection

An optional built-in English stop-word list removes common words. A separate protected-negation list prevents selected negation terms from being removed by that filter.

## Light stemming

An optional set of suffix rules shortens some token endings. This is intentionally lightweight and should not be confused with full lemmatization.

## POS tags

The app assigns approximate labels using small lexical sets and suffix rules. These labels are heuristic estimates.

## Document-term matrix

The matrix can show raw term counts, binary presence/absence values, or TF-IDF values. The vocabulary and per-segment values are displayed in the Matrix and Vocabulary views.
