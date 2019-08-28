# Classification
In machine learning and statistics, classification is a supervised learning approach in which the computer program learns from the data 
input given to it and then uses this learning to classify new observation. This data set may simply be bi-class (like identifying whether 
the person is male or female or that the mail is spam or non-spam) or it may be multi-class too.
<br>

![ML](https://miro.medium.com/max/599/0*SbLLq8PDBbxkMO6X.png)

<br>
For example, spam detection in email service providers can be identified as a classification problem. This is a binary classification
since there are only 2 classes as spam and not spam. A classifier utilizes some training data to understand how given input variables 
relate to the class. In this case, known spam and non-spam emails have to be used as the training data. When the classifier is trained
accurately, it can be used to detect an unknown email. <br>
Classification belongs to the category of supervised learning where the targets also provided with the input data. There are many
applications in classification in many domains such as in credit approval, medical diagnosis, target marketing etc
<br>

# Classification Algorithms

<br>
There is a lot of classification algorithms available now but it is not possible to conclude which one is superior to other. It depends on 
the application and nature of available data set. For example, if the classes are linearly separable, the linear classifiers like Logistic
regression, Fisher’s linear discriminant can outperform sophisticated models and vice versa.
<br>

## K Nearest Neighbours
The k-nearest neighbors (KNN) algorithm is a simple, easy-to-implement supervised machine learning algorithm that can be used to solve both
classification and regression problems.
The KNN algorithm assumes that similar things exist in close proximity. In other words, similar things are near to each other. KNN can be 
used for both classification and regression predictive problems. However, it is more widely used in classification problems in the
industry.

<br>

![KNN](https://camo.githubusercontent.com/73ca4c78c884d1d1cb654df85378cbbab9b76e54/68747470733a2f2f7777772e616e616c79746963737669646879612e636f6d2f77702d636f6e74656e742f75706c6f6164732f323031342f31302f7363656e6172696f312e706e67)
![KNN2](https://camo.githubusercontent.com/d551c83c63d841f282a76dd73439fe0cfbe87e2f/68747470733a2f2f7777772e616e616c79746963737669646879612e636f6d2f77702d636f6e74656e742f75706c6f6164732f323031342f31302f7363656e6172696f322e706e67)

<br>

### The KNN Algorithm
1. Load the data
2. Initialize K to your chosen number of neighbors
3. For each example in the data
3.1 Calculate the distance between the query example and the current example from the data.
3.2 Add the distance and the index of the example to an ordered collection
4. Sort the ordered collection of distances and indices from smallest to largest (in ascending order) by the distances
5. Pick the first K entries from the sorted collection
6. Get the labels of the selected K entries
7. If regression, return the mean of the K labels
8. If classification, return the mode of the K labels

<br> <br>

## Logistic Regression
It is a statistical method for analysing a data set in which there are one or more independent variables that determine an outcome. The
outcome is measured with a dichotomous variable (in which there are only two possible outcomes). The goal of logistic regression is to 
find the best fitting model to describe the relationship between the dichotomous characteristic of interest 
(dependent variable = response or outcome variable) and a set of independent (predictor or explanatory) variables. This is better than 
other binary classification like nearest neighbor since it also explains quantitatively the factors that lead to classification.
<br>
The logistic function is a Sigmoid function, which takes any real value between zero and one. It is defined as <br>
![Img](https://miro.medium.com/max/192/1*xtIMx01jy4myAo1N8bbSCA.png)

<br>
And if we plot it, the graph will be S curve, <br>

![Graph](https://miro.medium.com/max/355/1*DmZ86NmgX2syazCKtkcJsA.png)

<br> <br>

## Naive Bayes Classification
A Naive Bayes classifier is a probabilistic machine learning model that’s used for classification task. The crux of the classifier is based on the Bayes theorem. <br>
#### Bayes Theorem:
![NB](https://miro.medium.com/max/510/1*tjcmj9cDQ-rHXAtxCu5bRQ.png) 

<br>
Using Bayes theorem, we can find the probability of A happening, given that B has occurred. Here, B is the evidence and A is the hypothesis. The assumption made here is that the predictors/features are independent. That is presence of one particular feature does not affect the other. Hence it is called naive. <br>

#### Types of Naive Bayes Classifier:
1. Multinomial Naive Bayes:
This is mostly used for document classification problem, i.e whether a document belongs to the category of sports, politics, technology etc. The features/predictors used by the classifier are the frequency of the words present in the document. <br>
2. Bernoulli Naive Bayes:
This is similar to the multinomial naive bayes but the predictors are boolean variables. The parameters that we use to predict the class variable take up only values yes or no, for example if a word occurs in the text or not. <br>
3. Gaussian Naive Bayes:
When the predictors take up a continuous value and are not discrete, we assume that these values are sampled from a gaussian distribution. <br>
![GNB](https://miro.medium.com/max/422/1*AYsUOvPkgxe3j1tEj2lQbg.gif)

<br>
Naive Bayes algorithms are mostly used in sentiment analysis, spam filtering, recommendation systems etc. They are fast and easy to implement but their biggest disadvantage is that the requirement of predictors to be independent. In most of the real life cases, the predictors are dependent, this hinders the performance of the classifier

## Support Vector Machine
“Support Vector Machine” (SVM) is a supervised machine learning algorithm which can be used for both classification or regression challenges. However,  it is mostly used in classification problems. In this algorithm, we plot each data item as a point in n-dimensional space (where n is number of features you have) with the value of each feature being the value of a particular coordinate. Then, we perform classification by finding the hyper-plane that differentiate the two classes very well.

<br>

![SVM](https://miro.medium.com/max/300/0*9jEWNXTAao7phK-5.png)

<br>

![SVM2](https://miro.medium.com/max/300/0*0o8xIA4k3gXUDCFU.png)

<br>

Hyperplanes are decision boundaries that help classify the data points. Data points falling on either side of the hyperplane can be attributed to different classes. Also, the dimension of the hyperplane depends upon the number of features. If the number of input features is 2, then the hyperplane is just a line. If the number of input features is 3, then the hyperplane becomes a two-dimensional plane. It becomes difficult to imagine when the number of features exceeds 3.

![SVM3](https://miro.medium.com/max/1418/1*ZpkLQf2FNfzfH4HXeMw4MQ.png) <br>
![SVM4](https://miro.medium.com/max/755/0*ecA4Ls8kBYSM5nza.jpg)

<br>

Support vectors are data points that are closer to the hyperplane and influence the position and orientation of the hyperplane. Using these support vectors, we maximize the margin of the classifier. Deleting the support vectors will change the position of the hyperplane. These are the points that help us build our SVM.
