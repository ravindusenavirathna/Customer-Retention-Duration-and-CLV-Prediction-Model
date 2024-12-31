

# Customer Retention and CLV Prediction

This repository contains a comprehensive analysis and modeling approach for predicting **Customer Lifetime Value (CLV)** and **Retention Duration**. It includes data preprocessing, exploratory data analysis (EDA), machine learning model training, hyperparameter tuning, and evaluation. Additionally, it features custom testing functions and survival analysis to support business decision-making.



## Features

### 1. **Data Preprocessing**
- **Cleaning**:
  - Handles missing values and removes invalid data (e.g., negative quantities or prices).
- **Feature Engineering**:
  - Creates new features, such as `Revenue`, `Retention Duration`, and log-transformed values to handle skewed data.
- **Scaling and Splitting**:
  - Standardizes numerical features using `StandardScaler`.
  - Splits data into training and testing sets.

### 2. **Exploratory Data Analysis (EDA)**
- **Visualizations**:
  - Histograms for feature distributions (e.g., `Retention Duration`, `Total Revenue`).
  - Scatter plots for pairwise feature relationships.
- **Correlation Heatmap**:
  - Identifies relationships between key features (e.g., Recency, Frequency, Revenue).
- **Insights**:
  - Examines patterns to support feature selection for modeling.

### 3. **Predictive Modeling**
- Implements two models for:
  - **Retention Duration Prediction**
  - **Customer Lifetime Value (CLV) Prediction**
- **Grid Search with Cross-Validation**:
  - Hyperparameter tuning for models using `GridSearchCV`.
- **Evaluation Metrics**:
  - R² Scores
  - Root Mean Squared Error (RMSE)
  - Residual analysis and visualizations

### 4. **Custom Functions for Customer Insights**
- **Predict Retention and CLV**:
  - Predicts metrics for individual customers.
- **Visualize Customer Activity**:
  - Displays historical purchase behavior for specific customers.

### 5. **Survival Analysis**
- **Kaplan-Meier Estimator**:
  - Plots customer retention survival curves to analyze retention trends over time.



## Results Summary

1. **Retention Model**:
   - Evaluated with cross-validated R² scores and RMSE on test data.
   - Insights into factors affecting retention duration.

2. **CLV Model**:
   - Predicts customer revenue potential with competitive performance metrics.
   - Helps prioritize high-value customers for retention efforts.

3. **Survival Analysis**:
   - Demonstrates retention trends over time for strategic planning.



## Requirements

- Python 3.8+
- Required libraries:
  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn lifelines
  ```



## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your_username/Customer-Retention-CLV.git
   cd Customer-Retention-CLV
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook final.ipynb
   ```



## File Structure

- **final.ipynb**: Main Jupyter Notebook containing the entire workflow.
- **customer_segmentation.csv**: Example dataset for analysis and modeling.
- **README.md**: Documentation for the repository.



## Dataset

The dataset, `customer_segmentation.csv`, contains transactional data, including:
- **CustomerID**: Unique identifier for each customer.
- **Quantity**: Number of items purchased.
- **UnitPrice**: Price per unit.
- **InvoiceDate**: Date of the transaction.
- **Revenue**: Calculated as `Quantity × UnitPrice`.



## Usage

1. **Data Preprocessing**:
   - Load the dataset.
   - Perform cleaning and feature engineering.

2. **Modeling**:
   - Train predictive models for retention and CLV.
   - Evaluate models using R² and RMSE.

3. **Visualization**:
   - Analyze distributions, relationships, and residuals.

4. **Survival Analysis**:
   - Plot retention survival curves for insights into customer retention trends.

5. **Testing**:
   - Use custom functions to predict retention and CLV for specific customers.



## Example Visualizations

### Distribution of Retention Duration
A histogram showing the frequency distribution of retention durations.

### Revenue vs. Recency
Scatter plots analyzing how recent purchases relate to revenue generation.

### Residual Analysis
Histograms showing residuals for both retention and CLV models.



## Contributing

Contributions are welcome! Please open an issue or submit a pull request for improvements or additional features.
