# Coronavirus
This is a project i did as part of my semester course for Machine Learning. It involes time series forecasting using LSTM. As a challenge, we were only limited to use of Pytorch and
Numpy for the implementation of our models. We could not use any pre made models like ARIMA in statsmodel library.

This project does time series forecasting on daily coronavirus cases reported in a country and predicts future daily cases. The current project uses data uptil 27th May for predictions. 
You can also find a demonstration of predictions made on more recent data at the end of the jupyter file (uptil 11th June). 

Due to limitation of amount of data availalble for forecasting, we also try to find realted countries to our country of choice, and use their data to make more enhanced predictions.
A few techniques used to compare time series were corrleations and differences.
