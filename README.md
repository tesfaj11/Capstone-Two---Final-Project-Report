# Capstone-Two---Final-Project-Report
# California Housing Prices Prediction

This project analyzes housing data from California to build a machine learning model that predicts **median house prices** based on location, population density, and socio-economic factors.

---

## Project Overview

**Goal:** Predict the *Median House Value* in California districts using regression models.  
**Dataset:** [California Housing Dataset (from Scikit-learn)](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_california_housing.html)  
**Techniques:** Data Cleaning, EDA, Linear Regression, Random Forest, RMSE/R² Evaluation

---

## Project Structure

```bash
california_housing_project/
│
├── 1_importing_data.ipynb           # Load & explore data
├── 2_data_cleaning.ipynb            # Clean & prepare dataset
├── 3_eda.ipynb                      # Visualize and analyze trends
├── 4_modeling.ipynb                 # Train & evaluate regression models
├── model_metrics.txt                # Summary of model performance
├── final_report.pdf                 # Full project report (for stakeholders)
└── README.md                        # This file
Exploratory Data Analysis
Distribution of MedianHouseValue is slightly right-skewed

MedInc (Median Income) has strong positive correlation with house price

Population and room counts show nonlinear trends

Correlation Heatmap:
 Model Comparison
Model	R² Score	RMSE
Linear Regression	0.58	~0.73
Random Forest	0.81	~0.47

Random Forest outperformed Linear Regression significantly.

Top Features Influencing Price
MedInc – Median Income

AveRooms – Average number of rooms

HouseAge – Age of the housing

AveOccup – Average occupancy

Latitude & Longitude – Location effects

Final Recommendations
Use Random Forest for production if speed is not a concern.

Consider collecting more detailed location features (zip code, city).

Normalize high-income outliers to improve predictions.

Tools Used
Python (Pandas, NumPy, Scikit-Learn)

Jupyter Notebook

Seaborn & Matplotlib

Git/GitHub

License
This project is for educational use as part of Springboard’s Data Science Career Track Capstone 2.
