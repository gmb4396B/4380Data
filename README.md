# 4380Data
PREDICTION OF RADIATION PRODUCED PHOTO VOLTAIC CELLS

TASK:
Prediction how much radiation that can be harvest by solar cells.

My approach:
Neural Networks model MPLRegressor to predict radiation. I chose this model because it has all the necessary parameters required to 
accomplish the task. Also it has been used by others in prediction of weather.

Performance:
Due to time constraints I have not been able fully evaluate the model. But I was successful in getting the model to predict radiation to particular time I wanted.  Afte the training loss did not improve more than tol=0.000100 for 100 consecutive epochs, the model stopped traing.
It give a score of 70%

Summary of Work Done:

Data:
I obtain data from Kaggle Data Science website.
Input:Features are Radiatio, temperature wind speed, wind direction, humidity, pressure, hour of the day, sunrise hour and sunset hour.
Size of the data is: 3MB
I split data into 80% training and 20% testing.

Processing And Cleaning:
Used regular expressions and lamda expression get the some of the categories of data into string format.
Also normalize/stardized because the data was very skewed.
Using Pandas loc function I was able to pinpoint particular hours of the day or month of the year.
Then used to_numpy() function turn array format

Data Visualization:
<img width="571" alt="image" src="https://user-images.githubusercontent.com/105134530/167278553-82a83368-f404-4e36-93ff-773f9c85eceb.png">


![image](https://user-images.githubusercontent.com/105134530/167278463-cd9634ce-d687-4b69-addb-e5a04906d139.jpeg)

<img width="514" alt="image" src="https://user-images.githubusercontent.com/105134530/167278479-caeddf4f-1adb-4891-baa6-ef79ccab1a83.png">

<img width="527" alt="image" src="https://user-images.githubusercontent.com/105134530/167278515-333e9722-eb93-4328-bc5f-46af27c570cc.png">


