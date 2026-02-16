# Used Car Price Intelligence: AI-Enhanced Valuation 🚗📊

## Project Overview
This project develops a robust predictive engine to estimate the market value of used cars. By leveraging **Multivariate Regression** techniques and **Polynomial Feature Mapping**, the model identifies non-linear relationships between a vehicle's age, mileage, engine size, and fuel efficiency to provide accurate pricing insights.

This repository demonstrates a modern **AI-assisted Data Science workflow**, utilizing Generative AI for code optimization, logic validation, and rapid prototyping of complex visualization pipelines.

## 🧠 Technical Workflow
A hybrid approach was used to ensure both statistical rigor and development efficiency:

1. **Exploratory Data Analysis (EDA):** Performed deep-dive analysis to identify skews in fuel types and handle missing tax data via median imputation.
2. **Feature Engineering:** Applied `PolynomialFeatures` (Degree 2) to capture hidden interactions between variables that a standard linear model would miss.
3. **Regularization & Optimization:** Implemented **Ridge Regression (L2 Regularization)** to handle multi-collinearity. Used `GridSearchCV` to find the optimal alpha ($\alpha=10$).
4. **AI-Assisted Development:** Leveraged GenAI to streamline the creation of modular preprocessing pipelines and validate statistical assumptions during model selection.

## 📈 Model Performance & Results
The final Ridge Regression model significantly outperformed simple linear benchmarks by capturing combined feature effects.

| Metric | Multi-Variable Ridge Model |
| :--- | :--- |
| **R² Score** | **0.7080** |
| **MAE** (Mean Absolute Error) | **£1,754.02** |
| **RMSE** (Root Mean Sq. Error) | **2,558.99** |

### Key Insights:
* **Non-Linearity:** Used car prices do not depreciate linearly; polynomial mapping was essential to improve accuracy from an initial R² of ~0.34 to **0.71**.
* **Generalization:** The model achieved a CV R² of **0.74** during grid search, indicating strong performance on unseen market data.
* **Feature Importance:** Vehicle 'Year' and 'Engine Size' were identified as the primary drivers of valuation.

## 🛠️ Tech Stack
* **Programming:** Python
* **Libraries:** Scikit-Learn, Pandas, NumPy, Matplotlib, Seaborn
* **Environment:** Jupyter Notebook / Google Colab
* **Methodologies:** L2 Regularization, Polynomial Transformation, Hyperparameter Tuning, AI-Augmented Programming

## 📂 Repository Structure
* `Used Car Price Intelligence.ipynb`: Full analytical pipeline including data cleaning, EDA, and modeling.
* `README.md`: Project documentation and performance summary.

## 🚀 How to Use
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/Used-Car-Price-Intelligence.git](https://github.com/YOUR_USERNAME/Used-Car-Price-Intelligence.git)
