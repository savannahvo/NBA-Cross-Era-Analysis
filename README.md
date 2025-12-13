# Cross-Era NBA Team Performance Analysis (TPI)
## Overview
This project investigates one of basketball’s most debated questions: which historically dominant team stands above the rest—the **1995–96 Chicago Bulls**, the **2015–16 Golden State Warriors**, or the **2024–25 Oklahoma City Thunder**? Each team excelled within its own era, but major changes in pace, shooting philosophy, defensive rules, and player roles make raw statistics incomparable across decades. To overcome these structural differences, we developed the **Team Performance Index (TPI)**, a standardized metric designed to evaluate teams fairly across eras.

TPI incorporates **21 engineered performance metrics** covering offense, defense, and intangibles, weighted 40–40–20 to reflect holistic team performance. All statistics are transformed into **season-normalized z-scores**, eliminating distortions caused by league-wide trends such as rising pace or higher scoring. Playoff games are weighted more heavily (1.5×) to reflect their competitive importance. This normalization framework ensures each team is evaluated relative to its contemporaries rather than by inflated or era-biased totals.

The analysis uses game-level data from the **Historical NBA Dataset** (1947–present). Extensive data preparation, including cleaning raw box scores, merging opponent statistics, correcting mislabeled games, deriving possessions and efficiency metrics, and computing pace-adjusted measures where appropriate was performed. The final dataset includes full offensive and defensive profiles for all three target teams throughout their seasons.


Through standardized metrics and thoughtful visual design, this project provides a balanced, data-driven evaluation of three iconic teams. The TPI framework allows for fair cross-era comparison, revealing how each team performed relative to the expectations and norms of its basketball era. In doing so, it transforms a long-standing subjective debate into a rigorous analytical assessment of historical team greatness.

---
## Interactive Tableau Dashboard

