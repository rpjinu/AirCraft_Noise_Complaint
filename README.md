# AirCraft_Noise_Complaint
"Time series forecasting of aircraft noise complaints by community using ARIMA models."
<img src="https://github.com/rpjinu/AirCraft_Noise_Complaint/blob/main/Air_India_airCraft.png" width="1200">

# Aircraft Noise Complaints Forecasting

This project focuses on time series forecasting of aircraft noise complaints by community using ARIMA models. The dataset contains counts of complaints by community and by month, collected by the Aircraft Noise Abatement Office.

## Project Overview

The objective of this project is to predict future aircraft noise complaints based on historical data. The predictions can help in understanding and managing community concerns about aircraft noise disturbances.

## Dataset Information

- **Source**: The dataset is collected by the Aircraft Noise Abatement Office via the Complaint Hotline, Online Complaint Form, emails, letters, and telephone calls. It is used in monthly reports presented at the SFO Airport Community Roundtable meetings.

### Attributes:
- `Year`: The year of the aircraft noise complaint disturbance.
- `Month`: The month of the aircraft noise complaint disturbance.
- `Community`: The name of the community where the aircraft noise disturbance occurred.
- `Total Complaints`: The number of monthly complaints associated with the community.
- `Total Number of Callers`: The number of complainants associated with the community.
- `data_loaded_at`: Date the data was loaded onto the Open Data Portal.

## Project Structure

1. **Data Preparation**: 
   - Combined `Year` and `Month` columns to create a `Date` column.
   - Grouped data by `Date` and `Community` to aggregate complaints.

2. **Model Selection**: 
   - ARIMA (AutoRegressive Integrated Moving Average) models were chosen for time series forecasting.

3. **Model Training**: 
   - The data was split into training (80%) and testing (20%) sets.
   - ARIMA models were trained for each community.

4. **Model Evaluation**: 
   - The performance was evaluated using Mean Squared Error (MSE) on the test data.

5. **Forecasting**: 
   - The trained ARIMA models were used to forecast future complaints.

6. **Model Saving**:
   - The trained models were saved using `joblib` for future use.


