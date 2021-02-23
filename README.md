# Group - Cobra Kai
Members:
George Simon, Patrick Leon, Fred Mansfield, Austin Hauck

## Introduction
Early in the project while searching for data, we stumbled across a dataset concerning Enron, an energy company who committed egregious valuation fraud and went bankrupt in the mid-2000's. In the end, we steered away from this dataset, but we decided we still wanted to work with a Natural Learning Processing (NLP) machine. We also wanted to make sure that we worked with Amazon Warehouse Systems to gain experience in a valuable field.
## Project Question
Therefore, we decided to apply our NLP machine to Amazon reviews, asking ourselves one main question:
Can we predict a review score based on wording alone?


______________________________
### DATA USED
* [Amazon Reviews - Link](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)
    * Chosen Dataset: *amazon_reviews_us_Tools*
    * Note: for the purpose of this project we upload the data to our own Amazon s3 cloud storage.

### AMAZON S3
#### Requirements
* AWS Profile
​
#### Description
Utilizing Amazon AWS we choose to store our datasets in the cloud [S3](https://docs.aws.amazon.com/AmazonS3/latest/dev/Welcome.html) to access in our Googe Collab coding notebooks. Below is a link to the instruction readme for set-up and some notes on the free amazon services provided.
[Link to instructions.md](setup-instructions/amazon-S3-setup.md)

## Front-End Development
______________________________
### TABLEAU
#### Requirements
* [Tableau Public Profile](https://public.tableau.com/en-us/s/)

#### Description
In order to set the stage and explore the Amazon Reviews Dataset Tableau Public was utlized.

Three vizzes were created to highlight different features of the data.
* Star Ratings Votes Over Time - *this chart also had Amazon's Stock Price overlayed*
* Votes Over Time
* Products with Helpful Reviews

All three of these vizzes can be found at the below Tableau Public link:
[Tableau Public Vizzes Link](https://public.tableau.com/views/Amazon_Review_Vis/StarRatingVotesOverTime?:language=en&:display_count=y&:origin=viz_share_link)

## Back-End Development
________________________________
## Machine Learning Insights
________________________________
#### Natural Language Processing
Once we chose that our project is focusing on Amazon reviews we knew we would need to use Natuarl Language Processing (NLP). A quick review of what NLP is the "automatic manipulation of natural language, like speech and text, by software" (Brownlee, MachineLearningMastery.com).
#### Initial findings
Using linear regression as our model of choice at first seemed to be the right path to take as we saw the ratio of average negative word count to average word count decrease as the star ratings went up but when applied to the machine no clear outcome arise.
When we ran our data using the IDF, negative word count, and the ratio with a small amount of data our output looked promising with an r-squared of 0.517. However when we increased the amount of rows to be ran our r-squared dropped to 0.146.
#### Linear Regression Hardships
Based on how we ran our NLP machine using Linear Regression, our outcome - the ability to predict the star rating of reviews from the amount of negative words - is inconclusive. If we were to do another NLP machine learning project, we would test more than one linear regression model. These models would start by using a Random Forest to select the best features to analyze; in our case we did not use this because the bulk of our usable data was text.
After that we would use models such has K-nearest neighbors, Support Vector Machines (SVM), and/or Naïve Bayes. These models would either group the data points closer or, redarding Naïve Bayes, would quantify the likelihood of the event happening based upon the kowledge that the event has occurred in the past.
