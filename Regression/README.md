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
