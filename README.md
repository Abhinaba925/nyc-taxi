# 🚕 NYC Taxi Trip Duration Prediction

<p align="left">
  <img src="https://img.shields.io/badge/license-MIT-green.svg" alt="License: MIT">
  <img src="https://img.shields.io/badge/status-complete-blue.svg" alt="Project Status: Complete">
  <img src="https://img.shields.io/github/last-commit/your-username/nyc-taxi-prediction" alt="Last Commit">
</p>

This project tackles the [NYC Taxi Trip Duration competition on Kaggle](https://www.kaggle.com/c/nyc-taxi-trip-duration). It showcases a complete machine learning workflow, including in-depth **exploratory data analysis (EDA)**, advanced **feature engineering**, and the implementation of three powerful gradient boosting models: **XGBoost**, **LightGBM**, and **CatBoost**. Finally, it combines these models into an **ensemble** to achieve superior predictive accuracy.



---

## ✨ Features

* **In-depth EDA:** Visual analysis of trip durations, temporal patterns (rush hours, day of the week), and geographical distributions to inform feature creation.
* **Advanced Feature Engineering:** Creation of high-impact features like **Haversine distance** to calculate trip length and extraction of time-based features from timestamps.
* **Multi-Model Implementation:** Training and evaluation of XGBoost, LightGBM, and CatBoost to compare their performance on a real-world dataset.
* **Ensemble Modeling:** Combination of the individual model predictions into a single, more robust prediction using an averaging ensemble.

---

## 🛠️ Tech Stack & Tools

| Category | Technology / Tool |
| :--- | :--- |
| **Data & Analysis** | pandas, numpy |
| **Machine Learning**| scikit-learn, XGBoost, LightGBM, CatBoost |
| **Data Visualization** | matplotlib, seaborn |
| **Environment** | Jupyter Notebook / Python Scripts |

---

## ⚙️ Installation & Setup

Follow these steps to get the project running locally.

### Prerequisites

* Python (version 3.8 or higher)
* Git

### Steps

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/nyc-taxi-prediction.git](https://github.com/your-username/nyc-taxi-prediction.git)
    cd nyc-taxi-prediction
    ```

2.  **Create and activate a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install dependencies:**
    ```bash
    pip install pandas numpy scikit-learn xgboost lightgbm catboost matplotlib seaborn
    ```

4.  **Download the data:**
    Download `train.csv` and `test.csv` from the [Kaggle competition page](https://www.kaggle.com/c/nyc-taxi-trip-duration/data) and place them in the root directory of the project.

---

## 🚀 Usage

To run the full training, evaluation, and prediction pipeline, execute the main script from your terminal.

```bash
python train_model.py
