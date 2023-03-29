# Travel-Mode-Choice-Analysis Project
### Purpose of project:

This travel mode choice analysis is to help transportation planners understand and forecast travel demands, which ultimately assists them in terms of decision making such as the prioritization of infrastructure investments. 

### Summary of Approach:

This project utilizes two different machine learning approaches, namely supervised learning and unsupervised learning. 
Travel mode choice prediction uses supervised learning techniques. In this approach, the model predicts the individual’s select mode of transportation based on their attribute data. Four different algorithms were used for comparison purposes: Decision Tree, Gradient Boosting Classifier, Random Forest, and Bagging Classifier. 
K-means clustering model was used for the unsupervised learning model. The unsupervised learning model allows us to understand the groups of passenger behavior. 

### Results:

For the supervised learning model, the Bagging Classifier algorithm performed the best in the prediction of travel mode choice based on 13 attributes, with an accuracy of 0.95. The high prediction accuracy in all of the classifiers tested in this study demonstrated the applicability of machine learning algorithms in predicting travel mode choice using the attributes. 
The unsupervised learning model introduces a framework for passenger segmentation and identifies their travel habits. As such, these models can form as a strong basis for growth for the ride-sharing community as well as transportation planning to strengthen their ability to analyze travel demand which can facilitate moving people. 

### Data Source:
The National Household Travel Survey (NHTS) data in the New York state was used to construct and test the two different machine learning models including supervised learning and unsupervised learning.  
Data Source Citation: U.S. Department of Transportation, Federal Highway Administration, 2017 National Household Travel Survey. URL: http://nhts.ornl.gov.
More details on Data Cleaning and modelling:
### Data Cleaning:
Feature engineering was performed to restructure and clean the selected dataset for better model tuning. Based on the insights developed from the literature reviews, 13 features have been selected to train and test the mode choice model. The final dataset contains 81,401 rows. 
The 13 attributes include: Dwell Time (DWELTIME), Start Time (STRTTIME), Travel Time (TRVLCMIN), Weekend Trip (TDWKND), Trip Purpose (TRIPPURP), Trip Distance (TRPMILES), Age (R_AGE), Sex (R_SEX), Driver Status (DRIVER), Household Income (HHFAMINC), Count of Household Vehicles (HHVEHCNT), Category of workers per square mile in the census tract of the trip destination's location (DTEEMPDN), and Category of population density (persons per square mile) in the census tract of the trip destination's location (DTPPOPDN). The travel mode choice is represented as Trip Mode (TRPTRANS) in the dataset and has been simplified into 4 main categories: walk, bike, car, public transit.
### Supervised learning model:
The results show that the Bagging Classifier produces the best overall result compared to the rest. The high accuracy in all classifiers demonstrates the effectiveness of machine learning techniques in predicting travel mode choice. 
The prediction performance of the 4 machine learning models is evaluated using accuracy. Moreover, since there is over 80,000 data points, a 70-30 train test split was used instead of cross validation. The performance metrics are reported for the test data. 
The supervised learning model is useful for policy makers and transportation and urban planners to make investment decisions in terms of transportation infrastructure. In addition, corporations that support ride-sharing applications can also benefit from this model, as this model allows them to understand users’ preferred method of transport, which determines their price elasticity. An individual who is likely to walk is price elastic and is not likely to pay a premium for ride sharing, whereas an individual who has intentions of taking a taxi would be less price elastic and may pay a premium for ride sharing service. The prediction optimizes the use of taxpayers’ money by assisting with the infrastructure investment decision. In addition, the model is also very useful in the world of competitive pricing and produce a perfect price discrimination. 
### Unsupervised learning model:
K-means clustering with 4 clusters was used to produce other insights on the segmentation of the data. Two clusters were identified to have distinct identity from the cluster centers, a working group of passengers and a retired group of passengers.
The unsupervised learning model allows us to understand the groups of passenger behavior. This is particularly interesting as it can help transportation planners to plan transit and transit times accordingly, catering transit stops and schedules to specific groups of passengers. Moreover, it is also useful for ride-sharing applications as they can group passengers of similar preferences together and perform various marketing efforts (such as giving promotions) based on passenger’s group preferences. For example, one group can receive 10% discount while the other 15% discount per trip, and this is generally optimized rigorously by A/B testing in practice, where the discount amount is a free parameter in A/B Testing experiments. 
