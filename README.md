
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
- [Dashboard / Visuals](#dashboard--visuals)
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
- **Size**: ~90+ launches
- **Time Period**: 2010–2020
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
| Evaluation       | Accuracy, F1, LogLoss           |
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
- **Random Forest**

Metrics:
- Accuracy
- F1-Score
- Jaccard Index
- Log Loss (for probabilistic predictions)

---

## 📈 Results & Insights

| **Model**              | **Accuracy** | **F1 Score** | **Log Loss** |
|------------------------|--------------|--------------|--------------|
| Logistic Regression    | 83%          | 0.83         | 0.36         |
| Decision Tree          | 85%          | 0.85         | —            |
| Random Forest          | 87%          | 0.86         | —            |

- **Insight**: Random Forest performed best overall, showing the importance of ensemble learning.
- **Business Value**: Predictive models can simulate future outcomes and reduce risk in launch planning.

---

## 📊 Dashboard / Visuals

- Folium map showing launch sites and outcomes.
- Interactive EDA charts embedded in the notebook.
- You can export the visuals for presentation or integrate into a Power BI dashboard.

---

## 🧾 Conclusion

- **What worked**: Our experiments showed that Random Forest provided the best predictive performance.
- **What could improve**: Incorporating additional features like weather conditions and real-time telemetry.
- **Business value**: Predictive modelling can aid strategic planning, budgeting, and competitor benchmarking in the aerospace industry.

---

## 👨‍💻 Author

**Olabanji [Olaniyan]**  
Data Scientist  
📫 [LinkedIn](https://www.linkedin.com/in/olabanji-olaniyan-59a6b0198/) | [Portfolio](banjiola.github.io/Olabanji-Olaniyan/)
