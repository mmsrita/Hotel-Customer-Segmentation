# 🏨 Hotel Customer Segmentation (CRISP-DM) 

## 📌 Project Overview
In the hospitality sector, understanding customer behavior and preferences is key to effective marketing and revenue management. Traditional demographic segmentation often misses the nuances of guest behavior. 

Following the **CRISP-DM** methodology, this project leverages machine learning (*K-Means Clustering*) to build behavioral customer profiles. To address the geographical skew in the dataset (84.3% European guests), a **two-pronged clustering approach** was implemented to uncover distinct patterns for both European and Non-European markets without letting minority groups be overshadowed.

---

## 🔍 Key Exploratory Insights (EDA)
* **Booking Dynamics:** Demographic factors like age and continent are weak predictors of overall spending and frequency. Most guests book on short notice and stay for brief periods.
* **Special Requests:** The vast majority of guests do not make special requests, though *Middle-Aged Adults* and *Adults* show a higher tendency when requests are made.
* **Geographic Skew:** Europe accounts for **84.3%** of all customers. Non-European markets present different demographic balances (e.g., *Seniors* dominate in Oceania, while *Adults* lead in Africa).

---

## 🧩 Customer Segments & Profiles

### 🇪🇺 European Customers Model

| Cluster | Profile Name | Lead Time | Spending | Special Requests | Key Preferences |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Cluster 0** | 🛎️ Demanding, Comfort-Oriented | **High (~95 days)** | **Higher** | **Frequent** | **Luxury (>50%)** and **quiet environments** |
| **Cluster 1** | 🎒 Practical & Low-Demand | — | **Budget-conscious** | Low | **Cost-effectiveness** (neutral on luxury/quietness) |
| **Cluster 2** | 💎 Long-Term Loyalists | — | Moderate | Moderate | **100% luxury preference** & **longest loyalty** |

---

### 🌎 Non-European Customers Model

| Cluster | Profile Name | Lead Time | Spending | Special Requests | Key Preferences |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Cluster 0** | 🎒 Practical & Short-Notice | **Shortest (~75 days)** | Lower | Minimal | **Speed and economy** |
| **Cluster 1** | ⏳ Early Planners & Luxury Seekers | **Longest (~84 days)** | Slightly lower | Moderate | **100% luxury preference** |
| **Cluster 2** | 💎 High-Spenders & Tranquility Seekers | — | **Highest (Revenue/stay)** | **Highest** | **Quiet environments** and luxury |
