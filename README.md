# Sales Analysis Portfolio

This project demonstrates a comprehensive analysis of retail sales data, including data preprocessing, visualization, and machine learning modeling to predict weekly sales. The analysis is designed to showcase data analytics skills suitable for internships or professional roles in data analytics.

## Project Overview

The project uses three datasets to analyze retail sales:
- **Features data set**: Contains additional data about each store, such as temperature, fuel price, markdown information, and holidays.
- **Sales data set**: Includes weekly sales data for various departments across stores.
- **Stores data set**: Provides metadata about the stores, such as type and size.

The primary objective is to build a linear regression model to predict weekly sales based on the provided features.

---

## Steps Performed

1. **Data Loading and Exploration**
   - Loaded datasets and examined their structure and summary statistics.
   - Checked for missing values and inconsistencies.

2. **Data Preprocessing**
   - Converted date columns to datetime format.
   - Merged the datasets into a single cohesive dataset.
   - Imputed missing values using the mean strategy.

3. **Feature Engineering**
   - Extracted new features such as `Day_of_Week` and `Month` from the date column.
   - Encoded categorical variables using one-hot encoding.

4. **Visualization**
   - Explored sales distribution and trends.
   - Created a correlation heatmap to understand feature relationships.

5. **Modeling**
   - Split the data into training and testing sets.
   - Built a linear regression model to predict weekly sales.
   - Evaluated model performance using RMSE and R² metrics.

---

## Results

- **Model Evaluation**:
  - Root Mean Squared Error (RMSE): 21754.57
    
  This value indicates the average error (in the same units as the target variable, "Weekly Sales") between the predicted    and actual values. In this case, the model's predictions deviate by approximately 21,754 units of weekly sales on   average. A lower RMSE is better, but this figure should be interpreted in the context of the data's range and variance.

  - R² Score: 0.0924
    
  This value explains the proportion of variance in the target variable (Weekly Sales) that is explained by the model. Here, approximately 9.24% of the variation in weekly sales is captured by the model, suggesting that the current model is not highly predictive. Improvements, such as incorporating more features or using a more complex model, could be explored.

- **Key Insights**:
  - Seasonal trends significantly impact sales.
  - Certain features, such as store size and markdown values, show strong correlations with sales.

---

## How to Use

1. Clone this repository:
   ```bash
   git clone https://github.com/Ezeekie04/Retail-Sales-Analysis
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook Portfolio\ 1.ipynb
   ```

---

## Dependencies

- Python 3.8+
- Pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn
- Jupyter Notebook

---

## Files in Repository

- **Portfolio 1.ipynb**: Main analysis notebook.
- **README.md**: Documentation for the project.
- **Datasets**: (https://www.kaggle.com/datasets/manjeetsingh/retaildataset)

---

## License

This project is for educational purposes and is open-source under the MIT License.
