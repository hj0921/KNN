#### KNN Examples
KNN is applied to:
1. Dating Web Data
2. Hand Written Digit Data

#### KNN Basic Theory
KNN is a supervised learning that does not have the learning process. This algorithm classify different classes based on the calculated distance between the classifying point and all the training points, and it only considers k nearest neighbors. Therefore, the magnitude of the K is important to this algorithm.

#### Three key points to KNN
##### How to choose the K:
Small K will cause the small approximation error (only similar train data will be viewed and be useful to the classification) but the large estimation error (too sensitive to nearby data, so noise will affect the classificaiton result a lot). A more complex model is gained, if k is smaller.

"Approximation Error: When forming predictive models, because we want a tractable problem, and because we do not want to over-fit to the data (see 3), we restrict our set of models to some family. For example, in ordinary least squares regression we typically restrict ourselves to a linear model with normal noise which has fixed variance. If the nature of the data generating mechanism does not follow these rules, even the best predictor in this family to which we've restricted ourselves will have more error than the Bayes predictor.

Estimation Error: Once we've restricted ourselves to some family of predictors, we must use our data to pick one predictor from that family. What if we do not choose the right one? Then we incur more error. To be clear, I am not referring to picking the wrong predictor by accident, but rather by statistical inference on a limited set of data."

Reference: https://stats.stackexchange.com/questions/87750/what-does-the-term-estimation-error-mean

近似误差，更关注于“训练”。最小化近似误差，即为使估计值尽量接近真实值，但是这个接近只是对训练样本（当前问题）而言，模型本身并不是最接近真实分布。换一组样本，可能就不近似了。这种只管眼前不顾未来预测的行为，即为过拟合。估计误差，更关注于“测试”、“泛化”。最小化估计误差，即为使估计系数尽量接近真实系数，但是此时对训练样本（当前问题）得到的估计值不一定是最接近真实值的估计值；但是对模型本身来说，它能适应更多的问题（测试样本）。

作者：KnowNothing
链接：https://www.zhihu.com/question/60793482/answer/248437399
来源：知乎

##### Distance Measure Method:
There are more method for the distance measuring, such as Euclidean distance, Minkowski Distance and Manhatton Distance. 

##### Decision Rule:
Voted mathod is applied to the KNN, so the class with higher vote will be the output class.




