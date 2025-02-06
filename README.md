# Blood-Sugar-Forecasting
This project involves predicting blood glucose levels one hour into the future using LSTM and XGBoost models.

##Note
The dataset used in this project is not included to maintain confidentiality. The data was collected from my personal 780G insulin pump.

##Important Notes
This experiment is for personal training purposes only and does not provide medical advice.
The used files include:
Sensor data from the pump.
Insulin dosage data.
These files were merged based on timestamps.

Data Preprocessing:
A 5-minute interval exists between each glucose reading.
All records where the sensor was inactive or where the time interval between readings exceeded 5 minutes were removed.
Columns that were irrelevant to the analysis were dropped.
Data analysis was performed using ACF, PACF, and correlation studies. Supporting visuals are provided below.
Modeling:
XGBoost and LSTM models were developed to predict glucose levels one hour ahead.
Results suggest that LSTM outperformed XGBoost in generalization for this particular case.
Supporting results and visuals are included for reference.

for XGboost
Train RMSE: 4.325172075998727
Test RMSE: 7.725846688515379

for LSTM 
Train RMSE: 4.444908921167074
Test RMSE: 5.115404317750811
