# Fantasy-Football-Roster-Optimizer (Integer Linear Programming)

## Project Overview

This project applies Integer Linear Programming (ILP) to optimize Daily Fantasy Sports (DFS) roster construction under real-world constraints. DFS lineup selection is a constrained combinatorial optimization problem: selecting a limited roster from a large player pool while satisfying salary caps and positional requirements.

The goal of this project is to leverage player performance projections and injury filtering to construct high-performing, consistent fantasy lineups.

---

## Motivation

In fantasy football, success depends on selecting the right combination of players to maximize total points. Rather than relying solely on intuition, this project uses mathematical optimization to systematically construct the highest-performing team configuration based on player metrics and positional constraints.

---

## Getting Started

### Dependencies

The libraries needed are pulp, matplotlib, numpy, pandas, streamlit, seaborn, and plotly.

## Methodology

### 1. Data Preparation

* Retrieved projected player performance data from DraftKings
* Performed data cleaning and validation
* Filtered out unavailable players using injury designations (Q, O, IR)
* Ensured feasible and realistic optimization inputs

### 2. Optimization Model

Designed and implemented a Binary Integer Linear Programming (ILP) model to optimize roster selection.

#### Decision Variables

* Binary variables:

  * `1` = player selected
  * `0` = player not selected

#### Objective Function

* Maximize total projected fantasy points

#### Constraints

* Salary cap limit
* Fixed roster size
* Positional requirements (QB, RB, WR, TE, DST)
* FLEX eligibility constraint (RB, WR, TE allowed)

This formulation mirrors real-world resource allocation and knapsack-style optimization problems.

---

## Solution Process

* Constructed the linear programming problem
* Applied salary, positional, and roster constraints
* Solved the ILP model
* Generated the optimal roster
* Identified the FLEX player (RB, WR, or TE)
* Sorted and displayed the final roster with performance metrics

---

## Results

The optimized lineup achieved **142 projected fantasy points**, demonstrating that:

* Integer Linear Programming is an effective framework for DFS lineup construction
* Injury filtering improves feasibility and lineup stability
* Optimization improves lineup consistency compared to manual selection

---

## Conclusion

The Integer Linear Programming (ILP) framework proved to be a validated and effective method for generating optimal, value-driven rosters.

This project successfully demonstrates that combining mathematical optimization with injury-based filtering improves lineup consistency and maximizes projected fantasy performance.

---


### Installing

You can download my program through the "CMSE831_FinalProject_Andrews.ipynb" file attached to the repository.


## Authors

Contributors names and contact info

* Kendall Andrews - Author
* Data: Daily Fantasy Sports - (https://www.dailyfantasyfuel.com/nfl/projections/)
