SOM self-organising maps are unsupervised deep learning models that help in reducing dimensionality  by using neural networks
Used for feature detection,  anomaly detection
For fraud detection In credit card applications applications


In SOM first random weights are initialized , for a single example (customer) of the dataset the mean interneuron distance (MID) for all the nodes is calculated and the node with lowest MID(BMU-Best matching unit) is assigned to the example(customer).

After we find BMU for a node, we update the weights of the node and also the weights of the nodes which come under the BMUs radius. The closer to the BMU the more is the weight updated. 

The above is continued orv many times.Initilally the radius for each BMUs will  be high. But over iterations the radius will be reduced . to update the weights of nodes in the best possible way.
