# Project 

## King County Housing Price Prediction
The objective is to understand and process the data to make a model to predict future prices of the houses in this area. 
There a few things I need to do before diving into that. I have to check which data is continous and which is categorical. 
I need to deal with this data differently, therefore I will separate them into two different datasets. 
The dataset is quite big, (21597) therefore I will have to take a more general approach towards cleaning the data. 
Not inspecting the data checking variables one by one.

## Components
### Jupyter Notebook
The Jupyter Notebook is our key deliverable and contains details of our approach and methodology, data cleaning, exploratory data analysis, model training and tuning and recommendations.

### Presentation
The presentation gives a high-level overview of our approach, findings and recommendations for non-technical stakeholders. It is aimed to be between 5 and 10 minutes long.

### Data
The dataset can be found in this repository. 


### data Analysis 
#### What month is better to buy a house? 

![image](https://user-images.githubusercontent.com/36000513/116996312-22fcc580-acd3-11eb-88b1-d56f15d5278d.png)

![image](https://user-images.githubusercontent.com/36000513/116996288-19735d80-acd3-11eb-9241-baa093efda93.png)


Based on the previous graphs we can say that best time to buy a house is during the months of winter, which are: December, January and February. February being the best option out of them. The second best season will be Autumn, which includes September,October,November. November being the best option.


#### How does location affect prices? 

![image](https://user-images.githubusercontent.com/36000513/116996438-4de71980-acd3-11eb-84e5-0bb4d58deaaf.png)

There is a big difference in House price depending on the location. It is visible that house prices are higher at north than south, with prices ranging from 1.4 Million to 800.000. Also we can see that Houses with waterfront are more expensive as well, hence the most expensive location will be Mercer Island, Bellevue and Sammamish


#### what features affect price the most? 
![image](https://user-images.githubusercontent.com/36000513/116998820-b388d500-acd6-11eb-8dae-6e7db7ca889d.png)

![image](https://user-images.githubusercontent.com/36000513/116998843-bd123d00-acd6-11eb-9c8d-4aa4a2e655f4.png)

![image](https://user-images.githubusercontent.com/36000513/116998858-c0a5c400-acd6-11eb-86cb-c2cfd5bda81e.png)

![image](https://user-images.githubusercontent.com/36000513/116998878-c56a7800-acd6-11eb-98da-d6a69d44aa2f.png)

Overall, after sqft_living we can say that grade, bathrooms and bedrooms shows a good relationship with price, as when they increase so does price.

### Modelling
I will be creating 3 different models for this particular project.

Model X
This model will use simple linear regression. I want to see if with the most specific feature I can get a decent R^2 Metric

Model Y
This Model will use multiple linear regression. Increasing the amount of independent variables, to see if R^2 increases and to what point.

Model Z
This model will be the most complete and accurate. I will be aiming for the highest R^2 value and lowest Root Mean Squared Error.

Both Models, Y and Z will have the features with a p-value lower than 0.05

### Conclusion

![image](https://user-images.githubusercontent.com/36000513/116999045-03679c00-acd7-11eb-9bc7-b975d4abb70b.png)



Here we can see that the values compared with the TEST RMSE in the other table are not too far away from each other:

Model X Multiple Linear Regression Version C:

Cross-Validation Mean RMSE = 185585
Test RMSE = 184828

There's a 0.5% difference between them

Model Y Multiple Linear Regression Version C:

Cross-Validation Mean RMSE:101542
Test RMSE:101520

There's a 0.03% difference between them

Model Z Multiple Linear Regression Version C:

Cross-Validation Mean RMSE:103203
Test RMSE:103191
There's a 0.01% difference between them

Looking at all the data above I have come to the conclusion that the best Model is:

Model Z Multiple Linear Regression Version C

