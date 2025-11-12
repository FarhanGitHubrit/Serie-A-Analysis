# Serie-A-Analysis
A Power BI dashboard analyzing Serie A 2024/25 teams’ offensive and defensive performance. Includes custom DAX KPIs, shot efficiency, defensive efficiency, and xGA vs GA analysis. Visuals: matrix, KPI cards, scatter, and area charts for insight-driven performance tracking.

📊 Project Overview

This Power BI project analyzes Serie A 2024/25 team performance, focusing on offensive and defensive efficiency.
It uses DAX measures, KPI indicators, and interactive visuals to explore how each team performs in attack and defense — comparing actual outcomes with expected metrics such as Goals Against (GA) and Expected Goals Against (xGA).

🧩 Key Objectives

Compare Offensive vs Defensive performance across Serie A teams
Identify teams with strong or weak defenses
Visualize expected vs actual goals conceded (xGA vs GA)
Track Efficiency metrics using KPIs and color-coded matrices
Deliver actionable insights through Power BI storytelling

🧮 DAX Measures Created

| **Measure Name**                      | **Description**                                                                    |
| ------------------------------------- | ---------------------------------------------------------------------------------- |
| `DefensiveEfficiency`                 | `(Tackles_Won / Defensive_Actions) * 100` — measures overall defensive efficiency. |
| `BlockRate`                           | `(Blocks / Shots_on_Target) * 100` — measures defensive block success.             |
| `Goals Conceded per Match`            | `GoalsAgainst / MatchesPlayed` — average goals conceded per match.                 |
| `Goal Conversion Rate`                | `(Goals / Shots_on_Target) * 100` — measures attacking conversion efficiency.      |
| `Shot Accuracy %`                     | `(Shots_on_Target / Total_Shots) * 100` — measures shooting accuracy.              |
| `Offensive Strength Index`            | Composite measure combining goals, assists, and xG data.                           |
| `Avg_GA`, `Avg_xGA`, `Avg_TacklesWon` | League average benchmarks for KPI comparison.                                      |
| `Target50`                            | Static target benchmark measure (value = 50).                                      |


🧠 Key Metrics Explained

| **Abbreviation** | **Full Name**          | **Meaning**                                     |
| ---------------- | ---------------------- | ----------------------------------------------- |
| GA               | Goals Against          | Total goals conceded by a team.                 |
| xGA              | Expected Goals Against | Predicted goals conceded based on shot quality. |
| GD               | Goal Difference        | Goals scored minus goals conceded.              |
| Tackles_Won      | Successful Tackles     | Defensive tackles successfully completed.       |
| Interceptions    | Ball Interceptions     | Number of times the team intercepted the ball.  |


📈 Power BI Pages & Visuals

| **Page** | **Title**                       | **Description**                                      | **Visuals Used**                               |
| -------- | ------------------------------- | ---------------------------------------------------- | ---------------------------------------------- |
| Page 1   | Overall Team Summary            | Overview of team performance metrics                 | KPI Cards, Table, Clustered Bar Chart          |
| Page 2   | Offensive vs Defensive Analysis | Comparison between attacking and defensive strengths | Stacked Column, Donut, Scatter, Ribbon, Matrix |
| Page 3   | Defensive Analysis Summary      | In-depth defensive performance insights              | Matrix, Area Chart, KPI Cards, Bar Chart       |


🎨 Conditional Formatting & Insights
Color gradients applied to Matrix visuals to highlight performance differences:

| **Metric**                            | **High = Good?** | **Color Direction**            |
| ------------------------------------- | ---------------- | ------------------------------ |
| GA, xGA                               | ❌ No             | Green → Red (lower is better)  |
| Tackles_Won, Interceptions, Pressures | ✅ Yes            | Red → Green (higher is better) |


🧭 Insights Gained
Teams with low GA and xGA show strong defensive structures.

A large gap between xGA and GA reveals over- or under-performance defensively.
High Tackles_Won and Interceptions correlate with fewer goals conceded.
Offensive Strength Index identifies the most efficient attacking sides.

🛠️ Tools & Technologies

| **Tool**        | **Purpose**                                 |
| --------------- | ------------------------------------------- |
| Power BI        | Data visualization, KPI cards, DAX measures |
| Microsoft Excel | Data cleaning & preprocessing               |
| DAX             | Custom calculations for KPIs and ratios     |
| CSV Dataset     | Source data: `SerieA_Team_Full_Renamed.csv` |


📸 Dashboard Highlights
Interactive slicers for team comparison
Matrix with conditional formatting for instant defensive insight
Dynamic KPIs with benchmark targets
Area charts for overall performance trends

📌 Future Enhancements
Add player-level breakdowns
Include matchday-wise trends
Build ML predictions for next-season performance
