# Machine-Learning Automatidata
We are creating a machine learning model for a fictional Taxi company 'Automatida' to ancipate whether or not a customer will be a generous tipper to their drivers. We will implement feature engineering, model development, and evaluation to figure out what factors affect that. 
## Background on the Automatidata scenario
Automatidata works with its clients to transform their unused and stored data into useful solutions, such as performance dashboards, customer-facing tools, strategic business insights, and more. They specialize in identifying a client’s business needs and utilizing their data to meet those business needs. 

Automatidata is consulting for the New York City Taxi and Limousine Commission (TLC). New York City TLC is an agency responsible for licensing and regulating New York City's taxi cabs and for-hire vehicles. The agency has partnered with Automatidata to develop a regression model that helps estimate taxi fares before the ride, based on data that TLC has gathered. 

The TLC data comes from over 200,000 taxi and limousine licensees, making approximately one million combined trips per day. 

Note: This project's dataset was created for pedagogical purposes and may not be indicative of New York City taxi cab riders' behavior.

## Assignment
We will create a machine learning model for the TLC data to predict whether or not a customer is a generous tipper, what features affect that, and calculate the machine learning model's accuracy.

In this project, we will complete the following deliverables:

Complete a PACE planner mapping questions, data clean, data organize, and action items for each stage of the project scenario

Design and implement a machine learning model

Draft an executive summary of your results

## Data Cleaning and Organizing
We managed to merge 2 dataframes, create new columns from main columns and delete unnecessary columns to create columns we needed for the research and delete the ones we didn't. This coding process is shown the Data Cleaning Code file. This resulted in us having a column 'generous' which depicted whether a customer was considered to be generous by the percentage of tip they gave compared to the total cost of the trip. This would be very useful in the proceeding on the research.

## Design and implement a machine learning model
We created a Random Forest Classifyer to identity the best parameters to follow for the most accurate model in predicting the kind of customers that would be the most generous tippers. 
We first began by testing the balance of the data based on the amount of data that jad generous customers and the amount that didn't. This was to make sure our future model would have enough data of generous and ungenerous tippers to be able to accurately understand what factors make a generous tipper and predict if a new customer would be one. 

![balance](https://github.com/ElijahAgunbiade/Machine-LearningAutomatidata/assets/173221971/9c7e353e-f528-4cba-a916-2094fc95501b)

