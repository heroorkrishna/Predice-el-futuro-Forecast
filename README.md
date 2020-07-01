# Predice-el-futuro-Forecast.

Time Series forecasting techniques are very important for a data scientist to master as time series data occur in every domain from medical, stock market, climate change prediction, and so on.

Data consist of two files:

train_csv.csv: The training dataset consists of 80 observation with observation id, timestamp and feature value.

test_csv.csv:The next 40 observation along with observation id and timestamp are present here. You'll have to predict the value of feature at these timestamps.

value to predict: The value of feature attribute has to be predicted.

File Description
train_csv.csv - the training set
test_csv.csv - the test set
Data Fields
id - observation ID
time - timestamp for the given observation
feature - target feature to be predicted
Requirement
A solution.csv file will have to be submitted in order to enter the leaderboard. Solution.csv file will consist of two fields:

id: observation ID
feature: the predicted value of feature column


$$$$$$$$$$$$$$$$$$###################################################

I have used the LSTM ml model to predict the next outcome. I first split the data into 80/20 train/test. Then convert the x_train and y_train into NumPy array then reshape those arrays to shape accepted by LSTM models. Thenbuild t the LSTM network model, thereafter compiling the model and then training the model at 100 epochs.Then creating the test data for x_test and y_test and then converting it into np array and reshaping it similarly we did for train data.Then we make predictions and calculate the next 10min outcome and calculate the RMSE Score(112.14).Finally making a plot of test and prediction.
