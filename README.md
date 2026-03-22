# CO2 Emission Prediction Using Linear Regression

This project uses **Linear Regression** to predict **vehicle CO2 emissions (g/km)** based on numerical vehicle features such as engine size, cylinders, and fuel consumption. The dataset used is the **CO2 Emissions in Canada** dataset.

## Project Overview

The goal of this project is to analyze the relationship between vehicle characteristics and CO2 emissions, then build a machine learning model that can estimate emissions for unseen data.

The project includes:

- Data loading and preprocessing
- Exploratory Data Analysis (EDA)
- Distribution analysis of numerical features
- Visualization of categorical and numerical variables
- Correlation analysis
- Linear Regression model training
- Model evaluation using MSE, RMSE, and R² score

## Dataset

The dataset contains information about vehicles in Canada, including:

- **Engine Size (L)**
- **Cylinders**
- **Fuel Consumption City (L/100 km)**
- **Fuel Consumption Hwy (L/100 km)**
- **Fuel Consumption Comb (L/100 km)**
- **Fuel Consumption Comb (mpg)**
- **CO2 Emissions (g/km)**

Target variable:

- **CO2 Emissions (g/km)**

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## Workflow

### 1. Data Loading
The dataset is loaded using Pandas and inspected to understand its structure.

### 2. Exploratory Data Analysis
Basic statistical summaries are generated for the numerical features and target variable.

### 3. Data Visualization
The project visualizes:

- Histogram and boxplot of CO2 emissions
- Distribution of numerical features
- Frequency distribution of categorical features
- Scatter plots to study correlation between numerical features and CO2 emissions

### 4. Feature Selection
The model uses the following numerical input features:

- Engine Size (L)
- Cylinders
- Fuel Consumption City (L/100 km)
- Fuel Consumption Hwy (L/100 km)
- Fuel Consumption Comb (L/100 km)
- Fuel Consumption Comb (mpg)

### 5. Model Training
The dataset is split into:

- **70% training data**
- **30% testing data**

A **Linear Regression** model is then trained using Scikit-learn.

### 6. Prediction and Evaluation
The trained model is evaluated on the test set using:

- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**
- **R² Score**

## Results

Model performance achieved in this project:

| Metric | Score |
|--------|-------|
| MSE    | 359.04 |
| RMSE   | 18.95  |
| R²     | 0.894  |

These results indicate that the model explains about **89.4% of the variance** in CO2 emissions, showing strong predictive performance.

## Key Insights

- Fuel consumption features show a strong relationship with CO2 emissions.
- Most numerical features are close to normally distributed.
- Engine size and cylinders show less normal distribution compared to other variables.
- The model performs well even with only numerical features.
