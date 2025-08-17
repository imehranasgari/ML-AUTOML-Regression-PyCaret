# 🏠 House Price Prediction – Regression with PyCaret

## 1. Problem Statement and Goal of Project

The goal of this project is to predict house prices using a regression model built with the **PyCaret** library. The dataset used is the **House Prices: Advanced Regression Techniques** dataset, which involves predicting the `SalePrice` of homes based on various features like neighborhood, size, and condition.

---

## 2. Solution Approach

* **Data Preprocessing**

  * Loaded and cleaned the dataset, handling missing values by imputing with the mean.
  * Applied normalization and dimensionality reduction (PCA) to enhance model performance.

* **Model Setup**

  * Used PyCaret’s `setup()` function to prepare the dataset, excluding irrelevant features like `Alley` and `PoolQC`, which are not helpful for regression.

* **Model Creation and Comparison**

  * Applied multiple regression models using PyCaret’s `compare_models()` to find the best-performing one.
  * Fine-tuned hyperparameters and evaluated the models based on performance metrics like RMSE.

* **Interpretation and Insights**

  * Once the best model was selected, PyCaret’s built-in `interpret_model()` function was used for analyzing model predictions and understanding feature importance.

---

## 3. Technologies & Libraries

* **Python**
* **PyCaret** – A low-code machine learning library for building and deploying models efficiently.
* **Pandas** – For data manipulation and handling.
* **Matplotlib** – For visualization (if applicable).

---

## 4. Description about Dataset

* **train-houseprice.csv** – The training dataset containing house features (e.g., `OverallQual`, `GrLivArea`, `GarageCars`) and the target variable `SalePrice`.
* **test-houseprice.csv** – The test dataset for which predictions were made.

The dataset includes several categorical and numerical features, which were processed using techniques like **one-hot encoding** and **numerical imputation**.

---

## 5. Installation & Execution Guide

1. **Clone the repository**:

   ```bash
   git clone <repo-url>
   cd <repo-folder>
   ```
2. **Install dependencies**:

   ```bash
   pip install pycaret pandas matplotlib
   ```
3. **Run the notebook**:

   ```bash
   jupyter notebook PyCaret_reg.ipynb
   ```

---

## 6. Key Results / Performance

* The **best regression model** was selected after comparing various algorithms using PyCaret’s built-in model comparison tools.
* The model achieved a satisfactory performance with a low **RMSE**, demonstrating its capability to predict house prices accurately.

---

## 7. Screenshots / Sample Outputs

Typical outputs include:

* Model performance metrics.
* Visualization of model interpretations, including feature importance.

---

## 8. Additional Learnings / Reflections

* **PyCaret** simplifies the process of model creation and comparison, enabling rapid experimentation with minimal code.
* The integration of **PCA** improved the model's ability to handle high-dimensional data efficiently, reducing the risk of overfitting.
* The project highlights the effectiveness of automated machine learning tools for regression tasks, making it easier for data scientists to iterate quickly.

---

## 👤 Author

**Mehran Asgari**
📧 [imehranasgari@gmail.com](mailto:imehranasgari@gmail.com)
🌐 [https://github.com/imehranasgari](https://github.com/imehranasgari)

---

## 📄 License

This project is licensed under the Apache 2.0 License – see the `LICENSE` file for details.

---

> 💡 *Some interactive outputs (e.g., plots, widgets) may not display correctly on GitHub. If so, please view this notebook via [nbviewer.org](https://nbviewer.org) for full rendering.*

---
