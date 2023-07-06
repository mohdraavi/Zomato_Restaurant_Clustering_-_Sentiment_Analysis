# Zomato_Restaurant_Clustering_-_Sentiment_Analysis
Problem Statement:
The Project focuses on Customers and Company, you analyzed the sentiments of the reviews given by the customer in the data and made some useful conclusion in the form of Visualizations. Also, cluster the zomato restaurants into different segments. The data is vizualized as it becomes easy to analyse data at instant. The Analysis also solve some of the business cases that can directly help the customers finding the Best restaurant in their locality and for the company to grow up and work on the fields they are currently lagging in.

This could help in clustering the restaurants into segments. Also the data has valuable information around cuisine and costing which can be used in cost vs. benefit analysis

Data could be used for sentiment analysis. Also the metadata of reviewers can be used for identifying the critics in the industry.

Datasets: In this analysis we have used the following datasets.
**1.Zomato Restaurant Reviews dataset**
**1.Zomato Restaurants metedata dataset**

Data gives us the following features:
**Attributes ▶**

---
**Zomato Restaurant**
* Name : Name of Restaurants

* Links : URL Links of Restaurants

* Cost : Per person estimated Cost of dining

* Collection : Tagging of Restaurants w.r.t. Zomato categories

* Cuisines : Cuisines served by Restaurants

* Timings : Restaurant Timings

**Zomato Restaurant Reviews**
* Restaurant : Name of the Restaurant

* Reviewer : Name of the Reviewer

* Review : Review Text

* Rating : Rating Provided by Reviewer

* MetaData : Reviewer Metadata - No. of Reviews and followers

* Time: Date and Time of Review

* Pictures : No. of pictures posted with review

Steps involved:

Exploratory Data Analysis:

After loading the datasets, various analysis was performed by comparing our target variable CHD with other independent variables. We performed various analysis like feature engineering, feature transformation, handling outliers, analyzing categorical and numerical data, Understanding important features, etc.

Feature Engineering:

1)Handling missing values:

While exploring our project we keep in mind to handle missing values and fill them with their respective mean and modes.

2)Duplicate values treatment:

There were no duplicate values in our dataset

3)Outliers:

Outliers plays an important role for any machine learning project. In our project we had outliers at certain attributes. Instead of deleting them we imputed the outliers.

EDA Visualization:

EDA Visualization is performed by using seaborn libraries with various plots like histogram, violin plot, bar plot, etc. We have used these plots for describing correlations, for relationship of sex and person who is smoking or not, other attributes and their affect on target variable CHD. Visualizations comes in handy to do Univariate-variate and multi-variate analysis.

Label Encoding:

Machine Learning is performed only on numerical values, so there might be some column which do not have numerical values. Label Encoding is a popular encoding technique for handling categorical variables. In this technique, each label is assigned a unique integer based on alphabetical ordering. We performed this technique on attributes sex and is smoking.

Feature Selection:

Feature selection or variable selection is the process of selecting a subset of relevant features or variables from the total features of a level in a data set to build machine learning algorithms.

Advantages of selecting features:

There are various advantages of feature selection process. These are as follows:

Improved accuracy

Simple models are easier to interpret.

Shorter training times

Enhanced generalization by reducing Overfitting

Easier to implement by software developers

Reduced risk of data errors by model use

Variable redundancy

Bad learning behaviour in high dimensional spaces

Feature Splitting and Scaling

Feature splitting and scaling were done using variance threshold and chi-square tests which gave us better idea of our attributes and helped eliminating additional features.

Balancing target Variable

Since our target variable CHD was unbalanced, we used SMOTE to balance it.

SMOTE (Synthetic Minority Oversampling Technique) consists of synthesizing elements for the minority class, based on those that already exist. It works randomly picking a point from the minority class and computing the k-nearest neighbors for this point. The synthetic points are added between the chosen point and its neighbors.

ALGORITHMS:

1.K-Means Clustering

2.Logistic Regression

3.Xgboost


1.Logistic Regression:(With and Without Hyper-parameter Tunning)

Logistic regression is a statistical model that in its basic form uses a logistic function to model a binary dependent variable, although many more complex extensions exist. In regression analysis, logistic regression (or logit regression) is estimating the parameters of a logistic model (a form of binary regression).

2.K-nearest Neighbour: (With and Without Hyper-parameter Tunning)

The k-nearest neighbors (KNN) algorithm is a simple, supervised machine learning algorithm that can be used to solve both classification and regression problems. It's easy to implement and understand, but has a major drawback of becoming significantly slows as the size of that data in use grows.

3.Decision Tree: (With and Without Hyper-parameter Tunning)

Decision trees help you to evaluate your options. Decision Trees are excellent tools for helping you to choose between several courses of action. They provide a highly effective structure within which you can lay out options and investigate the possible outcomes of choosing those options.

4.Xgboost:(Ensemble technique based on boostingfbtos                                 e)

A Random Forest is a reliable ensemble of multiple Decision Trees (or CARTs); though more popular for classification, than regression applications. Here, the individual trees are built via bagging (i.e., aggregation of bootstraps which are nothing but multiple train datasets created via sampling of records with replacement) and split using fewer features. The resulting diverse forest of uncorrelated trees exhibits reduced variance; therefore, is more robust towards change in data and carries its prediction accuracy to new data. However, the algorithm does not work well for datasets having a lot of outliers, something which needs addressing prior to the model building.

Model Performance:

Logistic Regression:

For logistic regression the accuracy was 85.84 which increased to 85.98 after hyper parameter Tunning.

K-nearest Neighbors:

For K- nearest neighbors the accuracy was 84.36 which increased to 85.69 after hyper parameter Tunning.

Decision Tree:

For Decision Tree the accuracy was 74.92 which increased to 85.69 after hyper parameter Tunning.

Random Forest Classifier:

For Random Forest Classifier the accuracy was 84.80.

Conclusion:
Clustering and sentiment analysis were performed on a dataset of customer reviews for the food delivery service Zomato. The purpose of this analysis was to understand the customer's experience and gain insights about their feedback.

The clustering technique was applied to group customers based on their review text, and it was found that the customers were grouped into two clusters: positive and negative. This provided a general understanding of customer satisfaction levels, with the positive cluster indicating the highest level of satisfaction and the negative cluster indicating the lowest level of satisfaction.

Sentiment analysis was then applied to classify the review text as positive or negative. This provided a more detailed understanding of customer feedback and helped to identify specific areas where the service could be improved.

Overall, this analysis provided valuable insights into the customer's experience with Zomato, and it could be used to guide future business decisions and improve the service. Additionally, by combining clustering and sentiment analysis techniques, a more comprehensive understanding of customer feedback was achieved. 

Other important discoveries during analysis are - 
* AB's - Absolute Barbecues, show maximum engagement and retention as it has maximum number of rating on average and Hotel Zara Hi-Fi show lowest engagement as has lowest average rating.

* Price point for high rated hotel AB's= Absolute Barbecues is 1500 and price point for low rated restaurant Hotel Zara Hi-Fi is 400.

* North Indian food followed by chinese are best or indeemand food as sold by most of the restaurants.

* Great Buffets is the most frequently used tags and other tags like great, best, north, Hyderabad is also used in large quantity.

* Satwinder singh is the most popular critic who has maximum number of follower and on an average he give 3.5 rating.

* restaurant Collage - Hyatt Hyderabad Gachibowli is most expensive restaurant in the locality which has a price of 2800 for order and has 3.5 average rating. Hotels like Amul and Mohammedia Shawarma are least expensive with price of 150 and has 3.9 average rating.

Some recommendation based on the analysis ▶
* Based on negative reviews like some focused on issues with delivery time or food quality, the company should prioritize addressing these issues to imporve customer satisfaction.

* Based on the clustering, or user interaction customer should be given recommendations.

* Also use the clustering results to target specific customer segments and tailor marketing and promotional efforts accordingly.

Challenges Faced:

We have outliers in our dataset which accounts for 14% of data. So instead of discarding them we chose to impute them with median values of respective features.

We have 2 categorical features as string type which we labelled using label encoding.

We have so many features irrelevant for our model so we Adjust them like putting id feature as index and Those which have multicollinearity and values lower than variance threshold, we discarded them from our model.

Our target feature was highly Imbalanced. So, we use SMOTE to balance it before training.

Some computations were complex and had to be done correctly since wrong computations would have led to loss of data.
