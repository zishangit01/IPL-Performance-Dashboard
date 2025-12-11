📊 IPL Performance Dashboard (2008–2017)

An interactive Power BI analytics dashboard built using 10 years of IPL historical data, covering team performance, player insights, stadium analysis, and match-level trends.

⭐ Project Overview

This project provides a complete analytical view of IPL performance using ball-by-ball and match-level datasets.

The dashboard answers key questions such as:

🔍 Business Questions Solved

Which season recorded the highest total runs and most matches?

Who are the top batsmen and top bowlers across IPL seasons?

Does winning the toss increase the chance of winning the match?

Which stadium has hosted the most matches?

What are the trends in toss decisions (bat/field)?

How do teams perform year-over-year?

This dashboard is designed for:

👉 Sports analysts, cricket strategists, data analysts, BI developers & students.

🏗 Dashboard Pages
1️⃣ Season Trends

Total Matches Played

Total Runs Per Season

Total Sixes & Fours

Matches Trend Visualization

Team & Season Slicers

2️⃣ Player Analysis

Top 10 Batsmen (by total runs)

Top 10 Bowlers (by total wickets)

3️⃣ Match Analysis

Toss Winner vs Match Winner

Toss Decision Distribution

Stadium Hosting Analysis

🧩 Tech Stack

Power BI Desktop

DAX for calculated measures

CSV datasets (matches & deliveries)

📁 Dataset Description
1️⃣ Matches Dataset

Includes match-level information:

Match ID

Season

City & Venue

Teams (Team1, Team2)

Toss winner & toss decision

Match winner

2️⃣ Deliveries Dataset

Includes ball-by-ball details:

Batsman & Bowler

Runs (batsman runs + extras)

Boundaries (4s, 6s)

Wicket information

Match reference ID

🧮 Key DAX Measures Used
Total Sixes = COUNTROWS(FILTER(deliveries, deliveries[batsman_runs] = 6))

Total Fours = COUNTROWS(FILTER(deliveries, deliveries[batsman_runs] = 4))

Total Runs = SUM(deliveries[total_runs])

🎯 Key Insights

Some seasons show massive spikes in run scoring.

A few stadiums consistently host the highest match counts.

Toss winners tend to win slightly more matches (team-dependent).

Top-performing batsmen and bowlers show consistency across seasons.

📽 Video Explanation Requirement (For Assignment)

Your assignment requires:

✔ 7+ minute explanation video
✔ Explain: dataset, data modelling, visuals & insights
✔ Use this README + your dashboard + PDF report as script support

👤 Author

Zishan Alam
📧 zishanalam101@gmail.com

📍 Data Analyst Enthusiast
