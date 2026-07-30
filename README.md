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
Using the **Elbow Method** and **Silhouette Score**, 3 optimal clusters were identified:

* 🛎️ **Cluster 0 – Demanding, Comfort-Oriented:** High lead times (~95 days), higher spending, frequent special requests, and high demand for luxury (>50%) and quiet environments.
* 🎒 **Cluster 1 – Practical & Low-Demand:** Budget-conscious, low special requests, neutral on luxury and quietness. Focuses on cost-effectiveness.
* 💎 **Cluster 2 – Long-Term Loyalists:** Longest customer loyalty period, moderate requests, 100% preference for luxury, average spending.

### 🌎 Non-European Customers Model
Similarly validated using Silhouette Analysis, yielding 3 distinct international segments:

* 🎒 **Cluster 0 – Practical & Short-Notice:** Shortest lead times (~75 days), lower spending, minimal requests. Values speed and economy.
* ⏳ **Cluster 1 – Early Planners & Luxury Seekers:** Longest lead time (~84 days), 100% preference for luxury services, moderate requests, slightly lower spending.
* 💎 **Cluster 2 – High-Spenders & Tranquility Seekers:** Highest revenue per stay and highest number of special requests. Strong preference for quiet environments and luxury.

---

## 💡 Strategic Business Recommendations

### 🇪🇺 European Market Strategies
| Segment | Recommended Action |
| :--- | :--- |
| **Cluster 0 (Demanding & Comfort-Oriented)** | Target with premium room upgrades, quiet-zone guarantees, personalized stay packages, and high-margin add-ons (e.g., spa, private dining). |
| **Cluster 1 (Practical & Low-Demand)** | Focus on conversion via competitive pricing, functional package deals, and streamlined digital check-in processes. |
| **Cluster 2 (Long-Term Loyalists)** | Enroll in exclusive VIP loyalty tiers, offer early-bird perks, and maintain retention through personalized anniversary or return-stay offers. |

### 🌎 Non-European Market Strategies
| Segment | Recommended Action |
| :--- | :--- |
| **Cluster 0 (Practical & Short-Notice)** | Capture last-minute bookings via targeted OTA ads, mobile booking discounts, and fast-track booking options. |
| **Cluster 1 (Early Planners & Luxury Seekers)** | Promote long-lead booking packages with included luxury amenities, airport transfers, and premium service guarantees. |
| **Cluster 2 (High-Spenders & Tranquility Seekers)** | Offer bespoke luxury suites, tailored concierge services, and noise-isolated rooms to maximize revenue per stay. |
