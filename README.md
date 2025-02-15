# American House Prices Analysis  

## Overview  
This project analyzes **40,000+ house listings** across the U.S. to identify **key factors affecting home prices**. Through **data cleaning, feature engineering, and machine learning models**, we determine the strongest predictors of housing prices.  

## 📝 Key Insights  
✅ **Living Space (log-transformed)** is the most important feature for predicting home prices.  
✅ **Median Household Income & Geographic Location (Latitude/Longitude)** significantly impact house prices.  
✅ **Linear Regression performed poorly**, but **Random Forest improved accuracy significantly.**  

## 🛠️ Tech Stack  
- **Python**: Data analysis & modeling  
- **Pandas & NumPy**: Data manipulation  
- **Matplotlib & Seaborn**: Data visualization  
- **Scikit-Learn**: Machine learning models  
- **Google Colab**: Development environment  

## 📂 Dataset  
- **Source**: [Mention if it’s public; otherwise, describe the dataset]  
- **Size**: 40,000+ rows, 14 columns  
- **Key Features**: Price, Beds, Baths, Living Space, Zip Code, Median Household Income  

## 📊 Data Preprocessing & Feature Engineering  
- Handled **missing values** and removed redundant features.  
- Applied **log transformation** to reduce the impact of skewed data.  
- Created a new **Beds_Baths_Total** feature to improve model performance.  

## 📈 Models, Hyperparameter, Performance  
| Model and HP        | MSE (↓)      | MAE (↓)      | R² Score (↑)  |  
|---------------------|--------------|--------------|---------------|  
| **Linear Regression** | 775B  | 334K  | **0.29 (Poor)**    |  
| **Decision Tree**     | 661B  | 206K  | **0.39 (Better)**  |  
| **XGBoost**           | 309B  | 174K  | **0.72 (XGBoost)** |
| **Random Forest**     | 272B  | 156K  | **0.75 (Best!)**   |  

✅ **Random Forest performed the best, capturing complex relationships in housing prices.**  

##  Next Steps  
Try **Gradient Boosting Models (LightGBM)** for better performance.  
Use **Geospatial Data Visualization (Folium, Plotly)** for location-based insights.  
Expand the dataset with **external economic factors** like interest rates.  

## 🚀 How to Run the Project  
1️⃣ Clone this repository:  
```bash  
git clone https://github.com/yourusername/american-house-prices.git  
```  
2️⃣ Install dependencies:  
```bash  
pip install pandas numpy matplotlib seaborn scikit-learn  
```  
3️⃣ Run the Jupyter Notebook or Python script:  
```bash  
python analysis.py  
```  

##  Connect with Me  
📧 Email: daverywolf@gmail.com
🔗 LinkedIn: linkedin.com/in/david-keller-b76753265 
🖥️ GitHub: https://github.com/DreadJoy/American_House_Prices
