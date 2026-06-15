![Get it on Google Play](https://upload.wikimedia.org/wikipedia/commons/thumb/7/78/Google_Play_Store_badge_EN.svg/1280px-Google_Play_Store_badge_EN.svg.png)

# Google Play Store App Market Analysis
### Uncovering trends in app success for a new market entrant

End-to-end CRISP-DM project analyzing 10,800+ apps from the Google Play Store to advise a startup on its Android market entry strategy — covering data cleaning in PySpark, exploratory analysis and visualization in Python, and a published interactive Tableau dashboard.

## Business Questions
- Which app categories have the highest average installs?
- How does pricing (Free vs. Paid) affect ratings and installs?
- What's the relationship between number of reviews and installs?
- Which categories are most competitive (highest volume of apps)?
- What content ratings dominate the most successful apps?
- Is there a relationship between app size and user rating?

## Dataset
Kaggle's Google Play Store Apps dataset — 10,841 records across 13 columns covering category, rating, installs, price, size, content rating, and more.

## Tools
- **PySpark** — data loading, EDA, and cleaning
- **Pandas** — bridge to Matplotlib/Seaborn for visualization
- **Matplotlib / Seaborn** — in-notebook charts
- **Tableau Public** — interactive dashboard

## Process (CRISP-DM)
Data acquisition → business understanding → exploratory data analysis → cleaning (regex parsing of Installs/Price, size standardization to MB, corrupt/duplicate row removal, validation checks) → analysis with visualizations for each business question → multi-page Tableau dashboard.

## Key Findings
- Free apps massively outperform paid apps in installs — a free-to-download launch strategy is strongly supported by the data.
- FAMILY and GAME are the most saturated categories; Communication and Social have the highest installs but are dominated by a handful of mega-apps — mid-tier categories like Photography or Productivity may offer a more realistic entry point.
- "Teen" and "Everyone 10+" content ratings achieve higher average installs with less competition than the saturated "Everyone" segment.
- App size has little effect on ratings — a lightweight, well-built app isn't at a disadvantage.

## Dashboard
[Live interactive dashboard on Tableau Public](https://public.tableau.com/app/profile/miriam.kilonzo/viz/GooglePlayStoreMarketAnalysis_17807497458760/Page1MarketOverview?publish=yes) — three pages covering market overview, pricing & engagement, and app characteristics, with parameter controls, filters, and cross-chart highlighting.

## Repo Contents
- `play_store_analysis.ipynb` — full analysis: cleaning, EDA, visualizations, and writeup
- `google_play_store_dataset.csv` — raw data
- `google_play_store_dataset_cleaned.csv` — cleaned data used for the Tableau dashboard
