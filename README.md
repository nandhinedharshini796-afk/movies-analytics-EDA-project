# movies-analytics-EDA-project
Exploratory Data Analysis (EDA) on the TMDB 5000 Movies and Credits dataset using Pandas, Matplotlib, and Seaborn in Google Colab, covering data cleaning, aggregations, visualizations, and correlation analysis.   
# TMDB 5000 Movies — Exploratory Data Analysis (EDA)

An Exploratory Data Analysis (EDA) script exported from Google Colab (`untitled30.py`) analyzing the **TMDB 5000 Movies & Credits** dataset (`tmdb_5000_movies.csv` and `tmdb_5000_credits.csv` from `archive (1).zip`).

## Overview
This workflow walks through loading, inspecting, cleaning, summarizing, and visualizing movie attributes such as `budget`, `revenue`, `popularity`, `runtime`, `vote_count`, `original_language`, and `status`.

## What's Included
- **Data Loading & Merging:** Extracts CSV files from `archive (1).zip` and merges `df_movies` and `df_credits` on movie ID (`id` / `movie_id`).
- **Data Cleaning & Inspection:** Audits missing values (counts, percentages, and bar chart), fills missing values (`df_clean` using median for numeric and mode for categorical columns), checks duplicates, and generates summary statistics.
- **Outlier & Distribution Checks:** Computes min/max values, quantiles, and IQR outlier bounds, along with box plots for `budget` and `revenue`.
- **Aggregations & Grouping:** Groups data by `original_language` and `status` to examine movie counts, mean/median `revenue`, `budget`, and `runtime`.
- **Visualizations (Matplotlib & Seaborn):**
  - Histograms & KDE plots (`budget` distribution)
  - Bar charts & count plots (top `original_language` and `status`)
  - Scatter plots (`budget` vs `revenue` overall and colored by `status` or top languages)
  - Line charts (`average budget` by release year and `average revenue` by runtime)
  - Pie charts (`status` share), box plots (`runtime` by `status`, `revenue` by top languages), violin plots (`runtime` by `status`), and a numeric correlation heatmap
- **Targeted EDA Questions:** Explores top languages by movie count, highest average revenue by language, numeric correlations with `revenue`, and sampled budget-vs-revenue relationships.

## Tools & Libraries
- **Python** (Google Colab)
- **Pandas** & **NumPy**
- **Matplotlib** & **Seaborn**

## Dataset
- `tmdb_5000_movies.csv` and `tmdb_5000_credits.csv` (packaged inside `archive (1).zip`)
