Introduction
My goal is to understand the data good enough to make a model to predict future prices of the houses in this area. 
There a few things I need to do before diving into that. I have to check which data is continous and which is categorical. 
I need to deal with this data differently, therefore I will separate them into two different datasets. 
The dataset is quite big, (21597) therefore I will have to take a more general approach towards cleaning the data. 
Not inspecting the data checking variables one by one.

Modelling
I will be creating 3 different models for this particular project.

Model X
This model will use simple linear regression. I want to see if with the most specific feature I can get a decent R^2 Metric

Model Y
This Model will use multiple linear regression. Increasing the amount of independent variables, to see if R^2 increases and to what point.

Model Z
This model will be the most complete and accurate. I will be aiming for the highest R^2 value and lowest Root Mean Squared Error.

Both Models, Y and Z will have the features with a p-value lower than 0.05