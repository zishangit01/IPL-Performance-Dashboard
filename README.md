🏏 IPL Performance Dashboard (2008–2017)

An interactive Power BI Dashboard analysing 10 years of IPL historical data covering team trends, player insights & match analysis.

📌 Project Overview

This project provides a complete analytical view of IPL performance using ball-by-ball and match-level datasets.
The dashboard answers key business questions such as:

Which season had the highest runs and matches?

Who are the top batsmen & bowlers across all seasons?

Does winning the toss increase chances of winning the match?

Which stadium hosted the most matches?

How do teams perform year-by-year?

This dashboard is designed for sports analysts, cricket strategists, students, and business intelligence learners.

📂 Repository Structure
IPL-Performance-Dashboard/
│── IPL Dashboard.pbix
│── Dataset/
│     ├── matches.csv
│     ├── deliveries.csv
│── Images/
│     ├── image1.png
│     ├── image2.png
│── Project Report.pdf
│── Business Requirement.pdf
│── README.md   ← (you are here)

🗂 Dataset Description
1️⃣ Matches Dataset

Contains match-level information such as:

Match ID

Season

Teams

Venue

Toss winner & toss decision

Match winner

Player of the match

2️⃣ Deliveries Dataset

Contains ball-by-ball data:

Batsman

Bowler

Runs scored (batsman_runs)

Extras, wides, no-balls

Wickets

🔗 Data Model

A single relationship powers the entire model:

matches[id]  ───►  deliveries[match_id]


This enables season/team filters to flow across all visuals.

📊 Dashboard Features
✔ 1. Key Performance Indicators

Total Matches Played

Total Runs Scored

Total Sixes Hit

Total Fours Hit

✔ 2. Season Trends

📈 Line chart: Total Runs Per Season
📊 Bar chart: Matches Played Per Season

✔ 3. Player Performance

🏏 Top 10 Batsmen by Total Runs
🎯 Top 10 Bowlers by Total Wickets

✔ 4. Match Analysis

Impact of Toss Winner on Match Winner

Toss Decision Distribution (Bat/Field %)

Most Matches Hosted by Venue

🛠 DAX Measures Used
Total Runs = SUM(deliveries[batsman_runs])

Total Fours = COUNTROWS(FILTER(deliveries, deliveries[batsman_runs] = 4))

Total Sixes = COUNTROWS(FILTER(deliveries, deliveries[batsman_runs] = 6))

Matches Played = COUNT(matches[id])

🖥 Screenshots

(Add images from your Images/ folder here)

![Dashboard Screenshot](Images/image1.png)
![Player Analysis](Images/image2.png)

📥 How to Use

Download the IPL Dashboard.pbix file

Open in Power BI Desktop

Explore with interactive slicers (Team, Season Range)

🎯 Business Impact

This dashboard helps stakeholders:

Identify top-performing players for team selection

Analyse scoring trends for strategic decisions

Understand season growth patterns

Measure stadium-wise audience engagement

👨‍💻 Created By

Zishan Alam
(Data Analyst - Power BI, SQL, Excel)
