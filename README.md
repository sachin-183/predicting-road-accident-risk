# Predicting Road Accident Risk

##  My Participation
I participated the Kaggle competition and developed the **`predicting-road-accident-risk.ipynb`** notebook as my solution.  
The notebook includes:
- Full **EDA (Exploratory Data Analysis)**
- **Feature Engineering** for categorical and numerical variables
- **Model Training** using machine learning algorithms
- **Hyperparameter Tuning**
- **Prediction Generation** for the Kaggle submission file  

My focus was on achieving a balance between **model accuracy** and **generalization** on unseen data.

---

## 📂 Dataset

### Files
- `train.csv` — Training data with accident risk labels  
- `test.csv` — Test data for generating predictions  
- `sample_submission.csv` — Example of expected submission format  

### Key Columns
| Feature | Description |
|----------|--------------|
| `road_type` | Type of road (urban, rural, etc.) |
| `num_lanes` | Number of lanes |
| `curvature` | Curvature of the road |
| `speed_limit` | Speed limit (km/h) |
| `lighting` | Lighting conditions (daylight, dim, night, etc.) |
| `weather` | Weather conditions (clear, rainy, etc.) |
| `road_signs_present` | Presence of road signs |
| `public_road` | Whether the road is public |
| `time_of_day` | Morning, afternoon, evening, or night |
| `holiday` | Whether it’s a holiday |
| `school_season` | Whether it’s during a school season |
| `num_reported_accidents` | Reported past accidents |
| `accident_risk` | Target variable (risk score between 0 and 1) |

---

## ⚙️ Methodology

### 1. Data Loading & Cleaning
- Loaded the dataset using **Pandas**
- Handled missing or inconsistent values
- Visualized feature distributions and correlations

### 2. Feature Engineering
- Encoded categorical variables using **Label Encoding** and **One-Hot Encoding**
- Scaled numerical values with **StandardScaler**
- Created interaction and polynomial features for better model expressiveness

### 3. Model Building
Tested and compared multiple models, including:
- **Linear Regression**
- **Random Forest Regressor**
- **XGBoost Regressor**
- **LightGBM Regressor**

The best-performing model was selected based on **cross-validation RMSE**.

### 4. Model Evaluation
Metrics used:
- **Mean Absolute Error (MAE)**
- **Root Mean Squared Error (RMSE)**
- **R² Score**

### 5. Submission
- Generated predictions for the test set  
- Created a `submission.csv` file following Kaggle’s format

---

## 🧠 Technologies Used
- **Python 3.x**
- **NumPy**, **Pandas**
- **Scikit-learn**
- **Matplotlib**, **Seaborn**
- **XGBoost**, **LightGBM**
- **Jupyter Notebook**

---

## 📊 Results & Insights
- The model achieved solid predictive performance with optimized parameters.
- Key influential factors on accident risk:
  - Road curvature and speed limit  
  - Weather and lighting conditions  
  - Time of day and number of lanes  
- Feature importance analysis showed that **environmental and design factors** play a crucial role in road safety.

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/sachin-183/predicting-road-accident-risk.git
