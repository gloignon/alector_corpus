# Alector Corpus v2 (scraped 2026-03-16)

Note: I do not own this corpus. I did not make the original scraper. 

## Source

Scraped from [corpusalector.huma-num.fr](https://corpusalector.huma-num.fr/) using `scrapers/scrape_alector.py` (Playwright).

Original corpus: Gala, N., Tack, A., Javourey-Drevet, L., Francois, T., & Ziegler, J.C. (2020).
*Alector: A Parallel Corpus of Simplified French Texts with Alignments of Misreadings by Poor and Dyslexic Readers.*
LREC 2020.

## Contents

- `corpus/` — 79 text pairs (158 files)
  - `{000..078}_source.txt` — original (more complex) version
  - `{000..078}_target.txt` — simplified version
- `alector_metadata.csv` — title, author, genre, character counts

## Genre distribution

| Genre                    | Count |
|--------------------------|------:|
| explicatif\|documentaire |    39 |
| narratif\|conte          |    36 |
| narratif\|roman          |     3 |
| narratif\|fable          |     1 |

## Format

Each text file contains one sentence per line (proper line breaks, UTF-8).
This is an improvement over the original GitHub mirror which had entire texts on a single line.

## Update to the scraper

I re-did the scraper to use Playwright instead of selenium, the the original scraper is in this other repo: https://github.com/thiborose/alector_corpus
