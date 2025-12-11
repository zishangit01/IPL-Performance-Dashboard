# 📊 IPL Performance Dashboard (2008–2017)

An interactive **Power BI analytics dashboard** built using 10 years of IPL historical data, covering team performance, player insights, stadium analysis, and match-level trends.

---

## ⭐ Project Overview
This project provides a complete analytical view of IPL performance using **ball-by-ball** and **match-level** datasets.

The dashboard answers important questions such as:
- Season with the highest runs & matches  
- Top batsmen and bowlers  
- Impact of toss on match results  
- Most frequently used stadiums  
- Year-over-year team performance  

---

## 🔍 Business Questions Solved

- Which season recorded the **highest total runs** and **most matches**?  
- Who are the **top batsmen** and **top bowlers** across seasons?  
- Does **winning the toss** increase the chance of winning the match?  
- Which **stadium** has hosted the most matches?  
- What are the **bat/field toss decision trends**?  
- How do teams perform **year-over-year**?

---

## 🏗 Dashboard Pages

### **1️⃣ Season Trends**
- Total Matches Played  
- Total Runs Per Season  
- Total Sixes  
- Total Fours  
- Matches Trend Visualization  
- Team & Season Slicers  

### **2️⃣ Player Analysis**
- Top 10 Batsmen (Total Runs)  
- Top 10 Bowlers (Total Wickets)  

### **3️⃣ Match Analysis**
- Toss Winner vs Match Winner  
- Toss Decision Distribution  
- Stadium Hosting Most Matches  

---

## 🧩 Tech Stack
- **Power BI Desktop**  
- **DAX** (custom KPIs & measures)  
- **CSV Datasets** (matches & deliveries)

---

## 📁 Dataset Description

### **🏏 Matches Dataset**
Contains match-level information:
- Match ID  
- Season  
- City  
- Venue  
- Team1 & Team2  
- Toss Winner  
- Toss Decision  
- Match Winner  

### **🎯 Deliveries Dataset**
Contains ball-by-ball details:
- Batsman  
- Bowler  
- Batsman Runs  
- Extras  
- Boundaries (4s, 6s)  
- Wicket Information  
- Match Reference ID  

---

## 🧮 Key DAX Measures Used

```DAX
Total Sixes = COUNTROWS(FILTER(deliveries, deliveries[batsman_runs] = 6))

Total Fours = COUNTROWS(FILTER(deliveries, deliveries[batsman_runs] = 4))

Total Runs = SUM(deliveries[total_runs])
