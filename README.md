🚦 Accident Duration Prediction Project
📘 Project Overview

Guiding Questions

🎯 What were we trying to find out?
We aimed to predict the duration of traffic accidents using traffic, road, and weather data. Main question:
“Given accident and environmental conditions, how long will an accident last?”

🧠 What did we already know?
Factors such as road type, weather, traffic control, and time of day influence accident duration. Historical accident datasets provided these features along with recorded durations.

🏆 What did we aim to achieve?
We sought to build predictive models with low RMSE and high R² to accurately estimate accident duration, aiding traffic management and emergency response.

⚙️ What factors affected our results?

Temporal: Hour of day, day of week, month

Weather: Temperature, humidity

Road: Type, complexity, traffic controls

Accident specifics: Severity, number of vehicles

💡 Was there something new we could use?
We applied feature engineering (interactions, road complexity, temporal features) and ensemble models (Random Forest, Gradient Boosting, XGBoost) to improve predictive accuracy. An automated preprocessing and evaluation pipeline was implemented.

🛠 Project Stages
1️⃣ Data Preparation

What we did:

Loaded the dataset and inspected rows, columns, missing values, and data types.

Converted object types to appropriate types (category/datetime).

Removed punctuation and narrowed categories for optimal use.

Extracted year/month/day/hour/minute/second from start and end times.

Saved the cleaned dataset to a flatfile for downstream analysis.

2️⃣ Exploratory Data Analysis (EDA)

Summarized the dataset: data types, min/max values, missing values, unique counts.

Saved an overall summary to a Data Protocol Excel file.

Generated automated EDA reports via AutoViz.

Applied statistical methods and visualizations to identify patterns, trends, and potential issues.

3️⃣ Data Cleansing, Outliers, and Normalization

Detected outliers and handled them by capping or removing.

Normalized variables to prepare them for modeling.

3.2️⃣ Data Imputation & Encoding

Imputed missing values using median or mode.

Encoded categorical variables using one-hot or dummy encoding for model readiness.

4️⃣ Feature Engineering & Feature Selection

Added features capturing temporal, weather, and road interactions.

Applied feature selection to identify the most predictive variables.

5️⃣ Model Training & Fine-Tuning

Trained multiple regression models: Linear Regression, Decision Tree, Random Forest, AdaBoost, Gradient Boosting, XGBoost.

Fine-tuned models using GridSearchCV for optimal hyperparameters.

Evaluated performance using RMSE, MAE, and R².

Analyzed feature importance to interpret the models.

🚀 Quick Start

Clone the repository

git clone https://github.com/Roza-AS/ML_project.git
cd ML_project


Install dependencies

pip install -r requirements.txt


Run Jupyter Notebook

jupyter notebook


Notebooks were executed in this order:

Data Preparation

EDA

Data Cleansing

Data Cleansing_2 (Imputation & Encoding)

Feature Engineering & Model Training

📊 Deployment and Beneficiaries

💻 How the ML system can be deployed:
The pipeline can be integrated into traffic management platforms to provide real-time accident duration estimates, enabling efficient response planning. Preprocessing and prediction steps are automated.

👥 Who benefits:

Traffic management centers

Emergency response teams

City planners

Deployment improves decision-making, reduces congestion, and optimizes resource allocation.
