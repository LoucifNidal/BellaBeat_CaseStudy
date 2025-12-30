# Bellabeat Case Study – Smart Device Usage Analysis  
**Junior Data Analyst | Marketing Analytics**

![Dashboard Preview](images/dashboard.png)

---

## 📌 Project Overview
Bellabeat is a high-tech company that manufactures health-focused smart products for women.  
This case study analyzes **smart device fitness data** to uncover user behavior patterns and provide **data-driven marketing insights** that support business growth.

The analysis focuses on **non-Bellabeat smart device usage** to identify trends that can be applied to Bellabeat’s ecosystem, particularly the **Bellabeat App** and **Leaf device**.

---

## 🎯 Business Objective
**Primary Goal:**  
Analyze smart device usage data to understand how consumers engage with fitness tracking features and translate insights into **actionable marketing recommendations**.

**Key Questions:**
- What trends exist in smart device usage?
- How do users balance activity, sleep, and sedentary behavior?
- How can these insights inform Bellabeat’s marketing strategy?

---

## 👥 Stakeholders
- **Urška Sršen** – Co-Founder & Chief Creative Officer  
- **Sando Mur** – Co-Founder  
- **Bellabeat Marketing Analytics Team**

---

## 🧠 Product Focus
- **Bellabeat App** (Primary platform for user engagement)
- **Leaf Device** (Data input source feeding the app)

---

## 📂 Data Source
**FitBit Fitness Tracker Data** (Kaggle – CC0 Public Domain)

- Data collected from Fitbit users who consented to share activity and sleep data
- Dataset includes **18 CSV files** at different time granularities
- Data timeframe: **2016**

---

## ⚠️ Data Limitations (ROCCC Assessment)
- **Reliable:** Real user-generated device data
- **Original:** Device-level data shared publicly
- **Comprehensive:** Limited (small sample size, no demographics)
- **Current:** Not current (2016 data)
- **Cited:** Openly licensed (CC0)

👉 Insights are **directional**, not conclusive.

---

## 🧹 Data Preparation & Cleaning
To reduce complexity and ensure consistency, only **daily-level datasets** were used:

**Selected Datasets**
- `dailyActivity_merged.csv`
- `dailySteps_merged.csv`
- `sleepDay_merged.csv`

**Key Issues Identified**
- Duplicate user IDs across dates
- Inconsistent date formats
- Redundant time values (12:00 AM)
- Mixed time granularities
- Unnecessary columns

**Cleaning Actions**
- Removed duplicate daily records
- Standardized date formats
- Aligned datasets by date range
- Retained only analysis-relevant columns
- Verified absence of NULL values

---

## 🛠 Tools & Techniques
**Tool Used:**  
- **Google Sheets** (cleaning, analysis, visualization)

### Functions & Methods Used (Light Technical Overview)
- `UNIQUE()` – identify distinct user IDs
- `AVERAGE()` / `AVERAGEIF()` – calculate user-level metrics
- `COUNTIF()` – activity category distribution
- `IF()` – classify activity levels
- Conditional formatting – highlight patterns
- Unit conversion (minutes → hours)
- Sorting & filtering – integrity checks
- Pivot-style summaries – activity & sleep aggregation

---

## 📊 Analysis & Key Insights

### 1️⃣ Steps Analysis
Users were categorized by average daily steps:

| Activity Level | Daily Steps |
|----------------|------------|
| Low | < 5,000 |
| Moderate | 5,000 – 8,000 |
| High | > 8,000 |

**Insights**
- Most users fall into **Moderate** and **High** activity levels
- A notable segment remains **Low activity**, presenting engagement opportunities
- Step tracking is a strong behavioral anchor for users

---

### 2️⃣ Sleep Analysis
Metrics analyzed:
- Average sleep duration
- Time in bed
- Sleep efficiency gap (time in bed – time asleep)

**Insights**
- Users spend more time in bed than asleep
- Small gaps suggest generally efficient sleep for most users
- Larger gaps indicate potential sleep-quality issues
- Opportunity for sleep-focused features and nudges

---

### 3️⃣ Daily Activity Analysis
Average daily minutes by activity type:

| Activity Type | Avg Minutes/Day |
|--------------|----------------|
| Sedentary | ~1030 |
| Lightly Active | ~220 |
| Fairly Active | ~16 |
| Very Active | ~20 |

**Insights**
- Sedentary behavior dominates daily routines
- Light activity is common, but higher-intensity movement is rare
- Indicates opportunity for **behavioral nudges** and micro-activity campaigns

---

## 📈 Key Takeaways
- Users engage consistently with step and sleep tracking
- Sedentary behavior outweighs active movement
- Sleep efficiency varies across users
- Smart nudges and personalized insights could drive deeper engagement

---

## 💡 Marketing Recommendations
- Promote **short activity challenges** to reduce sedentary time
- Introduce **sleep efficiency insights** within the app
- Use step-based milestones for habit-building campaigns
- Segment users by activity level for personalized messaging

---

## 📎 How to Use This Project
1. Review the dashboard for a high-level overview
2. Read insights by analysis section
3. Apply findings to marketing or product strategy discussions
4. Extend analysis with newer or demographic-enriched datasets

---

## 📬 Contact
- **Email:** mednidalloucif@gmail.com  
- **GitHub:** https://github.com/LoucifNidal  
- **Kaggle:** https://www.kaggle.com/nidalloucif  
- **Portfolio:** https://loucifnidal.github.io  

---

© Loucif Mohamed Nidal — All Rights Reserved
