# Appliances-Energy-Prediction-by-Linear-Regression
The Dataset is at 10 min for about 4.5 months. The house temperature and humidity conditions were monitored with a ZigBee wireless sensor network.Each wireless node transmitted the temperature and humidity conditions around 3.3 min. Then, the wireless data was averaged for 10 minutes. The energy data was logged every 10 minutes with m-bus energy metres. Weather from the nearest airport weather station(Chievres Airport,Belgium) was downloaded from a public data set from Reliable Prognosis (rp5.ru) and merged together with the experimental data sets using the date and time column. Two random variables have been included in the data set for testing the regression models and to filter out non-predictive attributes. You need to predict the energy use of appliances.

![image](https://user-images.githubusercontent.com/122529968/229991524-602ecc8b-b8a5-4343-8630-d6b1b123deac.png)


## Problem Statement
The Dataset is at 10 min for about 4.5 months. The house temperature and humidity conditions were monitored with a ZigBee wireless sensor network.Each wireless node transmitted the temperature and humidity conditions around 3.3 min. Then, the wireless data was averaged for 10 minutes. The energy data was logged every 10 minutes with m-bus energy metres. Weather from the nearest airport weather station(Chievres Airport,Belgium) was downloaded from a public data set from Reliable Prognosis (rp5.ru) and merged together with the experimental data sets using the date and time column. Two random variables have been included in the data set for testing the regression models and to filter out non-predictive attributes. You need to predict the energy use of appliances.

**1.What is the mean comparison of all the features with every other feature?\
2.What is the Energy Consumption by Appliances per month?\
3.What is the Energy Consumption by Appliances per day arranged according to months?\
4.What is the Energy consumption for individual hour of day in total 4.5 months?\
5.On which day of the week, the energy consumption is highest**

## Project Summary -
Appliances Energy Dataset is providing the very useful information over 29 features including the datapoints on Visibility,Atmospheric Pressure, Windspeed and Dewpoint of surrounding area. We all know the relation between the surrounding temperature and household energy consumption pattern in various regions of world.For e.g In South India the Diuranal temperature change is low and revolves around 3-4 degrees. The perinial temperature is high and hence they might require cooling equipments more fequently. Hence incresing their energy consumption. This relationship have been expressed in the Appliances Energy Dataset.
In the Project we are going to perform a EDA to deep dive into the trends hidden in the Data. In addition with it we are going to perform the Linear Regression model to predict the basic energy consumption by the Appliances. In this project we are finding the relationship between 28 features in response with one dependent variable, so that we could be more accurate while performing the Predictions.

## Project Insights

 1.In the Dataset, the Appliances feature and Date feature is unleashing the large amount of information.

2.The remaining columns are usuall and standard at their on an average value. For e.g the Atmospheric Pressure column shows most of the normal variation as it remain constant most of the times.

3.The temperature at rooms are mostly average and humidity also show variation around its mean value.For e.g The normal room temperature of kitchen is near about 20 degrees.

4.In most of the rooms the temp is very normal and maintained.But the mean temperature outside the building is very low at 7.5 degrees.

5.The Dataset has been studied in Belgium, which is an european country and face North Sea from North-West in addition, it has close geographical connections with Scandanavian countries which are very cold places and comes under the Arctic Circle.

6.This might be the reason for its very less temperature.

7.Despite of having very less outside temperature,the room temperatures are maintained throughout all the rooms. Hence the house may be using the heaters inside the rooms, so this may have incresed the room temperature. So increased temperature may not only due to using the Appliances but due to some other factors also.

8.These factors can be anything, so observing the energy consumption in houses may underperform in comparison with recorded temperature.

9.When we have studied the months and its energy consumption, we just have grouped all the months and find out the sum of energy consumption in whole month.

10.The Dataset is studied in 2016 and for its first five months.It has been found that the month of march shows highest energy consumption by Appliances, near about 43000 Wh.

11.When we used 'hour' as our basis of analysis, we got to know about the evening's 6 'o' clock when the energy consumption is highest from whole day in the four months.

12.It was 4th day of April when the Appliances have consumed highest amount of energy.

13.When we come to the weekdays, Saturday was the day when highest Energy have been consumed by Appliances.

## Conclusion

The Linear Regression Model for pedicting the appliances energy shows the 35% accuracy for training dataste and 33% for testing accuracy.

The Lasso and Ridge Regularization do not show much significant improvement over the normal Linear Regression. Only 2% of accuracy have been improved in Regularization.

The Decision Tree Regressor have shown a significant improvement for both train and test accuracy. It shows 72% accuracy for training Dataset an 46% accuracy for the testing Dataset. But still the model is very less in its accuracy.

So Extreme Gradient Boost Regressor is turn to be most significant model here with highest train and test accuracy , 89% and 63% respectively.

It is turn out to be that the Temperature outside the building, temperature of parents room and Dewpoint contributes for maximum significance while calculating the model.
