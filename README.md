# Credit_card-fraud-detection
An anomaly detection model by using self organizing map (SOM) .

First, we install the Minisom package then we import the necessary libraries then we load the CSV file then divided it into two parts the X which will be trained and they just for adding markers for visualisation which will tell if the credit card was approved or not for specific winning nodes.


 then we apply feature scaling by using min Max scaler that is normalisation we assign a variable Som to create an object of mini Som class we are creating a 10X10 size unit size of map, Input length is 15 because there are 14 features plus one customer_id column. Sigma is the radius of BMU.

 Then randomly initialize weights then we train our self-organising map 
now we will visualise the map.

Mean interneuron  distance(MID)

bone adds Window on which map will be shown
Som.distance gives mean interneuron distance(MIDS) as a matrix and pcolor plots those MIDs on the graph/plot/map.

Now we will iterate through every applicant in the data set, 
Then, we will find the coordinates of the winning node with the help of .winner method and then add a marker at the specific node according to the applicant’s card approval. White MIDs are outliers because their inter neurone distance are larger so they are the ones that are anomalies. 

Win_map method gives all the customers in each winning node.
The white nodes, outline winning nodes have all the outliers. So  mapping[(8,1)] gives a list of all the outlier customers 
To reverse the feature scaling we will be using inverse_transform
The frauds are given in as an array of lists of customers’ features. Finally, we print the fraudulent ids.
