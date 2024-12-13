# Cookie Cats A/B Testing Analysis

## Project Overview
This project analyzes A/B test results from Cookie Cats, a popular mobile puzzle game. The test examined the impact of moving the first gate (where players must wait or pay to continue playing) from level 30 to level 40, focusing on player retention and engagement metrics.

## Business Problem
In Cookie Cats, players complete different levels and occasionally encounter gates that force them to wait or make an in-game purchase to progress. The current version of the game has the first gate at level 30. The product team wanted to test if moving this gate to level 40 would improve player retention.

## Dataset Description
The dataset includes:
- Player IDs
- Game version (gate at level 30 or 40)
- Number of game rounds played
- 1-day retention (boolean)
- 7-day retention (boolean)

## Analysis Methodology

### Metrics Analyzed
- Day-1 retention rates
- Day-7 retention rates
- Number of game rounds played

### Statistical Methods
- Chi-square tests for retention metrics
- T-tests for game rounds comparison
- Effect size analysis with relative differences

### Key Parameters
- Significance level (α): 0.05
- Statistical power: 0.80
- Minimum detectable effect: 10%

## Results

### Statistical Significance
1. Day-1 Retention
   - Not statistically significant (p = 0.0755)
   - Relative difference: -1.32%

2. Day-7 Retention
   - Statistically significant (p = 0.0016)
   - Relative difference: -4.31%

3. Game Rounds
   - Not statistically significant (p = 0.3729)
   - Relative difference: -2.21%

### Key Findings
- Moving the gate to level 40 resulted in a significant decrease in 7-day retention
- All metrics showed negative trends, though only 7-day retention was statistically significant
- The 4.31% decrease in 7-day retention is both statistically and practically significant

## Recommendation
Based on the analysis, the recommendation is to keep the gate at level 30 (control version) because:
1. Moving the gate to level 40 shows a significant negative impact on 7-day retention
2. All metrics show negative trends
3. There are no offsetting positive effects in other metrics to justify the change

## Technical Implementation
- Language: Python
- Key Libraries:
  - pandas
  - numpy
  - scipy.stats
  - statsmodels
  - matplotlib
  - seaborn

## Repository Structure
```
├── data/
│   └── cookie_cats.csv
├── notebooks/
│   └── AB_Testing_CookieCats.ipynb
├── README.md
```

## Getting Started
1. Clone the repository
2. Install required packages: `pip install -r requirements.txt`
3. Open and run the Jupyter notebook to see the detailed analysis

