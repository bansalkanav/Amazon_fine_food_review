# Amazon_fine_food_review
## Introduction
The Amazon Fine Food Reviews dataset consists of 568,454 food reviews. This dataset consists of a single CSV file, Reviews.csv

<b>Data Set</b><br />
<a href="https://www.kaggle.com/snap/amazon-fine-food-reviews">Click here</a> to get the dataset.<br />
<pre>Review.csv - 251MB</pre>

<b>Dataset statistics</b>
<pre>
    Number of reviews     568,454
    Number of users     256,059
    Number of products     74,258
    Users with > 50 reviews     260
    Median no. of words per review     56
    Timespan     Oct 1999 - Oct 2012
</pre>

<b>Data Fields Explanation</b>
<pre>
    Id - Unique row number
    ProductId - unique identifier for the product
    UserId - unqiue identifier for the user
    ProfileName
    HelpfulnessNumerator - number of users who found the review helpful
    HelpfulnessDenominator - number of users who indicated whether they found the review helpful
    Score - rating between 1 and 5
    Time - timestamp for the review
    Summary - brief summary of the review
    Text - text of the review
</pre>

## EDA Objective

Analysing the data & plot the required graphs to show that these conclusions are true:
<pre>
a. Positive reviews are very common.
b. Positive reviews are shorter.
c. Longer reviews are more helpful.
d. Despite being more common and shorter, positive reviews are found more helpful.
e. Frequent reviewers are more discerning in their ratings, write longer reviews, and write more helpful reviews
</pre>
<b>Note:</b> This notebook is highly inspired from the <a href="http://blog.nycdatascience.com/student-works/amazon-fine-foods-visualization/">Exploratory visualization of Amazon fine food reviews by Rob Castellano.</a>

## Model Building
<pre>
    STEP-1: Copy the data in Pandas DataFrame and drop unwanted columns.
    STEP-2: Text Preprocessing.
            a. Converting to lower-case.
            b. Removing HTML Tags.
            c. Removing Special Characters.
            d. Removing Stop Words.
            e. Stemming (Snowball Stemming)
    STEP-3: Vectorizing out Data Set
    STEP-4: Building and evaluating the model
            a. Naive Bayes
            b. Logistic Regression - with L1 and L2 regularizors
            c. Linear SVM
            d. RBF Kernel SVM 
</pre>
