# Cookie Cats A/B Testing Analysis 

## Introduction
This project analyzes player retention in the mobile puzzle game Cookie Cats through A/B testing. The analysis focuses on the impact of moving the first gate from level 30 to level 40, providing insights into optimal game design and player engagement strategies.

## Problem Statement
Cookie Cats implements gates that require players to either wait or pay to continue playing. The key question is: Does moving the first gate from level 30 to level 40 impact player retention? This analysis helps in determining the optimal gate placement for maximizing player engagement while maintaining a balanced gaming experience.

## Dataset
The dataset contains:
- `userid`: Unique identifier for each player
- `version`: Game version ('gate_30' or 'gate_40')
- `sum_gamerounds`: Number of game rounds played
- `retention_1`: Player returned after 1 day (True/False)
- `retention_7`: Player returned after 7 days (True/False)

## Analysis Overview
This project investigates:
- Comparison of 1-day and 7-day retention rates between control (gate_30) and treatment (gate_40) groups
- Statistical significance testing of retention differences
- Player engagement patterns across different gate placements


## Key Findings
1. Retention Rate Analysis:
   - Detailed comparison of retention metrics
   - Impact on short-term vs long-term retention
   - Statistical significance of observed differences

2. Player Behavior Insights:
   - Game rounds distribution analysis
   - Engagement patterns before and after gate encounter
   - Player progression analysis



## Technologies Used
- Python 
- Pandas for data manipulation
- NumPy for numerical computations
- SciPy for statistical analysis
- Matplotlib and Seaborn for visualization
- Jupyter for interactive analysis


