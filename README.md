# Estimation of Reference Evapotranspiration Using Machine Learning Models  
### A Case Study of the Ogun-Osun River Basin

---

## 📘 Abstract

Accurate estimation of reference evapotranspiration (ET₀) is essential for sustainable water resource management and the planning of agricultural ecosystems. This research evaluates the performance of various machine learning algorithms in predicting and forecasting monthly ET₀ within the Ogun-Osun River Basin (OORB).

Using 38 years of satellite meteorological data from NASA, ET₀ values were calculated for nine stations under OORB using the FAO-56 Penman-Monteith method. After performing feature extraction and correlation analysis, five optimal feature combinations were selected, with solar radiation and maximum temperature emerging as the most influential variables.

## 🧠 Machine Learning Models

The following ML algorithms were evaluated for ET₀ **prediction**:

- ✅ Support Vector Regression (SVR)
- ✅ Artificial Neural Network (ANN)
- ✅ Decision Tree (DT)
- ✅ Random Forest (RF)
- ✅ Extreme Gradient Boosting (XGBoost)

For **forecasting**, the study implemented:

- 🔁 **XGBoost** with extracted time-series features
- 🔁 **ARIMA** model

## 📊 Dataset

- **Source**: NASA satellite meteorological data
- **Duration**: 38 years of monthly data
- **Stations**: 9 locations across the Ogun-Osun River Basin
- **Features Used**: Solar Radiation, Max Temperature, and others (5 combinations total)
- **ET₀ Ground Truth**: FAO-56 Penman-Monteith model output

## 🧪 Performance Evaluation Metrics

- 📈 Coefficient of Determination (R²)
- ❌ Mean Absolute Error (MAE)
- ⚠️ Relative Absolute Error (RAE)
- 📉 Root Mean Square Error (RMSE)

## 📌 Key Findings

- **SVR** achieved the best results overall, with RMSE as low as **0.0444 mm/day**.
- **Decision Tree** showed the worst performance across most stations (RMSE up to **0.3278 mm/day**).
- With **just three key features**, ML models retained high accuracy — proving feature selection critical.
- **XGBoost** outperformed **ARIMA** in 5 of 9 stations when forecasting future ET₀ values.
The notebook and datasets used can be found in the codes and ETo folders respectively

## 🛠️ Tools & Libraries

- Python
- Pandas, NumPy
- scikit-learn
- XGBoost
- statsmodels (ARIMA)
- matplotlib, seaborn
- Jupyter Notebook

# Structure
```
ETo-estimation/
├── data/          # Processeed meteorological data
├── notebook/      # Main Jupyter Notebook Files            
└── README.md
```

## 📝 Citation
If using this research, kindly cite as:
Aiyegbeni I.T. Estimation of Reference Evapotranspiration Using Machine Learning Models: A Case Study of the Ogun-Osun River Basin. 2025.

- Link to the published manuscript: [Manuscript](https://abuja2024certificate.niae.net/downloads/NIAE_PROCEEDING_ABUJA_2024.pdf)
- Certification: [Certification](https://drive.google.com/file/d/1xo3v-4zBEnf7ydDHV9tGFd66Z7C5Y-b3/view?usp=sharing)

