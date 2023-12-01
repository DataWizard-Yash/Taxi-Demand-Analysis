# Taxi Demand Prediction

## Overview

This project focuses on predicting taxi demand in 15-minute intervals to optimize taxi fleet provisioning. Various models, including regression, XGBoost, ARIMA, and DNN, are implemented and compared for their suitability in forecasting taxi demand.

## Data

The dataset consists of JSON files named `year_2023_month_1` to `year_2023_month_12`, containing information about taxi trips. Each trip includes details such as driver ID, trip ID, start/end location, trip distance, speed, duration, payment type, start/end time, and trip fare.

## Assumptions

- The demand patterns exhibit short-term and long-term trends.
- Hierarchical aggregation of demand data by time and space is considered.

## Approach

1. **Data Preprocessing:**
   - Timestamps are converted to datetime format.
   - Spatial aggregation is performed.
   - Temporal features (day of the week, hour of the day) are extracted.
   - Categorical variables are encoded using OneHotEncoding.

2. **Model Selection:**
   - Regression models (linear regression, etc.).
   - XGBoost for handling complex relationships.
   - ARIMA for time series analysis.
   - Deep Neural Network (DNN) for capturing non-linear relationships.

3. **Model Evaluation:**
   - Models are evaluated using Mean Squared Error (MSE) or Root Mean Squared Error (RMSE).
   - Cross-validation is implemented for generalization assessment.

4. **Documentation:**
   - Code is well-documented with comments.
   - Visualizations illustrate data distribution, patterns, and model performance.

## Code Structure

### Data
- **Year 2023 Month 1:**
  - `year_2023_month_1.json`
- **Year 2023 Month 2:**
  - `year_2023_month_2.json`
- ...

### Code
- **Data Preprocessing:**
  - `data_preprocessing.ipynb`
- **Model Training:**
  - `model_training.ipynb`
- **Evaluation and Analysis:**
  - `evaluation_and_analysis.ipynb`

### Visualizations
- `demand_distribution.png`
- `model_comparison_chart.png`

### [README.md](README.md)

### [requirements.txt](requirements.txt)

---





## Results

- XGBoost achieved an RMSE of X.
- ARIMA achieved an RMSE of Y.
- DNN achieved an RMSE of Z.

## Challenges Faced

- Describe any challenges encountered during the project.

## Future Improvements

- Outline potential improvements or next steps for enhancing the model.

## How to Run the Code

1. Clone the repository.
2. Install dependencies: `pip install -r requirements.txt`.
3. Run the Jupyter notebooks in the `code/` directory.

## Acknowledgments

- Mention any resources, libraries, or tools used in the project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

