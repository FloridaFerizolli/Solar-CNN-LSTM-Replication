# Solar Irradiance Forecasting Using a CNN-LSTM Model

This repository contains the code and data for our group project in the *AI for Global Challenges* module at the University of Birmingham. We extended and replicated the study by Qing and Niu (2018), titled *"Hourly day-ahead solar irradiance prediction using weather forecasts by LSTM"* by incorporating a hybrid CNN-LSTM model.

## About the Study

The original paper used an LSTM-based deep learning model to forecast hourly solar irradiance one day in advance using multivariate weather features. Our project replicates and expands this approach by combining CNN and LSTM layers to improve the model’s ability to learn both local patterns and long-term dependencies in weather sequences.

We also prioritised transparency and accessibility by implementing the preprocessing pipeline using only NumPy and open-source libraries.

## Project Summary

- **Environment**: Jupyter Notebook (University of Birmingham vLab)
- **Language**: Python
- **Libraries**: NumPy, TensorFlow, Keras, matplotlib, scikit-learn
- **Data**: Publicly available weather and irradiance datasets from NREL
- **Model**: CNN-LSTM (50 LSTM units, trained for up to 100 epochs with EarlyStopping)
- **Evaluation Metric**: Root Mean Squared Error (RMSE)
- **Result**: Test RMSE = 0.0953 (scaled)

Both training and validation loss curves showed smooth convergence, and prediction plots demonstrated strong alignment with actual values.

## Files Included

- `solar_forecast_model_final.ipynb` – Final Jupyter Notebook with code and output
- `train_NREL_solar_data.csv` – Training dataset
- `validate_NREL_solar_data.csv` – Validation dataset
- `test_NREL_solar_data.csv` – Test dataset
- `README.md` – This file

## How to Run

1. Clone or download this repository.
2. Open `solar_forecast_model_final.ipynb` in Jupyter Notebook or Google Colab.
3. Ensure the three CSV data files are located in the same directory.
4. Run all cells from top to bottom.

The test RMSE and training performance plots will be displayed at the end of the notebook.

## Ethical and Societal Context

This project was developed using free, open-source tools with the intention of making deep learning for energy forecasting more accessible. The NumPy-based pipeline ensures that the approach can be replicated by users with limited computing resources. We also highlight the need for diverse, region-specific datasets and model transparency, particularly when deploying forecasting tools in energy-insecure settings.

## Reference

Qing, X. and Niu, Y., 2018. *Hourly day-ahead solar irradiance prediction using weather forecasts by LSTM*. Energy, 148, pp.461–468. https://doi.org/10.1016/j.energy.2018.01.177

## Authors

This project was submitted as part of the *AI for Global Challenges* module.

- Esther Daramola
- Aimee Twum-Danso
- Florida Ferizolli
