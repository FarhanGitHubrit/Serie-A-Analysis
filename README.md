# Serie-A-Analysis
A Power BI dashboard analyzing Serie A 2024/25 teams’ offensive and defensive performance. Includes custom DAX KPIs, shot efficiency, defensive efficiency, and xGA vs GA analysis. Visuals: matrix, KPI cards, scatter, and area charts for insight-driven performance tracking.

📊 Project Overview

This Power BI project analyzes Serie A 2024/25 team performance with a focus on offensive and defensive efficiency.
It uses DAX measures, KPI indicators, and interactive visuals to uncover how each team performs in attack and defense, comparing actual outcomes with expected metrics such as Goals Against (GA) and Expected Goals Against (xGA).

🧩 Key Objectives

Compare Offensive vs Defensive performance across Serie A teams

Identify teams with strong or weak defensive structures

Visualize expected vs actual goals conceded (xGA vs GA)

Track Defensive & Offensive efficiency using KPIs and color-coded matrices

Provide actionable insights through clear Power BI storytelling

🧮 DAX Measures Created
Measure Name	Description
DefensiveEfficiency	(Tackles_Won / Defensive_Actions) * 100 — measures how efficient a team is defensively.
BlockRate	(Blocks / Shots_on_Target) * 100 — represents block success rate.
Goals Conceded per Match	GoalsAgainst / MatchesPlayed — average goals conceded per match.
Goal Conversion Rate	(Goals / Shots_on_Target) * 100 — shows offensive efficiency.
Shot Accuracy %	(Shots_on_Target / Total_Shots) * 100 — measures precision in attack.
Offensive Strength Index	Composite measure combining goals, assists, and xG metrics.
Avg_GA, Avg_xGA, Avg_TacklesWon	League average benchmarks for comparison.
Target50	Static KPI benchmark for comparison (value = 50).
🧠 Key Metrics Explained
Abbreviation	Full Name	Meaning
GA	Goals Against	Total number of goals conceded by a team.
xGA	Expected Goals Against	Estimated goals a team was likely to concede based on shot quality.
GD	Goal Difference	Difference between goals scored and goals conceded.
Tackles_Won	Successful Tackles	Number of defensive tackles successfully completed.
Interceptions	Ball Interceptions	Number of times the team intercepted the ball.

📈 Power BI Pages & Visuals
Page	Title	Description	Visuals Used
Page 1	Overall Team Summary	Overview of team performance	KPI Cards, Table, Clustered Bar Chart
Page 2	Offensive vs Defensive Analysis	Compares attacking and defensive strengths	Stacked Column, Donut, Scatter, Ribbon, Matrix
Page 3	Defensive Analysis Summary	Focused analysis of defensive metrics	Matrix, Area Chart, KPI Cards, Bar Chart
🎨 Conditional Formatting & Insights

Color gradients applied in Matrix visuals to distinguish performance levels:

Metric	High = Good?	Color Direction
GA, xGA	❌ No	Green → Red (lower is better)
Tackles_Won, Interceptions, Pressures	✅ Yes	Red → Green (higher is better)

💡 This helps highlight top defensive teams (in green) and struggling defenses (in red).

🧭 Insights Gained

Teams with low xGA and GA indicate strong defensive organization.

Discrepancy between xGA and GA shows underperforming or overperforming defenses.

Higher Tackles_Won and Interceptions correlate with fewer goals conceded.

The Offensive Strength Index identifies efficient attacking sides.

🛠️ Tools & Technologies
Tool	Purpose
Power BI	Data visualization, KPI creation, DAX modeling
Microsoft Excel	Data cleaning and preprocessing
DAX (Data Analysis Expressions)	Custom measures and calculations
CSV Dataset	Source file: SerieA_Team_Full_Renamed.csv
📁 Dataset Info

The dataset includes comprehensive Serie A stats:

Team-level attributes (Squad, Goals, Assists, xGA, Tackles, Interceptions, Pressures, etc.)

Offensive and defensive action metrics

Expected goals data for deeper performance insights

📸 Dashboard Highlights

Interactive visuals with slicers for team comparison

Matrix with conditional formatting for quick defensive insight

Dynamic KPIs showing deviation from league averages

Area charts for total performance trends

📌 Future Enhancements

Integrate player-level breakdown for deeper analytics

Include matchday-wise performance trends

Use ML-based predictions for next-season performance
