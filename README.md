# DA-PROJECT1

# Data Analytics – Machine Learning Project Plan

## 1. Course Name

**Data Analytics – Machine Learning**

---

## 2. Team Information

**Team Name:** RAZAR

| Full Name               | Student ID | Group  | Role                | Phone             |
| ----------------------- | ---------- | ------ | ------------------- | ----------------- |
| **Ra'no Botirova**      |            | I24B   | Leader              | +998-33-004-05-45 |
| **Zarifa Tursunova**    |            | I24B   | Data Analyst        |                   |


---

## 3. Project Title

**Travel Locations Review Analysis and Insight Mining**

---

## 4. Dataset Information

* **Dataset Title:** Travel Reviews Dataset
* **Source Website / URL:** https://archive.ics.uci.edu/dataset/484/travel+reviews
* **Description:**
  The dataset contains average traveler ratings for different destination categories across East Asia (e.g., museums, beaches, restaurants). Each review rating is mapped from *Terrible (0)* to *Excellent (4)*. 
* **Why Selected:**
  → Real-world tourism review dataset suitable for analysis tasks such as clustering, classification, and exploratory data analysis. 
* **Size of Dataset:**
  ~980 rows (users) × 10 feature columns 

---

## 5. Project Objectives

* Analyse travel review ratings to understand user satisfaction patterns.
* Identify which categories (e.g., beaches, restaurants) are highly rated.
* Perform cluster analysis to find groups of similar traveler preferences.
* Extract actionable insights for tourism marketing or service improvement.

---

## 6. Data Preparation (Pandas)

```python
import pandas as pd

df = pd.read_csv("tripadvisor_review.csv")
df.head()
df.isnull().sum()
df = df.drop_duplicates()
```

---

## 7. Analysis Tasks

* **Descriptive statistics:**

  ```python
  df.describe()
  ```

* **Average rating per category:**

  ```python
  df.mean()
  ```

* **Grouping and sorting:**

  ```python
  df.sort_values(by='Category 4', ascending=False)
  ```

* **Clustering / segmentation:**
  *Use K-Means or hierarchical clustering to find patterns.*

---

## 8. Key Findings and Insights

* Identifying which attraction types tend to get higher ratings.
* Determining if certain categories correlate with each other (e.g., resorts & beaches).
* Clusters of users with similar preferences for targeted recommendations.

---

## 9. Project Timeline (5 Weeks)

| Week   | Activities                |
| ------ | ------------------------- |
| Week 1 | Dataset search & planning |
| Week 2 | Data cleaning & prep      |
| Week 3 | Data analysis & EDA       |
| Week 4 | Clustering / ML tasks     |
| Week 5 | Report & presentation     |

---

## 10. Outcome of the Project

* Gaining experience in data cleaning & Pandas operations
* Learning how to interpret multivariate review data
* Applying clustering or classification techniques

---

## 11. Conclusion

This project provides meaningful insights into how travelers rate different destination categories. It supports data-driven decisions for tourism service improvements.

---

## 12. References

* UCI Travel Reviews Dataset ([archive.ics.uci.edu][1])
* Pandas Documentation
* Scikit-learn Documentation

---

## 13. Appendix

* Code snippets
* Charts / graphs
* Clustering results

---
