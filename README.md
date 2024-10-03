# Impact of Posting Restrictions on User Retention in a Social Media Setting

## Overview

This project explores the effect of limiting the number of posts a user can make per day on 7-day retention rates in a social media startup setting. Using engagement metrics from over 90,000 users, I analyzed whether imposing posting restrictions helps retain users over time. This analysis is crucial for understanding how posting behaviors impact user satisfaction and engagement, ultimately informing strategies to increase platform retention.

**Repository Contents:**
- **`Impact_of_Posting_Restriction_Analysis.Rmd`**: The main R Markdown file containing code, analysis, and visualizations.
- **`platform_retention.csv`**: The dataset used for analysis.
- **`visualizations/`**: Directory containing images and plots generated during the analysis.
- **`README.md`**: Project overview and guidance.

## Project Motivation

The social media landscape is highly competitive, and user engagement is a key performance indicator for platform success. This project addresses whether implementing restrictions on user posting frequency can enhance user retention, which could have implications for content moderation strategies and community management.

## Research Questions

1. **Does limiting the number of posts a user can make per day improve 7-day retention rates compared to unrestricted posting?**
2. What impact does posting restriction have on other engagement metrics, such as the number of site visits within the first 7 days of registration?
3. Are there significant differences in 1-day retention rates between the limited and unlimited posting models?

## Dataset

- **Source**: Proprietary engagement data from a social media startup (simulated for this project).
- **Total Users Analyzed**: 90,189 users
- **Variables**:
  - `version`: The assigned posting model (`limited` or `unlimited`).
  - `retention_7`: Binary variable indicating whether a user was active 7 days after registration.
  - `site_visits_7`: Number of site visits within the first 7 days.
  - `retention_1`: Binary variable indicating whether a user was active 1 day after registration.

## Methodology

The analysis was conducted in the following steps:

1. **Data Cleaning and Preparation**:
   - Checked for missing values, outliers, and inconsistencies.
   - Filtered and transformed variables for easier interpretation and visualization.

2. **Exploratory Data Analysis (EDA)**:
   - Visualized 7-day retention rates across different posting models.
   - Created histograms to understand the distribution of site visits and retention rates.

3. **Statistical Testing**:
   - Conducted a difference of proportion test to evaluate the significance of the impact of posting restrictions on 7-day retention rates.
   - Performed a two-sample t-test to explore differences in site visits between the two posting models.
   - Used a chi-square test to analyze the association between posting model and 1-day retention.

## Key Findings

1. **7-Day Retention**:
   - There is a statistically significant increase in 7-day retention for the limited posting model compared to the unlimited model.
   - **P-value**: 0.00052, indicating strong evidence that limiting posts positively impacts retention.

2. **Site Visits**:
   - There was no significant difference in the number of site visits between the two posting models.
   - **P-value**: 0.23, suggesting that the posting model does not influence how frequently users visit the site.

3. **1-Day Retention**:
   - No significant association was found between the posting model and 1-day retention.
   - **P-value**: 0.098.


## Conclusion

Limiting the number of posts a user can make per day has a positive impact on 7-day retention rates, with an increase ranging from 0.43% to 1.3%. However, the posting restriction does not significantly affect other engagement metrics like site visits or 1-day retention. This suggests
