# Data-Practicum-Summer-2025


# Sentiment and Language Analysis of Song Lyrics to Predict Billboard Chart Success

## Overview

This project uses **sentiment analysis**, **topic modeling**, and **readability scores** to analyze song lyrics and predict their **Billboard Hot 100 peak chart positions**. Lyrics are pulled using the Genius API, and features like **sentiment**, **topic**, and **Flesch-Kincaid readability scores** are extracted and used to train regression models.

The goal is to explore whether lyrical emotion and language alone can predict a song’s chart success.

---

## Project Structure

```

Sentiment and Language Analysis.ipynb    # Main Jupyter notebook with full analysis
README.md              # Project documentation

```

---

## Features Extracted

- **Sentiment Score**: Using NLTK’s VADER sentiment analyzer.
- **Flesch-Kincaid Readability**: To assess lyrical complexity.
- **TF-IDF + NMF Topics**: Unsupervised topic modeling to group lyrical themes.
- **Language Detection**: To filter out non-English tracks.

---

## Tools & Libraries

- `pandas`, `numpy` — data manipulation
- `matplotlib`, `seaborn` — visualization
- `nltk` — sentiment analysis
- `textstat` — readability scoring
- `scikit-learn` — regression modeling
- `lyricsgenius` — Genius API integration
- `langdetect` — language filtering
- `BeautifulSoup`, `requests` — for web scraping when needed

---

## Key Findings

- Sentiment alone was **not a strong predictor** of chart position.
- Some topics (e.g., love vs. aggression) showed weak correlation to rank.
- Readability scores varied widely; most lyrics are simple, but high-complexity outliers exist.
- Combining sentiment, topics, readability improves regression accuracy.

---

## Potential Improvements

- Include more features like tempo and Spotify popularity score, etc.
- Expand dataset to include full Billboard Hot 100 dataset .
- Explore classification instead of regression (e.g., Top 10 vs. Not).

---

## Author

**RJ Clemens**  
Master's in Data Science and Strategic Analytics — Stockton University  


---

## License

This project is for educational purposes. Data sourced via the Genius API and Kaggle using Billboard Hot 100.

Link to Dataset: https://www.kaggle.com/datasets/dhruvildave/billboard-the-hot-100-songs
