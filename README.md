# Hotel Booking Cancellation Analysis

## Project Overview
This project aims to analyze hotel booking data to predict the likelihood of a customer canceling their booking. Using machine learning classification models, we will explore various factors such as the length of stay, room type, payment method, country of origin, and booking period that influence the cancellation decisions. The goal is to reduce the cancellation rate and optimize hotel operations by understanding customer behavior and improving the booking policies.

## Problem Statement
Hotel booking cancellations, especially close to the check-in date, can result in significant revenue losses and operational inefficiencies. To mitigate these effects, the hotel wants to predict the probability of booking cancellation and identify key factors that lead to such cancellations. By doing so, the hotel can:

- Take preventive actions like adjusting their cancellation policies or providing special offers.
- Maximize room allocation efficiency by predicting and minimizing last-minute cancellations.

## Business Objectives
1. **Predict whether a customer will cancel their booking** based on historical booking data.
2. **Identify the key variables** that influence booking cancellation, such as customer type, deposite method, and parking space.
3. **Reduce cancellation rates** by using insights from customer behavior and improving strategies like special offers or cancellation policies.

## Data
- The dataset consists of various features related to hotel bookings, including customer type, booking details, and room type.
- The dataset contains categorical variables (nominal, binary), with some having high cardinality.
- **Note**: The dataset is imbalanced, meaning that the majority of bookings are not canceled.

You can find the dataset here:(https://drive.google.com/file/d/1eeXOEY5B_zfSNhWeDDqPWCo9hAyDRAbc/view?usp=drive_link).

### Data Features
- **Customer Information**: Country, deposite method, etc.
- **Booking Details**: Room type, Waiting list period, customer type, etc.
- **Target Variable**: 
  - `0`: Booking not canceled
  - `1`: Booking canceled

## Analytical Approach
### Step 1: Data Preprocessing
- **Handle Missing Values**: Identify and handling missing data.
- **Feature Engineering**: Transform categorical variables into numerical formats for modeling.
- **Class Balancing**: Since the dataset is imbalanced, techniques like oversampling or undersampling may be applied.
  
### Step 2: Exploratory Data Analysis (EDA)
- Analyze the distribution of key variables such as room type, country, and waiting list period.
- Identify correlations between variables and cancellation rates.

### Step 3: Model Building
- **Classification Models**: Various machine learning classification algorithms will be used, such as:
  - Logistic Regression
  - Decision Trees
  - Random Forest
  - Gradient Boosting
  - CatBoost
  - Support Vector Machines (SVM)
- **Class Imbalance Handling**: Given the class imbalance, techniques like SMOTE (Synthetic Minority Over-sampling Technique) or class weights may be applied.

### Step 4: Model Evaluation
- **Primary Metric**: F1 Score to balance precision and recall.
- **Error Analysis**:
  - **Type 1 Error (False Positive)**: The model predicts a cancellation that doesn’t happen. This could result in unnecessary resources being allocated for offers or promotions.
  - **Type 2 Error (False Negative)**: The model fails to predict a cancellation that happens, resulting in a loss of revenue as the room remains unallocated.
- **Other Metrics**: Precision, Recall, f1 Score.

## Results
- **Key Variables**: Identify the most important factors influencing cancellations, such as room type, Waiting list period, and deposite method.
- **Model Performance**: The F1 Score is used to evaluate the effectiveness of the models.
  
## Conclusion
This analysis helps the hotel to:
1. Better predict which bookings are likely to be canceled.
2. Take preventive action to reduce cancellations, such as adjusting cancellation policies or offering special discounts for bookings at high risk of cancellation.
3. Improve overall customer satisfaction and resource allocation.

## Future Improvements
- **Fine-Tuning**: Further tuning of hyperparameters can improve model accuracy.
- **Feature Engineering**: Additional features like seasonal data or customer loyalty could enhance the predictions.
- **Real-Time Predictions**: Integrating this model into the hotel booking system for real-time predictions can further optimize operations.

## Setup & Requirements

### Dependencies
- Python 3.x
- pandas
- scikit-learn
- numpy
- matplotlib
- seaborn

### Instructions to Run
1. Clone this repository:
    ```bash
    git clone https://github.com/nurilmalani/Capstone_3_Hotel-Booking-Demand
    ```
2. Run the analysis notebook:
    ```bash
    jupyter notebook Capstone_3_Nur Ilmalani.ipynb
    ```

## Authors
- **Nur Ilmalani** (Data enthusiast, Hotel Cancellation Prediction)

