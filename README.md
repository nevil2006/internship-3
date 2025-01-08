 User Churn Prediction Project

 Project Overview
This project is focused on building a **User Churn Prediction** model for an e-commerce platform. The goal of the project is to predict which users are likely to churn (i.e., stop using the platform) based on their behavior. The predictions can help businesses implement retention strategies to retain valuable customers.

 Problem Statement
The problem is to identify which users are at risk of leaving the platform based on their historical interaction data (views, carts, and purchases). The goal is to build a model that predicts user churn and provides business insights on retention strategies.

 Dataset
The dataset used in this project is the `events.csv` file, which contains user interactions with the e-commerce platform. The file includes the following columns:
- `user_id`: Unique identifier for each user
- `event_time`: Timestamp of the event
- `event_type`: Type of event (e.g., view, add_to_cart, purchase)
- `product_id`: ID of the product interacted with
- `price`: Price of the product

Features Engineered
- Recency: Time since the last purchase or activity
- Frequency: Number of sessions or purchases within a given timeframe
- Monetary: Total amount spent by the user
- Session-based metrics: Average session duration, session count, and bounce rate
- Behavioral patterns: View-to-cart and cart-to-purchase ratios

Approach
1. Data Preprocessing:
   - Handle missing values and duplicates.
   - Parse `event_time` to datetime format.
   - Encode categorical variables where necessary.

2. Feature Engineering:
   - Calculate recency, frequency, and monetary values.
   - Extract session-based metrics and behavioral patterns.

3. Modeling:
   - Split the dataset into training and testing sets.
   - Train multiple models, including Logistic Regression, Random Forest, and XGBoost.
   - Use Random Forest for final prediction due to its handling of non-linear relationships and feature importance.

4. Evaluation:
   - Evaluate the models using metrics like AUC, precision, recall, and F1-score.
   - Focus on F1-score as it balances precision and recall.

5. Model Explainability:
   - Use SHAP (SHapley Additive exPlanations) to explain the model's decisions.

## Installation

To run this project, clone the repository and install the required dependencies:

```bash

