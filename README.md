# Airline Passenger Satisfaction ML

A machine learning project comparing **Logistic Regression** and **Decision Trees** algorithms on the Airline Passenger Satisfaction dataset.

## 📋 Project Overview

This project implements and evaluates two classification algorithms to predict airline passenger satisfaction based on various service and flight features. The goal is to determine which model performs better for this binary classification task.

## 📊 Dataset

- **Name:** Airline Passenger Satisfaction Dataset
- **Total Records:** 103,904 passengers
- **Target Variable:** `Satisfied` (Binary: Yes/No)
- **Data Split:**
  - Training: 80%
  - Validation: 10%
  - Testing: 10%

### Features

The dataset includes 27 features covering:

**Passenger Information:**
- Gender
- Age & Age Band
- Type of Travel (Personal/Business)
- Travel Class (Economy/Business/First)
- Flight Distance
- Destination & Continent

**Service Ratings (0-5 scale):**
- Inflight WiFi Service
- Departure/Arrival Time Convenience
- Ease of Online Booking
- Gate Location
- Food and Drink
- Online Boarding
- Seat Comfort
- Inflight Entertainment
- On-board Service
- Leg Room Service
- Baggage Handling
- Check-in Service
- Inflight Service
- Cleanliness

**Flight Performance:**
- Departure Delay (minutes)
- Arrival Delay (minutes)

## 🔧 Technologies & Libraries

- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Scikit-learn** - Machine learning algorithms
  - Logistic Regression
  - Decision Trees
  - StandardScaler for feature scaling
- **Matplotlib/Seaborn** - Data visualization

## 🚀 Project Structure

```
passenger-satisfaction-ml/
├── ML_model_final.ipynb    # Main Jupyter notebook with full analysis
├── README.md               # This file
└── DATA_CW5 (S).csv       # Dataset (required for execution)
```

## 📈 Data Preprocessing

1. **Missing Value Handling:** Missing numeric values filled with column means
2. **Target Encoding:** Satisfaction converted from Y/N to 1/0
3. **Feature Engineering:** Categorical variables encoded using one-hot encoding
4. **Feature Scaling:** StandardScaler applied to normalize numeric features

## 🤖 Models

### 1. Logistic Regression
- Linear classification algorithm
- Probabilistic approach
- Good for interpretability
- Assumes linear relationship between features and log-odds

### 2. Decision Trees
- Non-parametric tree-based algorithm
- Handles non-linear relationships
- Provides feature importance ranking
- Risk of overfitting on complex datasets

## 📊 Evaluation Metrics

Models are evaluated using:
- **Accuracy** - Overall correct predictions
- **Precision** - True positives among predicted positives
- **Recall** - True positives among actual positives
- **F1-Score** - Harmonic mean of precision and recall
- **ROC-AUC** - Model discrimination ability
- **Confusion Matrix** - True/False positives and negatives

## 📝 Usage

1. **Prerequisites:**
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```

2. **Run the Analysis:**
   - Open `ML_model_final.ipynb` in Jupyter Notebook
   - Ensure `DATA_CW5 (S).csv` is in the same directory
   - Execute all cells sequentially

3. **Expected Output:**
   - Data exploration visualizations
   - Model training and validation
   - Performance comparison charts
   - Feature importance analysis

## 🔍 Key Findings

- Comprehensive feature analysis and distribution visualizations
- Model performance comparison on validation and test sets
- Insights into which features most influence passenger satisfaction
- Trade-offs between model complexity and interpretability

## 💡 How to Interpret Results

1. **Accuracy Comparison:** Shows which model predicts satisfaction more correctly overall
2. **Precision vs Recall:** Helps decide model based on business priority (minimize false positives vs false negatives)
3. **Feature Importance:** Identifies key drivers of passenger satisfaction
4. **Confusion Matrix:** Reveals specific prediction errors

## 🎯 Recommendations

- Use **Logistic Regression** if interpretability and model simplicity are priorities
- Use **Decision Trees** if non-linear patterns and automatic feature interactions matter
- Consider **ensemble methods** (Random Forest, Gradient Boosting) for potentially better performance
- Deploy model with cross-validation for more robust performance estimates

## 📚 References

- Scikit-learn Documentation: https://scikit-learn.org/
- Logistic Regression: Classic approach to binary classification
- Decision Trees: Powerful non-parametric method for classification

## 👤 Author

**Abdullah Mujeeb**

## 📄 License

This project is open source and available for educational purposes.

---

**Last Updated:** 2026-09-13

**Status:** Complete - Model comparison and analysis finished
