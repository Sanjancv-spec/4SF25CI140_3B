# Python Fundamentals Challenge - CIE 1 (Milestone 1)

**USN:** 4SF25CI140  
**Section:** 3B  

## Overview
This repository contains the Milestone 1 submission for the Python Fundamentals Challenge. The project analyzes the Kaggle Anime Recommendations Database (~12,300 records) to perform data transformations, handle missing numerical values using mean imputation, extract grouped insights, and visualize patterns.

## Workflow Completed
1. **Data Understanding:** Loaded `anime.csv` using Pandas and examined data types, descriptive statistics, and null counts.
2. **Data Transformation:**
   - Dropped the redundant identifier column `anime_id`.
   - Converted the `episodes` column to numeric (`pd.to_numeric(errors='coerce')`), casting irregular values into NaN.
   - Added a derived feature `members_in_k` (`members / 1000`) for cleaner scale representation.
3. **Null Value Handling (Mean Imputation):**
   - Imputed missing values in `rating` and `episodes` using their respective column means.
4. **Insights Generated:**
   - Analyzed average ratings across different anime formats (`type`).
   - Identified the top 5 genre combinations by total community member engagement.
5. **Data Visualization:** Plotted an average rating bar chart by format and a scatter plot comparing community size against ratings using Matplotlib and Seaborn.

## Files Included
- `anime.csv`: Source dataset.
- `CIE1Milestone.ipynb`: Executed Jupyter Notebook containing code, tables, and generated plots.
- `README.md`: Project summary and workflow documentation.
