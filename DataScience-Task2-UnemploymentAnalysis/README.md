# Unemployment Analysis in India

## Project Overview
This project explores unemployment trends in India using Python, Pandas, Matplotlib, and Seaborn. It examines changes over time, differences between rural and urban areas, regional variation, and the distribution of unemployment rates.

## Objectives
- Analyze monthly unemployment trends from 2019 to 2020.
- Compare unemployment rates in rural and urban areas.
- Identify regions with higher average unemployment rates.
- Examine the distribution of unemployment-rate observations.
- Summarize insights through data visualizations.

## Dataset
The analysis uses the Kaggle dataset **Unemployment in India**, containing regional unemployment estimates, dates, employment estimates, labour participation rates, and rural/urban classifications.

The main dataset covers May 2019 to June 2020. After cleaning invalid dates, 740 of the original 768 records were retained.

## Tools and Libraries
- Python
- Pandas and NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Data Cleaning
- Removed leading and trailing whitespace from date values and text columns.
- Converted dates to datetime format.
- Converted numerical columns to numeric data types.
- Excluded records with invalid dates.
- Verified that the cleaned dataset contained no missing values in the analyzed columns.

## Key Findings
1. Monthly average unemployment rates remained approximately between 9% and 10% for much of the period before rising sharply in April and May 2020.
2. The monthly average peaked at approximately 24.9% in May 2020 before declining in June.
3. Urban records had a higher average unemployment rate than rural records in this dataset.
4. Tripura and Haryana had the highest regional average unemployment rates among the regions shown.
5. The distribution was right-skewed, with most observations at lower rates and a smaller number of unusually high values.

## Visualizations
1. Monthly average unemployment rate trend.
2. Rural versus urban unemployment comparison.
3. Average unemployment rate by region.
4. Distribution of unemployment-rate observations.

## Limitations
- The dataset covers a limited historical period and should not be interpreted as a description of current unemployment.
- The analysis uses averages of available records, which may not equal population-weighted national estimates.
- The observed increase in 2020 coincides with the COVID-19 lockdown period, but this analysis alone cannot establish causation.
- Invalid-date records were excluded, which may affect results if those records differ systematically from the retained data.

## Conclusion
This project demonstrates how Python-based exploratory data analysis can reveal temporal patterns, regional differences, and variation in unemployment estimates. The visualizations provide a starting point for understanding the dataset while highlighting the importance of data quality and careful interpretation.
