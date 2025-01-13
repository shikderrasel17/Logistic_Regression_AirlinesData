
# Logistic Regression_AirlinesData

This project focuses on building a logistic regression model to analyze and predict customer satisfaction based on various features from an airline dataset. The dataset contains information about customer demographics, flight details, and satisfaction levels, which are used to train the model.

## Model Details

- **Model Type**: Logistic Regression
- **Library Used**: scikit-learn
- **Primary Objective**: To predict customer satisfaction based on various features of the flight experience.

## Intended Use

This model is intended for:

- Understanding the key factors influencing customer satisfaction.
- Helping airlines improve their services by identifying areas that impact customer satisfaction the most.

## Data Source(s)

- **Dataset**: Invistico_Airline dataset
- **Source**: Provided during the AI/ML Bootcamp.
- **Features Included**:
  - Customer demographics (Gender, Age, Customer Type)
  - Flight details (Type of Travel, Class, Flight Distance)
  - Service ratings (Seat comfort, Food and drink, Inflight entertainment, etc.)
  - Delays (Departure Delay, Arrival Delay)

## Dataset Sample

| satisfaction | Gender | Customer Type | Age | Type of Travel | Class | Flight Distance | Seat comfort | Departure/Arrival time convenient | Food and drink | ... |
|--------------|--------|---------------|-----|----------------|-------|-----------------|--------------|-----------------------------------|----------------|-----|
| satisfied    | Female | Loyal Customer | 65  | Personal Travel | Eco   | 265             | 0            | 0                                 | 0              | ... |
| satisfied    | Male   | Loyal Customer | 47  | Personal Travel | Business | 2464         | 0            | 0                                 | 0              | ... |
| satisfied    | Female | Loyal Customer | 15  | Personal Travel | Eco   | 2138           | 0            | 0                                 | 0              | ... |
| satisfied    | Female | Loyal Customer | 60  | Personal Travel | Eco   | 623            | 0            | 0                                 | 0              | ... |
| satisfied    | Female | Loyal Customer | 70  | Personal Travel | Eco   | 354            | 0            | 0                                 | 0              | ... |

## Training Data

- **Size**: Split into training and testing datasets.
- **Preprocessing**: Handled missing values using iterative imputation. Categorical features were label-encoded.

## Test Data

- **Size**: The dataset was split into training (80%) and testing (20%) sets.
- **Purpose**: To evaluate the model's performance.

## Parameters

- **Regularization**: L2 (default in Logistic Regression)
- **Solver**: liblinear

## Feature Importance

Feature importance is derived from the coefficients of the logistic regression model. Key features impacting customer satisfaction include:

- **Flight Distance**
- **Type of Travel**
- **Class**
- **Onboard Service**
- **Inflight Entertainment**

## Metrics

- **Accuracy**: Evaluates how often the model predicts correctly.
- **Confusion Matrix**: To assess the model's performance in terms of True Positives, True Negatives, False Positives, and False Negatives.
- **Classification Report**: Includes precision, recall, F1-score for both classes (satisfied, not satisfied).

## Additional Information

### Dependencies

- Python 3.x
- pandas
- scikit-learn

### Installation

Clone the repository and install the required libraries:

```bash
git clone https://github.com/shikderrasel17/Logistic_Regression_AirlinesData.git
cd Logistic_Regression_AirlinesData
pip install -r requirements.txt
