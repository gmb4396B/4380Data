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

Problem Formulation:


<img width="514" alt="image" src="https://user-images.githubusercontent.com/105134530/167278479-caeddf4f-1adb-4891-baa6-ef79ccab1a83.png">

<img width="527" alt="image" src="https://user-images.githubusercontent.com/105134530/167278515-333e9722-eb93-4328-bc5f-46af27c570cc.png">

Problem Formulation:
Input :Temperature, humidity, wind speed, wind direction, time of the day
Output: Radiation.
Model: MPLRegressor. Was able to compare with any other model because this model was more equiped with all the necessary parameters.
Solver/optimizer: Adam
Activation: Relu.

Training: Software/hardware
Python,Sklearn,Pandas, numpy,seaborn and matplotlib.
Mac-pro.
It took about between five to ten minutes to train.
When the training loss did not improve more than tol=0.000100 for 100 consecutive epochs, I stopped traing.

Performance  Matrix:
Not recommended to use Roc curve  when it is Regression

Conclusion: 
Could not evaluate the model well. Given more time i tweak the model in various ways to get better results.

Future Work:
Improve the model.
Use the model predict all weather conditions,

Reproducing results and applying the package to other data:
I wrote an addition menu function that can be used to predict temperature , pressure, Humidity using the same data set. But addition functions and adjusts can be addedd to deal with other forms of data to predidct different categorical variables.

File in the repository 
Project_Prediction_Of_Solar_Radiation.ipynb
This jupyter notebook with the code for model

ReadMe.ipynb
The ReadMe.md gives an overview of the project

proposalDatascienceProject_1.pdf
This file laid the foundation of work at the begining of the project

SolarPredictionFlowChart1.pdf
This file shows schematic design of the model. 



