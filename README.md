# Amazon Bestsellers Analysis (2009–2019)

Exploratory analysis of Amazon's annual bestseller list (550 books, 2009–2019) examining pricing, genre, ratings, and author concentration, using Python and pandas.

## Objective
Understand what characterizes a bestselling book on price, genre, and customer rating, to inform merchandising and promotional decisions.

## Tech Stack
Python · pandas · NumPy · Matplotlib · Seaborn · Jupyter Notebook

## Approach
1. Cleaned and validated the dataset (price, rating, review count, genre fields).
2. Compared fiction vs. non-fiction across volume, price, and customer rating.
3. Analyzed price distribution against customer rating to look for a relationship.
4. Measured author concentration — how many distinct authors account for repeat bestseller appearances.

## Key Findings
- **Non-fiction titles appear more often** on the bestseller list than fiction, but the **highest customer ratings (4.8–4.9) skew toward fiction** titles.
- Customer ratings hold up well across the **$0–$30 price range**, with no clear evidence that higher price correlates with higher satisfaction in this dataset.
- **12 titles** are listed at $0.00 (promotional/free titles) — a small but notable segment.
- A relatively small set of authors accounts for a disproportionate share of repeat bestseller appearances, suggesting brand/author loyalty plays a meaningful role in this market.

## Business Recommendations
- Use non-fiction as the volume driver, but feature top-rated fiction titles in promotional placements.
- Don't assume premium pricing signals quality in this catalog — the data doesn't support that in the $0–$30 range.
- Consider using free/promotional titles as an acquisition tool, and formalize relationships with recurring bestselling authors.

## Limitations
This is 2009–2019 aggregate list data with no unit sales, revenue, or return figures — "bestseller" here reflects rank on Amazon's list, not sales volume, and rating counts can be skewed by a book's time on the list.

## Files
- `Amazon Final.ipynb` — full analysis notebook
- `bestsellers with categories.csv` — source data ([Kaggle: Amazon Top 50 Bestselling Books 2009–2019](https://www.kaggle.com/datasets/sootersaalu/amazon-top-50-bestselling-books-2009-2019))

## How to Run
```bash
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook "Amazon Final.ipynb"
```
