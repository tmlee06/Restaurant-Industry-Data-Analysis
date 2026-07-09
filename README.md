# Restaurant Industry Data Science Project

This repository contains my completed **DSC 10 midterm project**, where I analyzed restaurant industry data using Python and `babypandas`.

The project combines:
- data cleaning
- grouped summaries
- sorting and filtering
- feature engineering
- string processing
- table merges
- data visualization
- exploratory data analysis

## Project Overview

The goal of this project is to explore patterns across several restaurant datasets and answer questions about:

- large chain restaurants
- top independent restaurants
- fast-growing restaurant brands
- city-level restaurant trends
- Yelp ratings and customer perception

Using `babypandas`, the notebook investigates how restaurant sales, growth, pricing, location, and ratings relate to one another.

## Files Used

- `midterm-project.ipynb`  
  Main notebook containing the full analysis, code, visualizations, and written answers.

- `Top250.csv`  
  Data on the top 250 chain restaurants, including sales, year-over-year sales growth, units, and segment categories.

- `Independents100.csv`  
  Data on the top 100 independent restaurants, including sales, average check, city, state, and meals served.

- `Future50.csv`  
  Data on fast-growing restaurant brands, including location, sales, and growth metrics.

- `Yelp.csv`  
  Yelp ratings for restaurants used to compare ratings with restaurant pricing and geography.

- `populations.csv`  
  City population data used to normalize restaurant counts and compare food activity across cities.

## Main Questions Explored

### Part 1. Chains
This section focuses on large chain restaurants and segment-level trends.

Some of the questions explored include:
- Which segment categories appear most often among the top 250 chains?
- Which restaurant segments have the highest average sales?
- How do quick service chains compare to non-quick service chains in average sales?
- How can percent growth strings be converted into usable numeric values?
- Which chains fall into the highest growth category?
- Which segment categories appear strongest for future investment?

Key findings from this section include:
- Quick service restaurants had about **$1,700.61 million** higher average sales than non-quick service restaurants.
- The highest-selling segment categories were led by:
  - **Quick Service & Burger**
  - **Quick Service & Mexican**
  - **Quick Service & Coffee Cafe**
- Based on mean growth category, the three strongest segment categories were:
  - **Quick Service & Chicken**
  - **Quick Service & Pizza**
  - **Quick Service & Mexican**

### Part 2. Cities
This section shifts to city-level analysis using the independent restaurant and Future 50 datasets.

The notebook explores:
- which restaurants have the highest and lowest average check or sales per meal
- which cities have the highest typical restaurant prices
- how independent-restaurant activity compares to emerging-brand activity
- how city population affects restaurant concentration

Key findings from this section include:
- **Alinea** in **Chicago** had the highest average check at **$650**.
- **Pancake Pantry** had the lowest sales per meal at about **$16.58**.
- Among cities with at least three restaurants in the dataset, **Las Vegas** and **Miami Beach** had the highest median average checks.
- After adjusting for population, **West Hollywood** emerged as the “foodiest” city in the analysis.

### Part 3. Stars
This section merges restaurant data with Yelp ratings to study how ratings relate to price and location.

The notebook explores:
- how to clean restaurant names before merging datasets
- which restaurants appear multiple times across cities
- which states have higher proportions of highly rated restaurants
- how average check changes with rating
- which restaurants have the lowest Yelp ratings in the merged data
- how median average check varies by both city and rounded rating

Key findings from this section include:
- Duplicate restaurant names across cities included:
  - **Beauty & Essex**
  - **Gibsons Bar & Steakhouse**
  - **Joe's Seafood, Prime Steak & Stone Crab**
  - **Maple & Ash**
- The five lowest-rated restaurants in the merged dataset were:
  - **Paradise Cove Beach Cafe**
  - **Whiskey Joe's Tampa**
  - **Grand Central Oyster Bar**
  - **Gladstones**
  - **Frankenmuth Bavarian Inn**
- The average check among those five lowest-rated restaurants was **$46.80**.

## Methods and Skills Demonstrated

This project demonstrates:
- reading CSV files with `babypandas`
- selecting and transforming columns
- grouping and aggregation with `groupby`
- sorting and filtering tables
- writing helper functions for data cleaning
- converting strings to numeric features
- merging multiple datasets
- creating scatter plots, bar charts, and histograms
- drawing conclusions from real-world business data

## Tools and Libraries

This project was completed in Python using:
- `babypandas`
- `numpy`
- `matplotlib`
- `otter-grader`

## Results

All graded notebook checks passed successfully.

The final notebook output shows:
- all Part 1 graded questions passed
- all Part 2 graded questions passed
- all Part 3 graded questions passed

## How to Run

1. Clone this repository.
2. Make sure the CSV files are available in the expected data folder or update the file paths in the notebook.
3. Install the required packages.
4. Open and run `midterm-project.ipynb` in Jupyter Notebook or JupyterLab.

Example install command:

```bash
pip install babypandas numpy matplotlib otter-grader
```

## Notes

- This project was designed in the style of a course notebook, so some answers are embedded directly in notebook cells rather than separated into scripts.
- Several questions involve visual analysis through plots, so opening the notebook is the best way to see the full project.
- The repository is best structured with the notebook and all CSV files included together.
