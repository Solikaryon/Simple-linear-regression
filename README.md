# Linear Regression Analysis - Car Purchase Prediction

**Author:** Monjaraz Briseño Luis Fernando

## Project Description

This Jupyter notebook implements linear regression from scratch to predict car purchase amounts based on annual salary. The project includes multiple implementations and variations to demonstrate different approaches to linear regression analysis.

## Dataset

The analysis uses the `car_purchasing.csv` dataset with the following key variables:
- **Independent Variable (X):** Annual Salary
- **Dependent Variable (Y):** Car Purchase Amount

## Implementations

The notebook contains seven different implementations:

### 1. Basic Linear Regression (Full Dataset)
- Calculates correlation matrix
- Computes mean values
- Implements complete linear regression using all data
- Visualizes data points with regression line
- Uses NumPy for calculations

### 2. Train-Test Split (60-40) - Version 1
- Splits data: 60% training, 40% testing
- Trains model on training set
- Evaluates on test set
- Visualizes both training and testing data separately

### 3. Train-Test Split (60-40) - Version 2
- Similar to version 1 with refined plotting
- Improved visualization of regression line

### 4. Train-Test Split (60-40) - Version 3
- Enhanced implementation with separate prediction plotting
- Shows predictions vs actual values for test set

### 5. Reverse Split (40-60)
- Trains on 40% of data
- Tests on 60% of data
- Demonstrates model performance with less training data

### 6. Manual Implementation (No NumPy)
- Implements all calculations without NumPy
- Manual computation of:
  - Mean values
  - Slope (m)
  - Intercept (b)
- Uses list comprehensions for predictions

### 7. Train-Test Split Without NumPy
- Combines manual calculations with train-test split
- Manual implementation of:
  - Covariance
  - Variance
  - Linear regression parameters

## Mathematical Formulas Used

### Slope (m)
```
m = cov(x, y) / var(x)
```

### Intercept (b)
```
b = ȳ - m * x̄
```

### Prediction
```
y_pred = m * x + b
```

## Visualizations

Each implementation includes:
- Scatter plots of data points
- Linear regression lines
- Mean point markers (where applicable)
- Color-coded training and testing data
- Labeled axes and legends

## Technologies Used

- **Python 3.x**
- **Libraries:**
  - `pandas` - Data manipulation and CSV reading
  - `matplotlib.pyplot` - Data visualization
  - `numpy` - Numerical computations (in some implementations)

## File Structure

```
.
├── 24b_am_d01_p1_Monjaraz_Briseño_Luis_Fernando.ipynb
├── car_purchasing.csv (required data file)
└── README.md
```

## How to Run

1. Ensure you have Python 3.x installed
2. Install required libraries:
   ```bash
   pip install pandas matplotlib numpy
   ```
3. Place the `car_purchasing.csv` file in the root directory
4. Open the Jupyter notebook:
   ```bash
   jupyter notebook 24b_am_d01_p1_Monjaraz_Briseño_Luis_Fernando.ipynb
   ```
5. Run cells sequentially to see different implementations

## Key Outputs

Each implementation outputs:
- **Slope (m):** The rate of change in car purchase amount per unit salary
- **Intercept (b):** The baseline car purchase amount
- **Visualizations:** Graphs showing data distribution and regression fit

## Learning Objectives

This project demonstrates:
- Linear regression theory and implementation
- Train-test split methodology
- Manual computation of statistical measures
- Data visualization techniques
- Comparison of library-based vs. manual implementations

## Notes

- The dataset uses Latin-1 encoding
- Random state is set to 0 for reproducibility
- Different train-test ratios show how data split affects model training

## License

Educational project for learning purposes.
