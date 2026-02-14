Give-Life-Predict-Blood-Donations

🚀 Overview The Give Life: Predict Blood Donations project aims to forecast blood donations using machine learning. Blood is a precious gift, and predicting donor behavior helps blood banks plan drives, maintain supply, and ultimately save more lives.

This project uses historical donation data to predict whether a donor will give blood in the next donation cycle, applying a Logistic Regression model for interpretable and effective predictions.

🧠 The Problem Blood donation demand fluctuates throughout the year. During holidays or busy periods, donations drop significantly (for example, 27,000 fewer donations observed by Red Cross in Jan 2019). Blood banks need accurate predictions to plan campaigns and ensure enough supply.

Traditional methods often rely on manual tracking, which is slow and inefficient. Machine learning can identify patterns in donor history and improve forecasting.

💡 The Solution This project uses Logistic Regression to predict blood donations based on donor history. Key steps include:

Data Loading & Inspection: Understanding the structure and distribution of donor data.
Target Creation: Defining whether a donor gave blood in a specific period.
Train/Test Split: Stratifying to maintain target distribution.
Feature Normalization: Log-transforming high-variance features (for example, total blood donated).
Model Training & Evaluation: Training Logistic Regression and evaluating performance using AUC.
🛠️ Tech Stack

Language: Python 3.11+
Libraries: pandas, numpy, scikit-learn, Jupyter Notebook
Tools: Git & GitHub for version control
📊 Dataset Details

Source: UCI Machine Learning Repository
Size: 748 donor records
Columns:
Column	Description
R	Recency – months since last donation
F	Frequency – total number of donations
M	Monetary – total blood donated (c.c.)
T	Time – months since first donation
target	Whether donor gave blood in March 2007 (0 = No, 1 = Yes)
📈 Key Results

Model: Logistic Regression
Evaluation Metric: AUC
AUC Score: ~0.789 after log-normalization of high-variance feature.
Feature contributions can be analyzed using model coefficients to understand the impact of each factor on donation likelihood.
🏁 Future Scope

Use automated ML tools (like TPOT or Auto-sklearn) for pipeline optimization.
Explore ensemble methods to improve prediction accuracy.
Integrate real-time donor data for dynamic forecasting.
Develop a dashboard for blood banks to visualize predicted donation patterns.
⚙️ How to Run Locally

Prerequisites:

Install Python 3.11+
Install Jupyter Notebook (optional, for interactive exploration)
Installation:

pip install pandas numpy scikit-learn
