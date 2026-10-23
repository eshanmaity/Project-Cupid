# 💘 Project Cupid — AIML Capstone Project

**An End-to-End Machine Learning Project | Classification & Regression**

Project Cupid is an Artificial Intelligence and Machine Learning (AIML) capstone project focused on building, evaluating, and comparing machine learning models through a structured workflow. The project explores data preprocessing, feature selection, cross-validation, hyperparameter tuning, and performance evaluation for both classification and regression tasks.

---

## 🎯 Project Objectives

* Understand and preprocess the dataset for machine learning.
* Handle missing values and investigate potential outliers.
* Apply appropriate feature preprocessing and scaling techniques.
* Build and compare multiple classification models.
* Develop and evaluate regression models.
* Use cross-validation to obtain more reliable performance estimates.
* Apply feature selection and hyperparameter tuning.
* Compare baseline models with tuned models using appropriate evaluation metrics.

---

## 🛠️ Technologies Used

* **Language:** Python
* **Environment:** Google Colab / Jupyter Notebook
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
* **Machine Learning:** Classification, Regression, Feature Selection, Hyperparameter Tuning
* **Evaluation:** Cross-Validation, Accuracy, Precision, Recall, F1-Score, ROC-AUC, MAE, RMSE, R²

---

## 🔬 Project Workflow

The project follows a structured machine learning workflow divided into five modules.

### 1. Data Understanding and Exploration

* Inspect the dataset structure and features.
* Examine data types and descriptive statistics.
* Identify missing values and investigate feature distributions.

### 2. Data Preprocessing

* Handle missing values using suitable imputation techniques.
* Investigate outliers using statistical methods, including the Interquartile Range (IQR).
* Apply appropriate feature scaling where required.
* Prepare data for model training and evaluation.

### 3. Classification

Implement and compare classification algorithms, including:

* Logistic Regression
* Decision Tree Classifier
* Random Forest Classifier
* K-Nearest Neighbors (KNN)
* AdaBoost Classifier

**Evaluation metrics:**

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC

### 4. Regression

Implement and compare regression algorithms, including:

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor
* K-Nearest Neighbors Regressor
* AdaBoost Regressor

**Evaluation metrics:**

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score

### 5. Model Optimization and Evaluation

* Apply cross-validation to compare model performance.
* Perform feature selection using `SelectFromModel`.
* Use `RandomizedSearchCV` for hyperparameter tuning.
* Compare tuned models with baseline models.
* Evaluate the selected models on held-out test data.

---

## 📊 Classification Results

The following results are mean cross-validation scores obtained during model comparison.

| Model                    | Mean Accuracy | Accuracy Std. Dev. | Mean F1-Score | Mean ROC-AUC |
| ------------------------ | ------------: | -----------------: | ------------: | -----------: |
| Logistic Regression      |        0.8458 |             0.0112 |        0.5603 |       0.8689 |
| AdaBoost Classifier      |        0.8250 |             0.0150 |        0.5096 |       0.8380 |
| Decision Tree Classifier |        0.7938 |             0.0222 |        0.4787 |       0.7451 |
| Random Forest Classifier |        0.8302 |             0.0182 |        0.4743 |       0.8394 |
| KNN Classifier           |        0.8219 |             0.0227 |        0.4659 |       0.7967 |

### Tuned Classification Model

A Random Forest classification pipeline was optimized using feature selection and randomized hyperparameter search.

* **Baseline Logistic Regression F1-Score:** 0.5603
* **Tuned Random Forest F1-Score:** 0.5797
* **Absolute F1-Score improvement:** 0.0194

The tuned Random Forest achieved a modest improvement in cross-validated F1-Score over the baseline Logistic Regression model. Final model selection should also consider held-out test performance and the project's evaluation objectives.

---

## 📈 Regression Results

The following results are mean cross-validation scores obtained during regression model comparison.

| Model                   | Mean MAE | Mean RMSE | Mean R² |
| ----------------------- | -------: | --------: | ------: |
| Random Forest Regressor |   0.5523 |    2.7585 |  0.4435 |
| AdaBoost Regressor      |   1.6486 |    3.2479 |  0.2526 |
| KNN Regressor           |   0.5648 |    3.4162 |  0.2530 |
| Linear Regression       |   1.5877 |    3.8449 |  0.0515 |
| Decision Tree Regressor |   0.6900 |    3.8824 |  0.0001 |

### Tuned Regression Model

A Random Forest regression pipeline was optimized using feature selection and randomized hyperparameter search.

* **Baseline Random Forest RMSE:** 2.7585
* **Tuned regression RMSE:** 2.8916

The tuned model did not outperform the baseline Random Forest on cross-validated RMSE. This highlights the importance of comparing optimized models against baseline performance rather than assuming that hyperparameter tuning will always improve results.

*Note: These are cross-validation results, not held-out test-set metrics.*

---

## 🧠 Key Learnings

* Data preprocessing plays an important role in building reliable machine learning pipelines.
* Different algorithms perform differently depending on the data and evaluation metric.
* Accuracy alone may not fully represent classification performance, particularly when classes are imbalanced.
* Cross-validation provides a more robust basis for model comparison than a single training split.
* Feature selection can reduce the number of input features used by a model.
* Hyperparameter tuning does not guarantee better performance.
* Classification and regression require different evaluation metrics and model-selection criteria.

---

## 🚀 How to Run the Project

The project notebook can be executed in Google Colab without installing Python locally.

1. Open the `.ipynb` notebook from this repository.
2. Click **Open in Colab**, or download the notebook and upload it to Google Colab.
3. Run the notebook cells in order.
4. Review the preprocessing steps, model comparisons, evaluation metrics, and visualizations.

### Local Execution

To run the notebook locally, install Python and Jupyter Notebook, then install the required libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open `Project_Cupid_AIML_Capstone.ipynb` and execute the cells sequentially.

---

## 📁 Repository Structure

```text
Project-Cupid-AIML/
│
├── Project_Cupid_AIML_Capstone.ipynb
├── README.md
└── LICENSE
```

Additional reports, visualizations, and dependency files can be added as the project evolves.

---

## 🔮 Future Improvements

* Explore additional classification and regression algorithms.
* Investigate class imbalance and decision-threshold optimization.
* Perform systematic feature importance analysis.
* Compare further hyperparameter optimization strategies.
* Add clear visualizations for model performance and error analysis.
* Improve reproducibility through fixed random seeds and documented dependencies.
* Develop an interactive interface for exploring predictions and model results.

---

## 👨‍💻 Author

**Eshan Maity**

B.Tech — Computer Science and Engineering
Institute of Engineering & Management, Kolkata

* **GitHub:** [@eshanmaity](https://github.com/eshanmaity)
* **LinkedIn:** [Eshan Maity](https://www.linkedin.com/in/eshan-maity-b7610b366/)

---

## 📄 Disclaimer

This project was developed as an AIML capstone project for educational and practical machine learning experience. Reported performance values represent cross-validation results from the current model experiments; they should not be interpreted as guaranteed performance on unseen data.

---

⭐ If you find this project useful, feel free to explore the notebook and its machine learning workflow.
