📊 IPL Performance Dashboard (2008–2017)

An interactive Power BI analytics dashboard built using 10 years of IPL historical data, covering team trends, player insights, and match-level performance.

⭐ Project Overview

This project delivers a complete analytical view of IPL performance using ball-by-ball and match-level datasets.
The dashboard answers key business questions such as:

🔍 Business Questions Solved

Which season recorded the highest total runs and matches?

Who are the top batsmen and top bowlers across IPL seasons?

Does winning the toss increase the probability of winning the match?

Which stadium has hosted the most matches?

What are the batting/fielding toss decisions trends?

How do teams perform year-over-year?

This dashboard is designed for:
👉 Sports analysts, cricket strategists, data analysts, BI developers, and students.

🏗 Dashboard Pages
1️⃣ Season Trends

Total Matches Played

Total Runs Per Season

Total Sixes Hit

Total Fours Hit

Matches Trend Visualization

Team & Season Slicers

2️⃣ Player Analysis

Top 10 Batsmen by Total Runs

Top 10 Bowlers by Total Wickets

3️⃣ Match Analysis

Impact of Toss Winner on Match Winner

Toss Decision Distribution

Most Matches Hosted by Stadium

🧩 Tech Stack

Power BI Desktop

DAX for custom KPIs

CSV datasets (matches & deliveries)

🗂 Repository Structure
IPL-Performance-Dashboard/
│── IPL Dashboard.pbix
│── README.md
│── Project Report.pdf
│── Business Requirement.pdf
│── Dataset/
│     ├── matches.csv
│     ├── deliveries.csv
│── Images/
      ├── image1.png
      ├── image2.png
      ├── image3.png

📁 Dataset Description
1️⃣ Matches Dataset

Contains match-level information such as:

Match ID

Season

City

Venue

Team1 & Team2

Toss winner & Toss decision

Match winner

2️⃣ Deliveries Dataset

Contains ball-by-ball details:

Batsman & bowler

Runs (batsman + extras)

Boundaries (4s, 6s)

Wickets information

Match reference ID

🧮 Key DAX Measures Used
Total Sixes = COUNTROWS(FILTER(deliveries, deliveries[batsman_runs] = 6))

Total Fours = COUNTROWS(FILTER(deliveries, deliveries[batsman_runs] = 4))

Total Runs = SUM(deliveries.total_runs)

🎯 Key Insights

Some seasons show massive spikes in total runs.

A few stadiums host consistently high numbers of matches.

Toss winners win slightly more matches — but it varies by team.

Top-performing batsmen and bowlers remain consistent across seasons.

📽 Explanatory Video Requirement

Your assignment requires:
✔ 7+ minute video explanation
✔ Explain: dataset, modelling, visuals, insights

You can use this README + your dashboard + your PDF report for scripting.

👤 Author

Zishan Alam
📧 zishanalam101@gmail.com

📍 Data Analyst Enthusiast
