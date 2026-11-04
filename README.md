<div align="center">

<img src="assets/cleantxt-banner.png" alt="CleanText — Strip the noise. Keep the signal." width="100%">

# CleanText

**Strip the noise. Keep the signal.**

A browser-based text-processing playground for exploring tokenization, stop-word filtering, protected negations, lightweight stemming, part-of-speech heuristics, and document-term matrices.

[Open the app](index.html) · [Features](docs/FEATURES.md) · [Privacy](docs/PRIVACY.md)

</div>

## What it does

- Splits text into sentences, lines, or blank-line-separated segments.
- Tokenizes words and numbers while normalizing curly apostrophes.
- Optionally filters a built-in English stop-word list.
- Protects negations such as `not`, `never`, and `nothing` from filtering.
- Offers a lightweight suffix-based stemming option.
- Shows approximate part-of-speech (POS) tags using small word lists and rules.
- Builds document-term matrices using raw counts, binary values, or TF-IDF.
- Displays the vocabulary, removed terms, filtered segments, and token details.
- Lets you copy the cleaned output.

## Run locally

No build step or package installation is required.

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Paste or type text, choose your options, and select **Run pipeline**.

You can also use **Ctrl+Enter** (or **Cmd+Enter** on Mac) to run the pipeline.

## How it works

CleanText is a client-side educational tool. It tokenizes text, optionally removes stop words while preserving listed negations, optionally applies simple suffix rules, then calculates term counts and document frequencies for the selected matrix view. TF-IDF values are calculated from the segmented documents and normalized per document.

## Important limitations

- POS labels are approximate rule-based guesses, not output from a trained language model.
- The stemming option uses simple suffix rules; it is not full linguistic lemmatization.
- Stop-word filtering uses a built-in English list and may not suit every context or language.
- TF-IDF and token statistics are educational text-analysis features, not a semantic understanding of the text.
- The tool does not promise perfect cleanup or preserve every formatting detail in its token-based output.

## Privacy

The text-processing code runs in your browser. The current app does not include an account system or a server-side text-processing endpoint. See [docs/PRIVACY.md](docs/PRIVACY.md).

## Contributing

Bug reports and thoughtful improvements are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE).

---

<div align="center">

Made to make text analysis easier to explore. If CleanText is useful, consider giving the repository a ⭐ on GitHub.

</div>
