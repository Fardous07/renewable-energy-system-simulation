# Energy System Modeling and Renewable Forecasting Toolkit

Three integrated models for energy analysis:
1. **PyPSA-based Energy System Model** (Optimization)  
2. **ARIMA Solar Irradiance Forecast** (Time Series)  
3. **Hybrid LSTM Wind Speed Forecast** (Machine Learning)

---

## 🔌 Energy System Model (PyPSA)
**Model**: Linear optimization of electricity grid with renewables + storage  
**Features**:
- Hourly resolution over 24 hours
- Solar PV, wind turbines, gas peakers, and battery storage
- Cost-minimized dispatch with GLPK/HiGHS solvers
- Visualization of generation mix and storage dynamics

### 📁 Files
- `energy_system_model.py`: Main optimization script
- `grid_dispatch.png`: Generation/storage results
- `cost_breakdown.csv`: Operational cost analysis

### 🛠️ Dependencies
```bash
pip install pypsa numpy pandas matplotlib


# Renewable Energy Forecasting Models

Advanced time-series forecasting models for solar irradiance (ARIMA) and wind speed (hybrid LSTM with attention and wavelet transforms), using synthetic data.

## 🌞 ARIMA Solar Irradiance Forecast
**Model**: ARIMA (AutoRegressive Integrated Moving Average)  
**Features**:
- Synthetic solar irradiance data with diurnal cycles and noise
- ACF/PACF analysis for parameter selection
- 24-hour ahead forecasting with confidence intervals
- MSE evaluation and visualization

### 📁 Files
- `arima_solar_forecast.py`: Main script for data generation, modeling, and plotting
- `arima_forecast_results.csv`: Forecast outputs (actual vs predicted)
- `acf_plot.png`: Autocorrelation plot for ARIMA parameter tuning
- `arima_forecast.png`: Forecast vs actual plot

### 🛠️ Dependencies
```bash
pip install pandas numpy matplotlib statsmodels scikit-learn
