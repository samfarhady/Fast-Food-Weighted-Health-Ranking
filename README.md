# Fast-Food-Weighted-Health-Ranking

## Overview
Comparative nutritional analysis of 6 major fast food chains (Burger King, McDonald's, 
Wendy's, KFC, Taco Bell, Pizza Hut) to determine relative healthiness based on 
average menu item composition.

## Dataset
- Source: Kaggle — Fast Food Nutrition Menu V2
- ~1140 menu items across 6 chains after cleaning

## Methodology
- Cleaned missing values via median imputation; dropped columns with >50% missing data
- Selected 7 nutrients for analysis: saturated fat, trans fat, cholesterol, sodium, 
  sugar, fiber, and protein
- Deliberately excluded calories, carbs, and total fat — high values in these are 
  not inherently negative or positive
- Ranked each chain per nutrient (ascending for unhealthy, descending for healthy)
- Computed a composite weighted ranking across all 7 nutrients

## Key Findings
- Burger King ranks as the least healthy chain overall (composite score: 2.14)
- Pizza Hut ranks as the most healthy (composite score: 4.57)
- One-way ANOVA confirmed statistically significant differences across chains 
  for all 7 nutrients (all p < 0.05), validating the ranking methodology

## Tools
Python, Pandas, NumPy, Matplotlib, Seaborn, SciPy
