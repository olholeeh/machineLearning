## Student Performance Prediction (student-por dataset)

### 1. Dataset Loading

The dataset was loaded into a pandas DataFrame using `pd.read_csv()` with a semicolon (`;`) separator, as required for this dataset format.

### 2. Data Exploration

Initial exploration was performed using:

* `df.head()` to preview the data
* `df.info()` to understand data types
* `df.describe()` to summarize numerical features

The dataset contains both numerical and categorical variables related to student demographics, social factors, and academic performance.

### 3. Data Cleaning

The dataset was checked for missing values using `df.isnull().sum()`.
No significant missing values were found, so no rows or columns were removed.

### 4. Feature Engineering

Categorical variables were transformed into numerical format using **One-Hot Encoding**.
This step allows the regression model to process non-numeric data.

### 5. Data Preparation

* The target variable was set as **G3 (final grade)**
* Features (X) and target (y) were separated
* Data was split into training and testing sets using a **60/40 split**

### 6. Model Training

A **Linear Regression model** (same as used in the lab) was trained using a pipeline that includes preprocessing and modeling steps.

### 7. Model Evaluation

The model was evaluated using:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score

The model achieved a good level of accuracy, indicating that prior grades (G1, G2) and other factors are strong predictors of final performance.

### 8. Visualization

The following graphs were used to evaluate model performance:

* **Actual vs Predicted Plot** to assess prediction accuracy
* **Residual Plot** to analyze error distribution
* **Histogram of Residuals** to check normality

### 9. Conclusion

The Linear Regression model performed well on the dataset.
Previous academic performance (especially G2) was the most influential factor in predicting final grades.
The model demonstrates that student performance can be reasonably predicted using available features.
