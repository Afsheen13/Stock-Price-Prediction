# Stock-Price-Prediction
### Introduction :

Reliance Industries Limited is an Indian multinational conglomerate, headquartered in Mumbai. It has diverse businesses including energy, petrochemicals, natural gas, retail, telecommunications, mass media, and textiles. Reliance is one of the most profitable companies in India, the largest publicly traded company in India by market capitalization, and the largest company in India as measured by revenue.
In this project we have done data scraping using nsepy library. We have to predict the stock price of Reliance Industries for the next 30 days. We have used machine learning model LSTM or Long Short Term Memory for making predictions.

### Dataset :
We have Reliance data from 1st Jan,2015 to 15th Feb,2023. It has 2014 rows and 14 columns. It has columns like Symbol, Series, Prev Close, Open, High, Low, Last, Close, VWAP, Volume, Turnover, Trades, Deliverable Volume, %Deliverable.

### Objective :
Predict the Reliance Industries Stock Price for the next 30 days. There are Open, High, Low and Close prices that you need to obtain from the web for each day starting from 2015 to 2022 for Reliance Industries stock.

### Methodology :
Split the last year into a test set- to build a model to predict stock price.

Find short term, & long term trends.

Understand how it is impacted from external factors or any big external events.

Forecast for next 30 days.

### Importing Pandas, Numpy and Visualization libraries.
![image](https://user-images.githubusercontent.com/118348424/229709612-80e0d57d-ff72-4237-8d21-c7e4fa87142d.png)

![image](https://user-images.githubusercontent.com/118348424/229709710-0247a130-2f5a-482b-9063-6355bcc60973.png)

### Dataset!
![image](https://user-images.githubusercontent.com/118348424/229709959-c262670d-f5ea-45aa-8f5e-9b38814d4d89.png)

### Manual EDA using info, describe, shape, isnull, corr etc.
![image](https://user-images.githubusercontent.com/118348424/229710109-df120f63-492e-442b-b52d-212bb07de00e.png)
![image](https://user-images.githubusercontent.com/118348424/229710136-b9318b3d-42ec-4d21-b2f5-6e05f0911401.png)

### Correlation between all parameters
![image](https://user-images.githubusercontent.com/118348424/229710302-c403fb62-262a-4482-8e90-83daadc35e96.png)

### Visualizing all columns using boxplot, scatterplot, histogram, distplot, pairplot, heatmap, trend chart.
![image](https://user-images.githubusercontent.com/118348424/229710434-d488edd2-bb61-475e-bd21-35f4fc6b2f51.png)

![image](https://user-images.githubusercontent.com/118348424/229710500-21fabef6-91e7-486c-9d77-178819a0bb1e.png)

![image](https://user-images.githubusercontent.com/118348424/229710528-f93a262a-9120-45ac-93b5-8d653fc00545.png)
![image](https://user-images.githubusercontent.com/118348424/229710548-39d884a4-5ee2-47f9-80ec-eeedc7f523c8.png)

![image](https://user-images.githubusercontent.com/118348424/229710706-57c9f144-b313-40f3-8aa2-969f2f167e37.png)

![image](https://user-images.githubusercontent.com/118348424/229710722-c95e38cc-1833-4530-a844-d3503b0c1193.png)

![image](https://user-images.githubusercontent.com/118348424/229710745-4f472498-0770-4627-aa08-2d463d7804ff.png)

![image](https://user-images.githubusercontent.com/118348424/229710775-9b502301-1a2c-4047-862a-38ce41c539bc.png)

### Technical Analysis using Moving Average !
'Moving Average - MA' A moving average (MA) is a widely used indicator in technical analysis that helps smooth out price action by filtering out the “noise” from random price fluctuations. It is a trend-following, or lagging, indicator because it is based on past prices.
Visualized Close Price trend using MA for 10/20/50 days to smoothen out daily fluctuations.

![image](https://user-images.githubusercontent.com/118348424/229710983-16dbf80a-9d88-417f-adc2-c4108177e119.png)

### LSTM Model
Importing TensorFlow and ScikitLearn libraries to build model.

Divided dataset into 80% training, 20% test data.

Using MinMax Scaler to get values between 0 and 1.

Using LSTM model of RNN since we have time series data to forecast.

Building the model to train 60 values and predict every 61st value using for loop.

RMSE is 30.4 which is good.

Plotting predicted values against actual values.

![image](https://user-images.githubusercontent.com/118348424/229711414-66e2ee15-f36f-4573-8751-7e691cf535f4.png)

### Deployment using streamlit 

![image](https://user-images.githubusercontent.com/118348424/229711543-25d5b501-4a32-49c5-bead-e9273cae73a3.png)
![image](https://user-images.githubusercontent.com/118348424/229711599-d7a54944-4425-405a-9e18-3ffd17369c7d.png)
![image](https://user-images.githubusercontent.com/118348424/229711631-2eecee4e-48b2-4003-b5e8-de54306421a3.png)
![image](https://user-images.githubusercontent.com/118348424/229711663-cbb22130-9f48-4d61-b8a9-bdb65d1e823f.png)
![image](https://user-images.githubusercontent.com/118348424/229711718-f9b0b422-a0a3-4add-b2e9-d5d31e3050e8.png)
![image](https://user-images.githubusercontent.com/118348424/229711764-8c5b5099-72f3-44f2-8afb-fb65d563996b.png)











