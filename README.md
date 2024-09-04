# US_Housing

## Project Overview

The `US_Housing` project aims to predict housing prices in the United States using various regression techniques. By analyzing key features of houses, such as size, number of rooms, and location, the goal is to create a model that can accurately estimate housing prices. This project uses data analysis, feature engineering, and model optimization techniques to build and evaluate the performance of multiple regression models.

## Dataset

- **Source:** Download the dataset from Kaggle: [USA Housing Dataset](https://www.kaggle.com/datasets/bhavinmoriya/usa-housing/).
- **Data:** The dataset includes features such as area population, house age, number of rooms, and more. The target variable is the price of the house.

## Methodology

### Data Analysis

- **Visualization and Exploration:**
  - Used `Matplotlib` for plotting and visualizing data distributions.
  - Applied `Groupby()`, `info()`, `duplicated()`, `isnull()`, and `describe()` to explore and clean the dataset.

- **Feature Transformation:**
  - Employed `OrdinalEncoder()` to convert categorical variables into numerical formats suitable for model training.

- **Correlation Analysis:**
  - Utilized `seaborn.heatmap()` to visualize and analyze correlations between different features.

### Data Preparation

- **Data Splitting:**
  - Used `sklearn's train_test_split` to divide the dataset into training and testing sets, ensuring that the model is evaluated on unseen data.

- **Normalization:**
  - Applied `MinMaxScaler()` to normalize the data, improving the performance and convergence of the regression models.

### Model Development

- **Algorithms Used:**
  - Trained models using three regression algorithms: `LinearRegression()`, `Lasso()`, and `Ridge()`.

- **Hyperparameter Tuning:**
  - Implemented `RandomizedSearchCV` to optimize model parameters and perform cross-validation, enhancing model performance.

### Model Evaluation

- **Performance Metrics:**
  - Evaluated the models using several metrics:
    - **Root Mean Square Error (RMSE)**
    - **Mean Absolute Error (MAE)**
    - **Median Absolute Error**
    - **Explained Variance Score**
    - **R2 Score**

## Results

The models were evaluated using various metrics, with `LinearRegression()`, `Lasso()`, and `Ridge()` models providing insights into the relationships between the features and housing prices. The best model was selected based on its performance on the test data.

## Conclusion

This project demonstrated the use of regression models to predict housing prices in the U.S. The application of data normalization, feature encoding, and hyperparameter tuning contributed to the accuracy and reliability of the predictions.

## Future Work

- **Feature Engineering:**
  - Further refine features and explore additional variables to improve model predictions.

- **Advanced Modeling:**
  - Experiment with more complex algorithms, such as Random Forest or Gradient Boosting, to capture non-linear relationships in the data.

- **Model Deployment:**
  - Deploy the model as a web application to allow users to predict housing prices in real-time.


