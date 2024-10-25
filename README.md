# B211_Assignment7

## Project Purpose
This project aims to predict diabetes progression using three machine learning models: **Linear Regression**, **Decision Tree Regressor**, and **Support Vector Machine Regressor (SVR)**. Using the Scikit-Learn **diabetes dataset**, we compare each model’s performance to identify the most effective approach.

### Project Overview
- **Dataset**: Diabetes Dataset
- **Models Used**:
  - Linear Regression
  - Decision Tree Regressor
  - Support Vector Machine Regressor
- **Evaluation Metrics**: Variance Score, Mean Squared Error (MSE), \( R^2 \) Score.

### Model Implementation
1. **Linear Regression**: Predicts the target variable assuming a linear relationship. Adjusted to prevent negative predictions.
2. **Decision Tree Regressor**: Captures non-linear relationships but tends to overfit, resulting in the lowest accuracy.
3. **Support Vector Regressor**: A non-linear model that requires more tuning to improve performance on larger datasets.

### Model Performance
- **Variance**: Linear Regression captured the most variance (0.45549), with Decision Tree having the lowest (0.02805).
- **MSE**: Linear Regression had the lowest error (2900.19), while Decision Tree had the highest (5149.54).
- **\( R^2 \)**: Linear Regression achieved the highest score (0.4526), indicating it best fits the data.

### Limitations
- **Default Parameters**: Lack of tuning may reduce accuracy, especially for Decision Tree and SVR.
- **Handling of Negative Predictions**: Adjusted to 0, but may affect interpretability.
- **Single Train-Test Split**: Cross-validation could improve evaluation reliability.

### Conclusion
The **Linear Regression** model performed best and is recommended for this dataset. Cross-validation and tuning would further improve model reliability and performance.
