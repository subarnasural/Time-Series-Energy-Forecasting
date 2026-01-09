# Time-Series-Energy-Forecasting
Time Series Energy Consumption Forecasting using LSTM and GRU
# Time Series Energy Consumption Forecasting

## Project Overview
This project focuses on forecasting household energy consumption using deep learning–based time series models.  
The objective is to predict future power usage patterns based on historical consumption data and time-based features.

Accurate energy forecasting helps in load planning, demand management, and efficient energy utilization.

---

## Dataset Description
The dataset contains household power consumption measurements recorded at minute-level granularity.  
Key attributes include:
- Global active and reactive power
- Voltage and current intensity
- Sub-metering data for different household zones
- Date and time information

The data was resampled to hourly frequency for stable time series modeling.

---

## Data Preprocessing
The following preprocessing steps were applied:
- Conversion of date and time into a unified datetime index
- Handling missing values using forward filling
- Resampling minute-level data into hourly averages
- Log transformation of the target variable to stabilize variance
- Min-Max scaling for neural network training

---

## Feature Engineering
Time-based features were created to capture seasonal and behavioral patterns:
- Hour of the day
- Day of the week
- Weekend indicator

These features improve the model’s ability to learn daily and weekly consumption cycles.

---

## Models Implemented
Two deep learning models were implemented and compared:

### LSTM (Long Short-Term Memory)
- Captures long-term temporal dependencies
- Suitable for sequential energy consumption patterns

### GRU (Gated Recurrent Unit)
- Computationally efficient alternative to LSTM
- Faster convergence with competitive performance

---

## Model Evaluation
The dataset was split into:
- Training set
- Validation set
- Test set

Evaluation metrics:
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- R² Score

Both models were evaluated on unseen test data to measure generalization performance.

---

## Results
The models successfully learned energy consumption trends and produced accurate short-term forecasts.  
A comparison between LSTM and GRU demonstrated their effectiveness in time series forecasting tasks.

---

## Project Structure
Time-series-energy-forecasting/
│
├── Timeseries_Energy_Forecasting_Final_Code.ipynb
├── timeseries_energy_forecasting_final_code.py
├── requirements.txt
├── README.md

---

## Technologies Used
- Python
- NumPy, Pandas
- Matplotlib, Seaborn
- Scikit-learn
- TensorFlow (Keras)

---

## Future Improvements
- Incorporation of exogenous variables such as weather data
- Hyperparameter tuning and longer forecast horizons
- Deployment using a web dashboard or API

---

## Author
Subarna Sural  
B.Tech in Computer Science and Engineering (AI & ML)
