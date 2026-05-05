# Hotel-no-Show-Prediction
Predicting hotel no-shows using machine learning

📌 Project Title

Hotel No-Show Prediction & Revenue Optimization

📖 Overview

This project analyzes hotel booking data to identify patterns behind customer no-shows and builds a machine learning model to predict no-show probability.

The goal is to reduce revenue loss from unoccupied rooms and support data-driven operational decisions such as overbooking and targeted interventions.

🎯 Objectives
Perform exploratory data analysis (EDA) to uncover no-show patterns
Engineer meaningful features from booking data
Build and evaluate classification models
Optimize model performance based on business needs
Translate model outputs into actionable insights

📊 Dataset
~119,000 booking records
Features include:
booking details (branch, platform, room type)
customer attributes (country, first-time vs returning)
pricing and stay information

🔧 Data Cleaning & Preparation
Removed invalid / null rows
Converted data types (numeric, categorical)
Cleaned and transformed pricing data (multi-currency → SGD)
Engineered features:
length_of_stay
price_sgd
nightly_rate
expected_price_sgd
arrival_month_num

📈 Exploratory Data Analysis (EDA)

Key insights:

📍 Branch differences: No-show rates vary by location
💻 Platform effect: Booking source impacts reliability
👤 First-time customers: Higher likelihood of no-show
💰 Pricing behavior: Price influences commitment level
🏨 Stay length: Longer stays show different patterns

🤖 Machine Learning
Models Used:
K-Nearest Neighbors (baseline)
Random Forest (final model)
Final Model: Random Forest
Accuracy: 74%
No-show Recall: 61%
Precision (no-show): 66%

📊 Model Evaluation

Confusion Matrix:

[[12204  2829]
 [ 3429  5416]]

Interpretation:

Correctly identified 5,416 no-shows
Missed 3,429 no-shows
Improved detection compared to baseline model

💰 Business Impact
~1000 additional no-shows detected vs baseline
Estimated impact: ~$400,000 SGD revenue opportunity

⚖️ Trade-offs
Increased false positives (predicting no-show incorrectly)
Acceptable trade-off for improving detection of high-risk bookings

🚀 Business Recommendations
Implement risk-based overbooking strategy
Use model for customer risk scoring
Apply targeted interventions:
reminders
deposits
incentives

🧠 Key Takeaways
Model performance must align with business objectives, not just accuracy
Recall optimization is critical for minimizing revenue loss
Feature engineering significantly impacts model effectiveness

🛠️ Tech Stack
Python
pandas, numpy
matplotlib
scikit-learn

📁 Project Structure

├── data/
├── notebooks/
├── README.md

👤 Author

[Ng Yian Keong]
