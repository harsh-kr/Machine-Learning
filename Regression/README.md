# Linear Regression
Linear Regression is a machine learning algorithm based on supervised learning. It performs a regression task. Regression models a target
prediction value based on independent variables. It is mostly used for finding out the relationship between variables and forecasting.
Different regression models differ based on – the kind of relationship between dependent and independent variables, they are considering
and the number of independent variables being used.
<br><br>
![ML LinReg](https://www.onclick360.com/wp-content/uploads/2018/12/linear-regression.jpg)
<br><br>
Linear regression is a linear model, e.g. a model that assumes a linear relationship between the input variables (x) and the single output
variable (y). More specifically, that y can be calculated from a linear combination of the input variables (x).
<br>
When there is a single input variable (x), the method is referred to as simple linear regression. When there are multiple input variables,
literature from statistics often refers to the method as multiple linear regression.
<br>
Different techniques can be used to prepare or train the linear regression equation from data, the most common of which is called Ordinary
Least Squares. It is common to therefore refer to a model prepared this way as Ordinary Least Squares Linear Regression or just Least
Squares Regression.
<br><br>
Linear regression equation looks like this: <br>
![Linear Reg](https://s3.amazonaws.com/thinkific/file_uploads/118220/images/734/0a4/d4c/1548919480093.jpg)
<br>
Here, we have Y as our dependent variable (Sales), X’s are the independent variables and all thetas are the coefficients. Coefficients
are basically the weights assigned to the features, based on their importance. For example, if we believe that sales of an item would have
higher dependency upon the type of location as compared to size of store, it means that sales in a tier 1 city would be more even if it is
a smaller outlet than a tier 3 city in a bigger outlet. Therefore, coefficient of location type would be more than that of store size. So, 
for linear regression with only one feature, i.e., only one independent variable, our equation becomes, <br>
![Linear Reg](https://s3.amazonaws.com/thinkific/file_uploads/118220/images/99f/9b9/a82/1548919484765.jpg)
<br> This equation is called a simple linear regression equation, which represents a straight line, where ‘Θ0’ is the intercept, 
‘Θ1’ is the slope of the line. <br><br>
![Image](https://sebastianraschka.com/images/faq/closed-form-vs-gd/simple_regression.png)
<br>
<br>
# Polynomial Regression
What happens if we know that our data is correlated, but the relationship doesn’t look linear? So hence depending on what the data looks like, we can do a polynomial regression on the data to fit a polynomial equation to it. <br>
![Lin Reg](https://miro.medium.com/max/500/1*xz_haBuJRSI2DaveNk-3gw.gif)
<br>
Hence If we try to use a simple linear regression in the above graph then the linear regression line won’t fit very well. It is very difficult to fit a linear regression line in the above graph with a low value of error. Hence we can try to use the polynomial regression to fit a polynomial line so that we can achieve a minimum error or minimum cost function. The equation of the polynomial regression for the above graph data would be: <br>
y = θo + θ₁x₁ + θ₂ x₁² <br><br>
This is the general equation of a polynomial regression : <br>
Y=θo + θ₁X + θ₂X² + … + θₘXᵐ + residual error <br>
![Poly Reg](https://miro.medium.com/max/500/1*Cat1swI8xmNYui6w5AYp8A.gif)
<br> <br>
# Support Vector Regression
Support Vector Machine can be applied not only to classification problems but also to the case of regression. Still it contains all the main features that characterize maximum margin algorithm: a non-linear function is leaned by linear learning machine mapping into high dimensional kernel induced feature space. The capacity of the system is controlled by parameters that do not depend on the dimensionality of feature space.In simple regression we try to minimise the error rate. While in SVR we try to fit the error within a certain threshold. <br>
The terms related to SVR that one should know are :
1. Kernel: The function used to map a lower dimensional data into a higher dimensional data.
2. Hyper Plane: In SVM this is basically the separation line between the data classes. Although in SVR we are going to define it as the line that will will help us predict the continuous value or target value
3. Boundary line: In SVM there are two lines other than Hyper Plane which creates a margin . The support vectors can be on the Boundary lines or outside it. This boundary line separates the two classes. In SVR the concept is same.
4. Support vectors: This are the data points which are closest to the boundary. The distance of the points is minimum or least.
<br>

![SVR](https://miro.medium.com/max/512/1*fVCEP_qxSWYwKcpkt2Xk2w.png)

<br>
All the points are within the boundary line(Red Line). Our objective when we are moving on with SVR is to basically consider the points that are within the boundary line. Our best fit line is the line hyperplane that has maximum number of points.
<br> <br>

# Decision Tree Regression

![DTReg](https://acadgild.com/blog/wp-content/uploads/2018/09/Decision-tree.jpg)

<br>

### What is CART? <br>
CA - Classification Trees <br>
RT - Regression Trees <br> <br>
### What kind of linear regression is Decision Tree Regression? <br>
Non-linear regression <br><br>
### What is the default criterion for Decision Tree Regression class? <br>
Default criterion is MSE (Mean Square error). MSE = the square difference b/w the prediction and the real result and taking the sum of these differences to measure the error. <br> <br>
### What kind of model is Decision Tree Regression model falls into? <br>
Non-continuous model <br> <br>
### Why do we need to plot with high resolution data set for visualizing Decision Tree Regression? <br>
In Decision Tree Regression, the predicted values are obtained as per the average of that particular interval. Thus, without a high resolution, the plot would not show the actual representation of the fact that the prediction is based on averages in that particular interval. <br> <br>
### Will Decision Tree Regression best suit for 1D models or 2D models? <br> 
Decision Tree Regression models are best suited for 2D models. <br> <br>

![DTreg](https://miro.medium.com/max/700/1*Oln4_uIkjKd-wAyL3a-upw.png)

![DTreg2](https://miro.medium.com/max/700/1*Xb_S8tBQ_CZbyfd_7duaAQ.png)

![DTreg3](https://miro.medium.com/max/700/1*IEJReGjY_hC1DslXZ7kZFg.png)

![DTreg4](https://miro.medium.com/max/700/1*hF572qULmK0_xA37tujkYg.png)
