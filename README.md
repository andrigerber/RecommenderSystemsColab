# Improving Deezer’s Music Recommendation Engine

This repository presents our work on **Improving Deezer’s Music Recommendation Engine** for the DSG17 Online Phase. This project is a group work carried out at **HSLU (Hochschule Luzern)** by Gerber Andri, Del Conte Fabian, and Olympio Arnold. Our project delivers a complete, modular pipeline—from data exploration to advanced modeling—for predicting if a user will listen to a track for more than 30 seconds.

---

## Overview

The project is divided into three core notebooks:

1. **EDA.ipynb**  
   - **Purpose:** Conduct rigorous exploratory data analysis to assess data quality, detect outliers, and derive key temporal and behavioral features.
   - **Outcome:** A detailed data dictionary and insights that drive subsequent feature engineering.

2. **Preprocess_Feature_store.ipynb**  
   - **Purpose:** Transform raw data into a unified feature store using chunk-wise loading, timestamp conversion, outlier filtering, and engineered features (e.g., user behavior, time bins).
   - **Outcome:** Consistent, high-quality processed datasets for both training and testing.

3. **Specific_Preprocess_and_Modelling.ipynb**  
   - **Purpose:** Build and evaluate recommender models ranging from baseline methods (content-based, collaborative filtering, matrix factorization, PMF, RBM) to advanced approaches (Factorization Machines, NCF/NeuMF, GraphSAGE).
   - **Outcome:** Models optimized primarily for ROC AUC, with additional metrics (precision, recall, F1) to ensure robust performance.

---

## Key Insights

- **Feature Engineering:** Advanced preprocessing (time-based, behavioral, and cross features) is critical for model success.
- **Modeling Strategies:** Deep learning and graph-based methods (e.g., GraphSAGE) significantly outperform traditional baselines.
- **Evaluation:** ROC AUC is the primary metric, ensuring threshold-independent performance even with imbalanced data.
- **Scalability:** A modular pipeline allows for continuous updates and real-time integration in a production environment.

---

## How to Run

1. **EDA.ipynb:**  
   - Open the notebook (in Colab or JupyterLab), load your raw data, and perform initial exploration.

2. **Preprocess_Feature_store.ipynb:**  
   - Run the training and test pipelines to generate processed datasets with uniform features.

3. **Specific_Preprocess_and_Modelling.ipynb:**  
   - Load the processed data, select and tune models, and generate final predictions for evaluation or deployment.

---

## Final Thoughts

Our approach blends robust feature engineering with state-of-the-art modeling techniques to create a competitive recommendation engine. For detailed model configurations, evaluation metrics, and experimental insights, please refer to the full report in the Appendix.

Enjoy exploring and extending this pipeline!