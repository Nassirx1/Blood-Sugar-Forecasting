# Blood-Sugar-Forecasting
This project involves predicting blood glucose levels one hour into the future using LSTM and XGBoost models.

## Note
The dataset used in this project is not included to maintain confidentiality. The data was collected from my personal 780G insulin pump.

## important Notes
This experiment is for personal training purposes only and does not provide medical advice.
The used files include:
Sensor data from the pump.
Insulin dosage data.
These files were merged based on timestamps.

## Data Preprocessing
A 5-minute interval exists between each glucose reading.
All records where the sensor was inactive or where the time interval between readings exceeded 5 minutes were removed.
Columns that were irrelevant to the analysis were dropped.

description of data.JPG
![description of data](https://github.com/user-attachments/assets/c0942a92-f280-4ba7-bbc6-b6c471a5f2c6)
diabetes ACF.png
![diabetes ACF](https://github.com/user-attachments/assets/10a0cebf-e3db-4cb8-b733-9e02c47bed44)
diabetes PACF.png
![Diabetes PACF](https://github.com/user-attachments/assets/43f8f83e-4945-4057-a91d-14d63404ff39)
diabetes correlation.png
![diabetes correlation](https://github.com/user-attachments/assets/307bbcdd-5d22-4a2e-b7f6-6750b64b69de)

Blood-Sugar-Forecasting
ta analysis was performed using ACF, PACF, and correlation studies. Supporting visuals are provided below.
Modeling:
XGBoost and LSTM models were developed to predict glucose levels one hour ahead.
Results suggest that LSTM outperformed XGBoost in generalization for this particular case.
Supporting results and visuals are included for reference.

## for XGboost
Train RMSE: 4.325172075998727
Test RMSE: 7.725846688515379
![XGboost results](https://github.com/user-attachments/assets/1280840b-7eae-41aa-a2fc-2744cc93031b)

## for LSTM 
Train RMSE: 4.444908921167074
Test RMSE: 5.115404317750811
![LSTM results](https://github.com/user-attachments/assets/a6c9b1a7-901b-49bf-84ab-9a1623c3802f)
