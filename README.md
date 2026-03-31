# SRIS — Smart Restaurant Intelligence System

> **Cognifyz Technologies | Machine Learning Internship Project**  
> A complete ML suite for restaurant data analysis, rating prediction, recommendation, cuisine classification, and location-based insights.

---

## Project Overview

SRIS (Smart Restaurant Intelligence System) is a machine learning project developed as part of the **Cognifyz Technologies Machine Learning Internship Program**. It brings together four powerful ML modules — each targeting a distinct analytical challenge in the restaurant domain — using a unified dataset of restaurant records containing features like cuisine type, location coordinates, price range, votes, and aggregate ratings.

The project demonstrates the full ML pipeline: data preprocessing, feature engineering, model training, evaluation, and insight extraction.

---

## Modules

This project implements **3 out of 4** available tasks from the internship program:

---

### Task 1 — Restaurant Rating Prediction

**Objective:** Build a regression model that predicts the aggregate rating of a restaurant based on its features.

**Approach:**
- Handled missing values and encoded categorical variables (e.g., cuisine type, city)
- Split data into training and testing sets
- Trained regression models including **Linear Regression** and **Decision Tree Regressor**
- Evaluated performance using **Mean Squared Error (MSE)** and **R² Score**
- Analyzed feature importances to identify the most influential predictors of restaurant ratings

**Key Insight:** Features like price range, number of votes, and whether online delivery is available tend to be strong predictors of aggregate ratings.

---

### Task 2 — Restaurant Recommendation System

**Objective:** Create a content-based recommendation engine that suggests restaurants matching user preferences.

**Approach:**
- Preprocessed dataset by handling nulls and encoding categorical variables
- Defined recommendation criteria: **cuisine preference** and **price range**
- Built a **content-based filtering** system using cosine similarity on feature vectors
- Tested the system with sample user preference profiles and evaluated recommendation quality

**Key Insight:** Content-based filtering works well for restaurant recommendations since user preferences (e.g., "I like Italian, mid-range price") map cleanly to restaurant attributes.

---

### Task 3 — Cuisine Classification

**Objective:** Train a classification model to categorize restaurants by their cuisine type.

**Approach:**
- Preprocessed data and encoded categorical variables
- Split into train/test sets with stratification across cuisine classes
- Trained classifiers including **Logistic Regression** and **Random Forest**
- Evaluated using **Accuracy**, **Precision**, **Recall**, and **F1-Score**
- Analyzed per-cuisine performance to identify class imbalance or bias issues

**Key Insight:** Some cuisine types are underrepresented in the dataset, which creates class imbalance — addressed through analysis and noted as a limitation.

---

### Task 4 — Location-Based Analysis *(not included in this submission)*

---

## Repository Structure

```
SRIS_Cognify/
│
├── Task1_Rating_Prediction/
│   ├── rating_prediction.ipynb       # Main notebook
│   └── README.md                     # Task-specific notes
│
├── Task2_Recommendation_System/
│   ├── recommendation_system.ipynb
│   └── README.md
│
├── Task3_Cuisine_Classification/
│   ├── cuisine_classification.ipynb
│   └── README.md
│
├── data/
│   └── restaurant_dataset.csv        # Source dataset
│
└── README.md                         # This file
```

---

## Tech Stack

| Category | Tools / Libraries |
|---|---|
| Language | Python 3.x |
| Data Handling | `pandas`, `numpy` |
| Visualization | `matplotlib`, `seaborn` |
| Machine Learning | `scikit-learn` |
| Similarity (Task 2) | `sklearn.metrics.pairwise` |
| Notebooks | Jupyter Notebook |

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/MercuryConnor/SRIS_Cognify.git
cd SRIS_Cognify
```

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 3. Launch the notebooks

```bash
jupyter notebook
```

Navigate to any task folder and open the `.ipynb` file to explore the full pipeline.

---

## 📊 Results Summary

| Task | Model Used | Key Metric | Score |
|---|---|---|---|
| Rating Prediction | Decision Tree Regressor | R² Score | *see notebook* |
| Recommendation | Cosine Similarity | Qualitative evaluation |
| Cuisine Classification | Random Forest | Accuracy | *see notebook* |

> Exact scores depend on the dataset split. Refer to individual notebooks for full evaluation outputs.

---

## 🏢 About Cognifyz Technologies

**Cognifyz Technologies** is a leading data science and AI company that delivers cutting-edge solutions in machine learning, artificial intelligence, and data analytics. They also offer training programs to develop practical skills in these areas.

- 🌐 [www.cognifyz.com](https://www.cognifyz.com)
- 📧 contact@cognifyz.com
- 💼 [LinkedIn: @cognifyz-Technologies](https://linkedin.com/company/cognifyz-Technologies)
- 📸 Instagram: [@cognifyz_tech](https://instagram.com/cognifyz_tech)

---

## 👤 Author

**MercuryConnor**  
Machine Learning Intern — Cognifyz Technologies  
[GitHub](https://github.com/MercuryConnor)

---

> *"Where Data Meets Intelligence"* — Cognifyz Technologies
