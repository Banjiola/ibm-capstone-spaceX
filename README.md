
# 💼 **SpaceX Falcon 9 First Stage Landing Prediction**

> *This project utilises machine learning to predict the successful landing of SpaceX Falcon 9 rockets to assess potential cost savings.*

---

## 📌 Table of Contents
- [Overview](#overview)
- [Business Objective](#business-objective)
- [Dataset](#dataset)
- [Tools & Techniques](#tools--techniques)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Results & Insights](#results--insights)
- [Conclusion](#conclusion)
- [Author](#author)

---

## 🧩 Overview

This project analyzes historical SpaceX launch data to build a machine learning model that predicts whether the **first stage of a Falcon 9 rocket will land successfully**. 

- **Objective**: Build a predictive model using logistic regression, SVM, decision trees, and ensemble methods.
- **Impact**: Helps evaluate potential cost savings from successful booster landings — a major differentiator in the commercial space industry.

---

## 🎯 Business Objective

> Can we predict if a Falcon 9 rocket’s first stage will land successfully?

- **Target users**: Aerospace analysts, budget planners, and competitive space contractors.
- **Value**: Enables competitors to estimate cost viability and plan alternative launch strategies.

---

## 📊 Dataset

- **Source**: SpaceX Launch data (via API and web scraping)
- **Key Variables**:
  - `FlightNumber`, `PayloadMass`, `Orbit`, `LaunchSite`, `LandingOutcome`, `BoosterVersion`
  - Target: `Class` (1 = Landed, 0 = Not landed)

---

## 🛠️ Tools & Techniques

| **Category**     | **Tools**                                      |
|------------------|------------------------------------------------|
| Language         | Python                                         |
| Data Handling    | `pandas`, `numpy`, `requests`, `beautifulsoup4`|
| Visualization    | `matplotlib`, `seaborn`, `plotly`, `folium`    |
| Modeling         | `scikit-learn`                                 |
| Evaluation       | Accuracy           |
| Notebook Platform| Jupyter / IBM Skills Network                   |

---

## 🔎 Exploratory Data Analysis

Performed exploratory analysis on:
- Launch success by site
- Payload vs. success correlation
- Flight number trends
- Visualizations:
  - Pie charts, scatter plots, and world maps using `folium` for site mapping
  - Correlation heatmaps

---

## 🏗️ Feature Engineering

- **Categorical encoding**: One-hot encoding for launch sites and booster versions
- **Scaling**: StandardScaler on numerical features
- **Feature selection**: Reduced highly correlated or low-impact variables

---

## 🤖 Modeling

Models evaluated:
- **Logistic Regression**
- **Support Vector Machines**
- **Decision Tree**
- **K-Nearest Neighbor**

Metrics:
- Accuracy
---

## 📈 Results & Insights

| **Model**              | **Accuracy** | 
|------------------------|--------------|
| Logistic Regression    | 83%          |
| Decision Tree          | 83%           |
| Random Forest          | 83%          |
|K Nearest Neighbor      | 83%          |

- **Business Value**: Predictive models can simulate future outcomes and reduce risk in launch planning.

---

## 🧾 Conclusion

- **What worked**: Our experiments showed that all models acheived similar predictive performance.
- **What could improve**: Incorporating additional features like weather conditions and real-time telemetry.
- **Business value**: Predictive modelling can aid strategic planning, budgeting, and competitor benchmarking in the aerospace industry.

---

## 👨‍💻 Author

**Olabanji [Olaniyan]**  
Data Scientist  
📫 [LinkedIn](https://www.linkedin.com/in/olabanji-olaniyan-59a6b0198/) | [Portfolio](banjiola.github.io/Olabanji-Olaniyan/)
