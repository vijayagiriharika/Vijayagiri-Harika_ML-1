## Machine Learning
## Important Machine Learning Algorithms

Good understanding of the following algorithms is required.

### Linear regression

We aim to predict a target variable using some given data variables. What we can do is to pass a line from the data set fitting the data set as shown.
To generalise, you draw a straight line such that it crosses through the maximum number of points. Once we have done that, we can predict the target value using that line as the hypothesis function.
<br/>![linear regression](https://www.researchgate.net/profile/Hieu_Tran33/publication/333457161/figure/fig3/AS:763959762247682@1559153609649/Linear-Regression-model-sample-illustration.ppm)<br/>
The only problem is how to define the values of slop and intercept of the line.
<br/>![linear regression intuition](https://miro.medium.com/max/656/1*4nBp-NeOFGBc-nNzP-VG3w.png)<br/>
We can use calculus to get the minimum values of slope and intercept such that the line passes through maximum number of points. More commonly, gradient descent is used for updating parameters at each step. [Gradient descent](https://machinelearningmastery.com/linear-regression-tutorial-using-gradient-descent-for-machine-learning/#:~:text=Gradient%20Descent%20is%20the%20process,downhill%20towards%20the%20minimum%20value.), [more details.](https://en.wikipedia.org/wiki/Linear_regression#:~:text=In%20statistics%2C%20linear%20regression%20is,is%20called%20simple%20linear%20regression.)
We will not go into detailed mathematics because this note just provides intuition for the algorithms.

### Polynomial Regression
Sometimes the line may not fit the data because of the data might have a high dimensional polynomial nature. So a line won't be enough. For this we need to increase the degee of attibutes (which can be done using the scikit-learn library).
Check the below figure for linear regression.
<br/>![linear regression](https://miro.medium.com/max/875/1*US9Nk7SxtBlwvAswpXehng.png)<br/>
As you can see in the figure, the given line can fit the data almost perfectly. Simple linear regression is fine in this case.
Now look at this figure.
<br/>![polynomial regression](https://miro.medium.com/max/875/1*MhTfu8jmERKpstkYCc7n3w.png)<br/>
The line for predicted speeds is not able to fit the ground truth perfectly. The data is too complex for simple linear regression to make predictions. We need to have high degree attributes.
Now look at this figure.
<br/>![polynomial regression](https://miro.medium.com/max/875/1*866wXGUKYkkwgguk3o-8Gg.png)<br/>
This hypothesis function fits the data almost perfectly. So to decide between linear and polynomial regression, you have to visualize the data. Use python's seaborn for better aid in visualization.
For detailed mathematics behind polynomial regression, [Click Here](https://en.wikipedia.org/wiki/Polynomial_regression)

### Random Forest Regression
First let's look at Ensemble Learning. Ensemble learning is a technique that combines the predictions from multiple weak machine learning algorithms together to make more accurate predictions. Since the model is comprised of many models, it is called an Ensemble model. Look at the image below for better understanding.
<br/>![ensemble](https://miro.medium.com/max/434/0*IsQCuCZCTX_zc7Xy.png)<br/>
Random forest is an supervised machine learning that can be used for classification and regression. It has trees which have no interaction in between them, they are completely independent from each other. Each tree acts as an independent model, which can be combined with others to form an ensemble. Each tree uses random data from the original data set when generating its splits, adding randomness to prevent overfitting. For many data sets, it produces a highly accurate classifier. It gives estimates of what variables that are important in the classification therefore, can be used for feature selection. It has an effective method for estimating missing data while maintaining accuracy.
<br/>![random forests](https://miro.medium.com/max/656/0*f_qQPFpdofWGLQqc.png)<br/>

### Support Vector Regression
SVM is one of the most powerful machine learning algorithm available today. A linear regression is only able to generate a line to predict the data points, while a support vector regression can also generate a hyperplane. In SVM, Margin is the perpendicular distance between the hyperplane and the closest points. SVM tries to maximise this margin, no penalty region in built by SVM in the muti dimensional data.
<br/>Look at the image.<br/>
![SVM](https://miro.medium.com/max/875/0*uwRVvFVLmKi3T9pS.png)<br/>
Making a hyperplane to fit this data is very difficult, specially it it's high dimensional. SVM does this task perfectly. SVR tries to have as many support vectors as possible within the margin, thus it keeps the error within the threshold.
A major difference between Linear regression and SVR lies on the fact that Linear regression tends to minimize the error and SVR tends to keep it within a threshold.
For further information visit [Sklearn SVR](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVR.html)<br/> <br/>

# Vijayagiri Harika
[<img align="left" alt="email" width="26px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/mail-dot-ru.svg"/>](mailto:vijayagiriharika7386@gmail.com) 

[<img align="left" alt="linkedin" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/linkedin.svg"/>](https://www.linkedin.com/in/vijayagiri-harika-1425a8201) 

[<img align="left" alt="GitHub" width="22px" src="https://raw.githubusercontent.com/github/explore/78df643247d429f6cc873026c0622819ad797942/topics/github/github.png" />](https://github.com/vijayagiriharika)

<br/>
