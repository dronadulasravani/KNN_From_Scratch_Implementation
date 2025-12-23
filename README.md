# KNN_From_Scratch_Implementation
---

## ⚙️ Step-by-Step Implementation

### Step 1: Load the Dataset
- Load the diamonds dataset using pandas

### Step 2: Identify Features and Target
- **Features (X):** carat, cut, color, clarity, depth, table, x, y, z
- **Target (y):** price

### Step 3: Train-Test Split
- Split data into **75% training** and **25% testing**

### Step 4: Data Preprocessing (Training Data)
- **Categorical Encoding:** One-Hot Encoding (`cut`, `color`, `clarity`)
- **Numerical Scaling:** StandardScaler
- Implemented using `ColumnTransformer`

### Step 5: Data Preprocessing (Test Data)
- Apply the same transformations using `transform()` only

### Step 6: KNN from Scratch
- Implemented Euclidean distance manually
- Predicted prices using mean of nearest neighbors
- No use of sklearn’s KNN in this step

### Step 7: Model Evaluation
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

### Step 8: Sklearn KNN Comparison
- Train `KNeighborsRegressor`
- Compare results with scratch implementation

---

## 🧮 Why Scaling & Encoding Are Important

- KNN is a **distance-based algorithm**
- Feature scaling ensures no feature dominates distance
- One-hot encoding avoids introducing artificial ordering in categorical data

---

## 📊 Results Summary

| Model | MAE | RMSE | R² |
|------|-----|------|----|
| KNN (Scratch) | Comparable | Comparable | Comparable |
| KNN (Sklearn) | Slightly Better | Optimized | Optimized |

> Minor differences occur due to vectorization and internal optimizations in sklearn.

---

## 🛠️ Libraries Used

- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib (optional for visualization)

---

## 🚀 How to Run the Project

1. Clone the repository:
   ```bash
   git clone <your-github-repo-url>
