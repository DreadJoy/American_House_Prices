# 🏠 American House Prices — Data Science Project

This project explores predictive modeling of American house prices using a combination of deep learning and ensemble methods. We integrate a neural network, Monte Carlo dropout (for uncertainty quantification), and a random forest regressor to build a strong ensemble model.

---

## 📊 Dataset Description
- **Source**: American Housing Dataset (CSV format)
- **Size**: ~40,000 rows × 14 columns
- **Features**: Includes square footage, number of rooms, year built, location data, etc.
- **Target Variable**: House price (log-transformed for modeling)
- **Preprocessing**:
  - Missing value handling
  - Feature scaling
  - Log-transform of target variable

---

## 🧠 Modeling Approach
### Models Used:
1. **Neural Network (NN)**
   - Two hidden layers with dropout
   - Optimized with Bayesian hyperparameter tuning
2. **Monte Carlo Dropout (MC)**
   - Used during inference to estimate predictive uncertainty
3. **Random Forest (RF)**
   - Tree-based model with good performance on structured data

### Ensemble Strategy:
- Combine all three models via simple averaging:
  ```
  Final Prediction = (NN + MC Dropout + RF) / 3
  ```
- We also tested weighted and optimized blending strategies.

---

## 📈 Results
| Model           | R² Score | RMSE     |
|----------------|-----------|----------|
| Neural Net     | 0.7630    | 0.4035   |
| MC Dropout     | 0.7629    | 0.4036   |
| Random Forest  | 0.7727    | 0.3952   |
| **Ensemble**   | **0.7754** | **0.3928** |

- The ensemble performed best, capturing the strengths of each model.
- The models generalize well across the entire housing price spectrum (small homes to luxury mansions).

---

## 📉 Uncertainty & Explainability
- MC Dropout was used to generate prediction intervals and visualize model uncertainty.
- SHAP (SHapley Additive exPlanations) plots helped identify important features for RF and NN.

---

## 🔮 Future Work
- Predict buyer preferences and match homes to likely customers.
- Add geospatial modeling or clustering by ZIP code.
- Explore pricing trends over time for forecasting.

---

## 🚀 How to Run
1. Clone the repository
2. Open the Jupyter Notebook (`American_House_Data.ipynb`)
3. Install requirements: `pip install -r requirements.txt`
4. Run cells in order to reproduce results

---

## ✅ Final Thoughts
This project demonstrates the value of combining multiple modeling strategies. Neural networks, probabilistic methods, and tree-based models each contribute unique insights. Together, they form a more powerful predictive tool.

We’ll revisit this dataset in a future project focused on customer-side modeling. For now, this ensemble sets a solid baseline.

---

**Author**: DreadJoy 
**Email**: daverywolf@gmail.com
**LinkedIn**: linkedin.com/in/david-keller-b76753265   

