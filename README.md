# Duplicate bug report detection (Eclipse)

When users file the same bug twice, a bug tracker fills with duplicates that waste triage time.
This project predicts whether a pair of Eclipse bug reports describes the same bug, from the raw
HTML pages of the reports.

**Result: 94% accuracy on the validation pairs** (92% on training), with a logistic regression on
four features. The confusion matrix is balanced: 1,888 true negatives and 1,854 true positives.

## Pipeline

1. **Web scraping:** extraction of the summary, description, product and component from each
   report's HTML page (BeautifulSoup).
2. **Text preprocessing:** tokenisation, stop-word removal, stemming (Snowball).
3. **Representation:** bag-of-words vectors, implemented from scratch.
4. **Pair features:** cosine similarity between the two summaries, cosine similarity between the
   two descriptions, same product (0/1), same component (0/1).
5. **Model:** logistic regression trained on the labelled pairs (duplicate = 1, not duplicate = −1),
   evaluated on a separate validation set.

## Run

```bash
pip install numpy scikit-learn nltk beautifulsoup4 matplotlib
jupyter notebook TP_bug_reports.ipynb
```

The bug report archive (HTML pages and the training and validation pairs) came with the course
and is not redistributed. Assignment designed by Irving Muller Rodrigues for a data mining course;
solved as part of my Bachelor's degree in AI at Université Côte d'Azur (November 2024). The
notebook is in French and English.
