# wyj

In this project, The dataset that we used was’ breast cancer-wisconsin ’, which can be download at https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/breast-cancer-wisconsin.data. There are 698 samples in this data, each samples has 9 features and 1 target variable ‘Class’. A total of five machine learning methods were selected, namely: Decision Tree Classifier, Logistic Regression, SGD Classifier, Linear SVC, K-Neighbors Classifier. 


## **Decision Tree Classifier**
Decision tree is a prediction model; It represents a mapping between object attributes and object values, Each node in the tree represents an object, and each fork path represents a possible property value, Each leaf is the value of the object represented by the path from the root node to the leaf. Decision tree is the best choice to describe nonlinear relationship.
## Linear classification model
Linear classification model is to make classification decisions through the linear combination of features to achieve the purpose of prediction. 
## LinearSVC
Support vector machine (SVC) is a class of generalized linear classifiers that classify data binary according to the supervised learning method. Its decision boundary is the maximum margin hyperplane for solving the learning sample. 
## K-Neighbors Classifier
k-Nearest Neighbor is: in the eigenspace, if most of the k nearest (that is, the closest) samples near a sample belong to a certain category, the sample also likely belongs to this category

# project process
1. After importing packages, we used pd.read_csv() to read datasets, and we used data.head() and data.info() to check whether the data was read correctly.Then, we set the head for the data set and removed any missing data.
2. We ues StandardScaler to standardize the features because the accuracy of the fit results was improved when it was standardized.
3. We use train_test_split function to Divide the dataset，20% of the dataset as testset and 80% of the dataset as training set. 
4. We preprocess the dataset to eensure the mean of each dimension of the data is 0 and the variance is 1. 
5. We trained the dataset in five ways, and used the data from the test set to make the prediction and store the data in y_Pred. 

# Interpretation of result
The following table shows the accuracy and r2-score of several algorithms：

The accuracy of each algorithms:

![avatar](https://github.com/wyj-01/wyj/blob/main/准确率.png)

The r2-score of each algorithms:

![avatar](https://github.com/wyj-01/wyj/blob/main/R2.png)

