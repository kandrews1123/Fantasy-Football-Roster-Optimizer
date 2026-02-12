# Fantasy-Football-Roster-Optimizer

## Project Overview

This project explores Daily Fantasy Sports (DFS) lineup construction as a constrained combinatorial optimization problem. The objective is to select an optimal roster from a large pool of NFL players while satisfying salary cap and positional constraints. Lineup selection is formulated as a binary Integer Linear Programming (ILP) problem (similar to a knapsack problem), where decision variables indicate whether a player is selected.

Using player performance metrics and injury filtering (e.g., removing questionable, doubtful, or injured players), the model constructs high-performing team configurations. The project compares different objective strategies, including maximizing expected fantasy points and incorporating risk-aware metrics (volatility) to improve lineup consistency.

**Research Question:**
Can optimization techniques combined with injury filtering improve lineup consistency and overall fantasy performance?


## Getting Started

### Dependencies

The libraries needed are pulp, matplotlib, numpy, pandas, streamlit, seaborn, and plotly.

### Installing

You can download my program through the "CMSE831_Final Project.ipynb" file attached to the repository.


## Authors

Contributors names and contact info

* Kendall Andrews - Author
* Data: Daily Fantasy Sports - (https://www.dailyfantasyfuel.com/nfl/projections/)
