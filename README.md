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
We managed to merge 2 dataframes, create new columns from main columns and delete unnecessary columns to create columns we needed for the research and delete the ones we didn't. This coding process is shown the [Data Cleaning Code](https://github.com/ElijahAgunbiade/Machine-LearningAutomatidata/DataCleaningCode). This resulted in us having a column 'generous' which depicted whether a customer was considered to be generous by the percentage of tip they gave compared to the total cost of the trip. This would be very useful in the proceeding on the research.

## Design and implement a machine learning model
We created a Random Forest Classifier and an XGB Classifier and compare the F1 Score to identity the most accurate model in predicting the kind of customers that would be the most generous tippers. 

We first began by testing the balance of the data based on the amount of data that had generous customers and the amount that didn't. This was to make sure our future model would have enough data of generous and ungenerous tippers to be able to accurately understand and predict what factors make a generous tipper without reporting false or unrepresentative statements. Our outcome fortunately came out to our generous tippers being 52% of the data, as seen in the image below, which is about even; therefore, there would be no misinterpretation when creating the model.  

![balance](https://github.com/ElijahAgunbiade/Machine-LearningAutomatidata/assets/173221971/9c7e353e-f528-4cba-a916-2094fc95501b)

Knowing the data wasn't biased, we decided to build a Random Forest Classifier with our test data as well as an XGB Classifier to test their F1 scores. We also fitted training set on both Classifiers for better results.

![random forest](https://github.com/ElijahAgunbiade/Machine-LearningAutomatidata/assets/173221971/9cd55447-5712-4ab5-9566-b9d5a16edebc)

![XGB classifier](https://github.com/ElijahAgunbiade/Machine-LearningAutomatidata/assets/173221971/4a8b9326-db2c-4bbd-b547-39983ba00fcb)

![F1 Score overall](https://github.com/ElijahAgunbiade/Machine-LearningAutomatidata/assets/173221971/306f6029-f2ed-4ead-9e18-e18216d8902a)

Seeing that our F1 scores in both classifiers are over .50, this means using either models gives us a better chance of predicting who will be a generous tipper than, say a coin flip by about a 40% increase. However, given that our Rainforest Classifier has a higher F1 score than our XGB model, we opted for the Rain Forest Classifier as a higher F1 score means this model is better for prediction in this dataframe than the XGB model. 

We then created a Confusion Matrix to understand the characteristics of the Rain Forest Classifyer. We found that the model is almost twice as likely to predict a false positive than it is to predict a false negative. This means the model is far more likely to predict a generous tipper and be wrong, than to predict a normal tipper and be wrong. This is less desirable, because it's better for a driver to be pleasantly surprised by a generous tip when they weren't expecting one than to be disappointed by a low tip when they were expecting a generous one. However, the overall performance of this model was satisfactory.

![confustion matrix](https://github.com/ElijahAgunbiade/Machine-LearningAutomatidata/assets/173221971/b8316abf-2476-47d1-b146-4b7aa2522a70)

Lastly, we created a bar graph to plot the most influencial features that affects whether a customer will be a generous tipper or not in a descending order. We found that vendor id(who the driver is), predicted fare(how much the trip itself is expected to cost), average duration (how long the trip last), and average distance plays a heavy impact whether a customer would be a generous tipper or not

![graph](https://github.com/ElijahAgunbiade/Machine-LearningAutomatidata/assets/173221971/97360365-fafd-4311-b10f-2727c54e57f4)

##Executive Summary
Well.....





