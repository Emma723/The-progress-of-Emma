# The-progress-of-Emma
There is the repository where restores R language learning process by Emma. 
I just learned how to change the commit on Github, and I just knew that the edit process on Github named commits.

# It is my first time to use Github to record the interesting process of how to use R to manage practical probelms

1) How to get a linear regresstion fuction and how to access the accuracy of a linear regression model.
I pratice the above process by using R, with the example of the IBM human attribution.

Firstly, I use the exercise to markdown the learning process of R language
# linear regression (with the example of the dataset of statistical learning)
library(MASS)
library(ISLR)
fix(Boston)
names(Boston)
lm.fit = lm(tax~medv,data = Boston)
attach(Boston)
lm.fit = lm(tax~medv)
summary(lm.fit)

confint(lm.fit) # get the confidence interval of the linear fuction

# The difference between confidence interval and prediction interval
The prediction interval compute the interval of several specifically predictors, but the confidence interval is focused on the whole data set of the predictors.
# There may be some different between using the confidence interval and prediction interval
predict(lm.fit, data.frame(medv=(c(2,8,3)),interval = "confidence"))
predict(lm.fit, data.frame(medv=c(2,8,3),interval ="prediction")

confint(lm.fit)


