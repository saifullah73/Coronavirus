# Coronavirus Daily Case Forecasting
This is a project i did as part of my semester course for Machine Learning(CS471). It involes time series forecasting using LSTM. As a challenge, we were only limited to use of Pytorch and Numpy for the implementation of our models. We could not use any pre made models like ARIMA in statsmodel library.  
This project does time series forecasting on daily coronavirus cases reported in a country and predicts future daily cases. The current project uses data uptil 27th May for predictions. You can also find a demonstration of predictions made on more recent data at the end of the jupyter file (uptil 11th June). 

## This project involes:
### Finding Related Countries
Due to limitation of amount of data available for forecasting, we try to find realted countries to our country of choice, and use their data to make more enhanced predictions.
We used two techniques to compare time series 
1. Correlation
2. Difference of Series   
Final decision was made by giving 40% weightage to correlation scores, and 60% weightage to difference scores.On this analysis we identify 5 countries we think are most realted to our country of choice (Pakistan in our case)  

### Forecasting
We use data of each country uptil 10th May and make predctions uptil 27th May, and compare the results with the real life daily cases. We also train our models on data upto 27th May and then predict cases one month into the future.
LSTM were trained on daily cases trends, which was non stationary, a demo also exists in which series were made stationary prior to being fed to our model.

### More Recent Results
You can also find daily corona virus cases predctions made for more recent data (11th June). These prediction were made for Pakistan ,and LSTM were trained on series after smoothing them with a moving average window of 5.






