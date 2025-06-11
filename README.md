# 🏠 Airbnb Host Retention Strategy – Data & AI Driven Marketing

This project applies machine learning and optimization to predict Airbnb host churn and design a targeted retention strategy. By allocating $1,000 incentives only where they yield positive ROI, the solution maximizes net profit and retains high-value hosts.

---

## 📌 Problem Statement

Airbnb faces revenue risk from losing hosts—especially high earners. With limited resources, the challenge is to **predict host churn** and identify which hosts should receive a $1,000 retention incentive to maximize future profit.

---

## 🎯 Objective

Build a data-driven framework that predicts churn, segments hosts by value, and **optimally allocates retention gifts** to maximize net profit while minimizing unnecessary spend.

---

## 🗂️ Dataset Overview

- 🏡 Host-level booking and revenue data (multi-year)
- 🌎 Geographic data (latitude/longitude, city)
- 📊 Behavioral features (annual revenue, churn label, booking frequency, etc.)

---

## 🧹 Data Preprocessing

- Summary statistics, missing value treatment
- Outlier handling via statistical methods
- Feature engineering: spatial clusters (K-Means), revenue segments, dummy variables

---

## 🧠 Modeling & Retention Logic

- Model training: Logistic Regression, Decision Tree, Random Forest, Gradient Boosted Trees (with GridSearch CV)
- Final model: Random Forest (81% test ROC)
- Retention scoring: Calculate expected profit gain from retaining each host  
  - Allocate $1,000 retention gift only where:  
    *Expected revenue gain from retention > $1,000 incentive cost*

---

## 📈 Results

| Metric                 | Value      |
|------------------------|------------|
| Test ROC (Random Forest) | **0.81**  |
| Hosts Targeted           | 334       |
| Total Spend              | $334,000  |
| Cohort Competition Rank  | **1st**   |

- The targeted retention approach **maximized profit** and topped the class leaderboard.

---

## 🧪 Libraries Used

- `pandas`, `numpy`, `scikit-learn`
- `matplotlib`, `seaborn`
- `scipy`

---

## 🧠 Key Learnings

- Combining **churn modeling** and **expected revenue optimization** can maximize marketing ROI.
- **Clustering** and segmentation enable more nuanced retention targeting.
- Model interpretability and business logic alignment are critical for adoption.

---

## 🚀 Future Work

- Incorporate **lifetime value prediction** for more strategic targeting
- Experiment with **uplift modeling** to directly estimate treatment effects
- Deploy as a dashboard for Airbnb marketing teams

---

## 🤝 Acknowledgements

- Airbnb anonymized host data (academic use)
- Scikit-learn for modeling utilities

---

## 🏅 Example Use Case

> Coming soon: Interactive dashboard showing selected hosts for retention and projected ROI.
