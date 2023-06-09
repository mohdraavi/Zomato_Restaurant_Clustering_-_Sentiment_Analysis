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
**Zomato Restaurant metadata**
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

* Importing libraries
* Loading the dataset 
* Shape of dataset
* Dataset information 
* Understanding the columns
* Variable description
* Data wrangling
* Data visualization
* Story telling and experimenting with charts like wordcloud,heatmap,
* Data Preprocessing


 1. Missing values handling

  2. Duplicate values handling

  3. Outliers handling using isolation forest


  4. Categorical Encoding using one-hot encoding

  5. Textual data preprocessing
   
    a. Expand contraction

    b. Lower Casing

    c. Removing URL & digits

    d. Removing stop words and white spaces

    e. Rephrase text

    f. Tokenization

    g. Text normalization

    h. POS

    I. Text Vectorization

  6. Feature Manipulation & Selection
  7. Data Transformation
  8. Data Scaling
  9.Dimensionality Reduction using pca
  10.Data Splitting
  11. Imbalanced Class Handling
* clustering
* Sentiment analysis
* Conclusion.



ALGORITHMS:

1.K-Means Clustering

unsupervised machine learning algorithm used for clustering data points into groups or clusters based on their similarity. The goal of K-means clustering is to divide a dataset into K distinct clusters, where each data point belongs to the cluster with the nearest mean value.

2.Logistic Regression


Logistic regression is a statistical model that in its basic form uses a logistic function to model a binary dependent variable, although many more complex extensions exist. In regression analysis, logistic regression (or logit regression) is estimating the parameters of a logistic model (a form of binary regression).


4.Xgboost:(Ensemble technique based on boosting)

XGBoost is based on the concept of gradient boosting, which involves building an ensemble of weak prediction model and iteratively improving their predictions by minimizing a loss function through gradient descent.


Model Performance:



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
