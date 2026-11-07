# Stars vs Sales: Do Product Reviews Actually Drive Success?

A data science project analyzing whether Amazon star ratings and written reviews actually line up with how well products sell.

**Team: Data Detectives** — Sonal Chakraborty, Vishana Baskaran, Hari Balaji

## Research questions

1. **Do higher-rated products actually have higher sales or popularity?**
   Popularity rises sharply once ratings pass about 4 stars and peaks around 4.8. It drops off near a perfect 5.0, which is rare.
2. **Is the number of reviews more important than the average rating?**
   Both are positively related to recent purchases, but review count is the much stronger predictor. This holds across correlation, standardized regression and visualizations.
3. **Are extreme reviews (1-star or 5-star) more influential than moderate reviews?**
   Highly rated products (4.5–5) clearly lead in both sales and engagement. Low-rated products get very little attention.
4. **Does the language of a review reflect its star rating?**
   Sentiment and rating are positively correlated, but only weakly. Positive words show up often in negative reviews too.

## Repository contents

| File | Description |
|---|---|
| `stars_vs_sales_analysis.ipynb` | Full analysis notebook (code, charts, write-up) |
| `stars_vs_sales_analysis.html` | Rendered HTML version of the notebook, viewable without Jupyter |
| `data/reviews.csv` | Amazon review-text dataset used for Question 4 |
| `requirements.txt` | Python packages needed to run the notebook |

## Data

- [Amazon Products Sales Dataset (42K items, 2025)](https://www.kaggle.com/datasets/ikramshah512/amazon-products-sales-dataset-42k-items-2025) — ratings, review counts, purchases last month (Questions 1–3)
- [Amazon Sales Dataset](https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset) — review text (Question 4)

The notebook downloads both datasets automatically with `kagglehub`. The main products dataset (~37 MB) isn't stored in this repo because of its size.

## How to run

```bash
pip install -r requirements.txt
jupyter notebook stars_vs_sales_analysis.ipynb
```

## Tools

Python, pandas, NumPy, Matplotlib, scikit-learn, NLTK
