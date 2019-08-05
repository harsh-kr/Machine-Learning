# K Nearest Neighbours Classification
The k-nearest neighbors (KNN) algorithm is a simple, easy-to-implement supervised machine learning algorithm that can be used to solve both 
classification and regression problems.<br>
The KNN algorithm assumes that similar things exist in close proximity. In other words, similar things are near to each other. KNN can be used
for both classification and regression predictive problems. However, it is more widely used in classification problems in the industry.
To evaluate any technique we generally look at 3 important aspects:
1. Ease to interpret output
2. Calculation time
3. Predictive Power

<br>

![KNN1](https://www.analyticsvidhya.com/wp-content/uploads/2014/10/scenario1.png)
![KNN2](https://www.analyticsvidhya.com/wp-content/uploads/2014/10/scenario2.png)

<br>

### The KNN Algorithm
1. Load the data
2. Initialize K to your chosen number of neighbors
3. For each example in the data<br>
3.1 Calculate the distance between the query example and the current example from the data.<br>
3.2 Add the distance and the index of the example to an ordered collection<br>
4. Sort the ordered collection of distances and indices from smallest to largest (in ascending order) by the distances
5. Pick the first K entries from the sorted collection
6. Get the labels of the selected K entries
7. If regression, return the mean of the K labels
8. If classification, return the mode of the K labels
