# Customer Experience Analytics for Ethiopian Fintech Apps

This project analyzes customer satisfaction with mobile banking apps in Ethiopia by scraping and processing Google Play Store reviews. The analysis focuses on three banks: **Commercial Bank of Ethiopia (CBE)**, **Bank of Abyssinia (BOA)**, and **Dashen Bank**. The goal is to uncover satisfaction drivers, pain points, and provide actionable insights for app improvement.

---

## Task 1: Data Collection and Preprocessing

**Objective:** Collect and clean user reviews for further analysis.

**Steps Taken:**

1. **Web Scraping:**

   * Reviews were scraped from the Google Play Store using Python scripts.
   * Collected fields include: review text, rating, date, bank/app name, and source.
   * Targeted a minimum of 400 reviews per bank

2. **Preprocessing:**

   * Removed duplicate reviews.
   * Handled missing data (reviews without text were removed).
   * Normalized dates to `YYYY-MM-DD` format.
   * Saved the cleaned dataset as `data/clean/cleaned_reviews.csv`.

**Outcome:**
A clean dataset ready for sentiment and thematic analysis, with over 1,200 reviews collected and preprocessed.


## Task 2: Sentiment and Thematic Analysis

**Objective:** Analyze user sentiment and identify key themes to understand user satisfaction and issues.

**Steps Taken:**

1. **Sentiment Analysis:**

   * Used **TextBlob** to compute polarity scores for each review.
   * Polarity ranges from -1 (negative) to +1 (positive).
   * Saved sentiment scores alongside reviews in the cleaned CSV.

2. **Keyword Extraction & Thematic Analysis:**

   * Identified recurring concepts such as "account", "login error", "slow transfer", and "good UI".
   * Grouped keywords into 3–5 overarching themes per bank (e.g., "Account Access Issues", "Transaction Performance", "User Interface & Experience").
   * Saved the analysis results in a CSV for visualization and reporting.

**Outcome:**

* Each review is assigned a sentiment score and potential theme(s).
* Top keywords per bank provide insight into user satisfaction drivers and pain points.


## Next Step

* do task 3
