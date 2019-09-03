# Clustering
Clustering is the task of dividing the population or data points into a number of groups such that data points in the same groups are
more similar to other data points in the same group than those in other groups. In simple words, the aim is to segregate groups with
similar traits and assign them into clusters.

<br>

![Cluster](https://www.analyticsindiamag.com/wp-content/uploads/2018/10/photo-1442436575481-b94af86bd2cd.jpg)

<br>
Let’s understand this with an example. Suppose, you are the head of a rental store and wish to understand preferences of your costumers
to scale up your business. Is it possible for you to look at details of each costumer and devise a unique business strategy for each one
of them? Definitely not. But, what you can do is to cluster all of your costumers into say 10 groups based on their purchasing habits
and use a separate strategy for costumers in each of these 10 groups. And this is what we call clustering.
<br>
Two of the most popular clustering algorithms are – K Means clustering and Hierarchical clustering.
<br>

### KMeans Clustering
K means is an iterative clustering algorithm that aims to find local maxima in each iteration. This algorithm works in these 5 steps :
1. Specify the desired number of clusters K : Let us choose k=2 for these 5 data points in 2-D space. <br>
![img1](https://www.analyticsvidhya.com/wp-content/uploads/2016/11/clustering-2.png)
2. Randomly assign each data point to a cluster : Let’s assign three points in cluster 1 shown using red color and two points in cluster
2 shown using grey color. <br>
![img2](https://www.analyticsvidhya.com/wp-content/uploads/2016/11/clustering-2-1.png)
3. Compute cluster centroids : The centroid of data points in the red cluster is shown using red cross and those in grey cluster using
grey cross. <br>
![Img3](https://www.analyticsvidhya.com/wp-content/uploads/2016/11/clustering-3.png)
4. Re-assign each point to the closest cluster centroid : Note that only the data point at the bottom is assigned to the red cluster
even though its closer to the centroid of grey cluster. Thus, we assign that data point into grey cluster <br>
![Img4](https://www.analyticsvidhya.com/wp-content/uploads/2016/11/clustering-4.png)
5. Re-compute cluster centroids : Now, re-computing the centroids for both the clusters. <br>
![Img5](https://www.analyticsvidhya.com/wp-content/uploads/2016/11/clustering-5.png)

<br>

Repeat steps 4 and 5 until no improvements are possible : Similarly, we’ll repeat the 4th and 5th steps until we’ll reach global optima.
When there will be no further switching of data points between two clusters for two successive repeats. It will mark the termination of 
the algorithm if not explicitly mentioned.

### Hierarchical Clustering
Hierarchical clustering, as the name suggests is an algorithm that builds hierarchy of clusters. This algorithm starts with all the data
points assigned to a cluster of their own. Then two nearest clusters are merged into the same cluster. In the end, this algorithm
terminates when there is only a single cluster left. <br>
The results of hierarchical clustering can be shown using dendrogram. The dendrogram can be interpreted as: <br>
![HC](https://www.analyticsvidhya.com/wp-content/uploads/2016/11/clustering-6.png)

<br>

At the bottom, we start with 25 data points, each assigned to separate clusters. Two closest clusters are then merged till we have just
one cluster at the top. The height in the dendrogram at which two clusters are merged represents the distance between two clusters in 
the data space.
<br>
The decision of the no. of clusters that can best depict different groups can be chosen by observing the dendrogram. The best choice of
the no. of clusters is the no. of vertical lines in the dendrogram cut by a horizontal line that can transverse the maximum distance
vertically without intersecting a cluster.
<br>
In the above example, the best choice of no. of clusters will be 4 as the red horizontal line in the dendrogram below covers maximum
vertical distance AB.
<br>

![HC2](https://www.analyticsvidhya.com/wp-content/uploads/2016/11/clustering-7.png)

1. This algorithm has been implemented above using bottom up approach. It is also possible to follow top-down approach starting with all
 data points assigned in the same cluster and recursively performing splits till each data point is assigned a separate cluster.
2. The decision of merging two clusters is taken on the basis of closeness of these clusters. There are multiple metrics for deciding 
the closeness of two clusters : <br>
Euclidean distance: ||a-b||2 = √(Σ(ai-bi)) <br>
Squared Euclidean distance: ||a-b||22 = Σ((ai-bi)2) <br>
Manhattan distance: ||a-b||1 = Σ|ai-bi| <br>
Maximum distance:||a-b||INFINITY = maxi|ai-bi| <br>
Mahalanobis distance: √((a-b)T S-1 (-b))   {where, s : covariance matrix} <br>

## Difference between Kmeans and Hierarchical Clustering
1. Hierarchical clustering can’t handle big data well but K Means clustering can. This is because the time complexity of K Means is
linear i.e. O(n) while that of hierarchical clustering is quadratic i.e. O(n2).
2. In K Means clustering, since we start with random choice of clusters, the results produced by running the algorithm multiple times
might differ. While results are reproducible in Hierarchical clustering.
3. K Means is found to work well when the shape of the clusters is hyper spherical (like circle in 2D, sphere in 3D).
4. K Means clustering requires prior knowledge of K i.e. no. of clusters you want to divide your data into. But, you can stop at 
whatever number of clusters you find appropriate in hierarchical clustering by interpreting the dendrogram

## Applications of Clustering
Clustering has a large no. of applications spread across various domains. Some of the most popular applications of clustering are:

1. Recommendation engines
2. Market segmentation
3. Social network analysis
4. Search result grouping
5. Medical imaging
6. Image segmentation
7. Anomaly detection
