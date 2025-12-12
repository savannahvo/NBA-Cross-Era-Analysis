# Cross-Era NBA Team Performance Analysis (TPI)
## Overview
This project investigates one of basketball’s most debated questions: which historically dominant team stands above the rest—the **1995–96 Chicago Bulls**, the **2015–16 Golden State Warriors**, or the **2024–25 Oklahoma City Thunder**? Each team excelled within its own era, but major changes in pace, shooting philosophy, defensive rules, and player roles make raw statistics incomparable across decades. To overcome these structural differences, we developed the **Team Performance Index (TPI)**, a standardized metric designed to evaluate teams fairly across eras.

TPI incorporates **21 engineered performance metrics** covering offense, defense, and intangibles, weighted 40–40–20 to reflect holistic team performance. All statistics are transformed into **season-normalized z-scores**, eliminating distortions caused by league-wide trends such as rising pace or higher scoring. Playoff games are weighted more heavily (1.5×) to reflect their competitive importance. This normalization framework ensures each team is evaluated relative to its contemporaries rather than by inflated or era-biased totals.

The analysis uses game-level data from the **Historical NBA Dataset** (1947–present). Extensive data preparation, including cleaning raw box scores, merging opponent statistics, correcting mislabeled games, deriving possessions and efficiency metrics, and computing pace-adjusted measures where appropriate was performed. The final dataset includes full offensive and defensive profiles for all three target teams throughout their seasons.


Through standardized metrics and thoughtful visual design, this project provides a balanced, data-driven evaluation of three iconic teams. The TPI framework allows for fair cross-era comparison, revealing how each team performed relative to the expectations and norms of its basketball era. In doing so, it transforms a long-standing subjective debate into a rigorous analytical assessment of historical team greatness.

---
## Core Structure of the Team Performance Index (TPI)
This weighting reflects the idea that elite teams are driven primarily by two-way performance with intangibles acting as a meaningful but secondary differentiator.

The final TPI score is calculated as: TPI = (0.40 x Offense Score) + (0.40 x Defense Score) + (0.20 x Intangibles Score) 

---
## Offensive Component (40%)
Ten offensive metrics that collectively describes a team's scoring efficiency, shooting profile, playmaking, ball security, and second-chance creation. All ten metrics are incorporated into the Total Performance Index (TPI) to produce a multi-dimensional view of offensive strength

#### Core Efficiency Metrics:
1. Offensive Rating (ORtg) Points scored per 100 possessions. This metric is inherently pace-adjusted and is one of the most important indicators of offensive performance.
2. True Shooting Percentage (TS%) Comprehensive shooting efficiency that accounts for the value of three-point shots and the bonus efficiency from free throws.
**3. Effective Field Goal Percentage (eFG%)** Field goal percentage adjusted for the added value of made three-point shots.
**4. Field Goal Percentage (FG%)** Basic shooting efficiency measuring made field goals relative to attempts

#### Volume and Style Metrics:
**5. True Shooting Attempts (TSA)** Represents total shooting volume; incorporating both field goal attempts and free throw attempts (scaled by 0.44).
**6. Free Throw Rate (FT Rate)** Frequency of free throw attempts relative to field goal attempts, capturing aggression and rim pressure.
**7. Three-Point Rate (3PT Rate)** Share of field goal attempts that come from beyond the arc, reflecting offensive shot selection and spacing.

#### Playmaking and Ball Security:
**8. Assist Ratio** Assists per made field goal, indicating ball movement and play creation efficiency.
**9. Assist-to-Turnover Ratio (AST/TOV)** Balances playmaking and ball security by measuring assists relative to turnovers.

#### Second-Chance and Transition:
**10. Offensive Rebound Percentage (ORB%)** Percentage of available offensive rebounds secured, capturing second-chance creation and transition pressure potential.

