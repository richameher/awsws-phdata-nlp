# Amazon Review Analysis
To predict whether an Amazon product review is negative and do a deeper dive into what causes negative reviews.

# Datasets
Amazon review dataset: https://s3.amazonaws.com/fast-ai-nlp/amazon_review_polarity_csv.tgz
The dataset determines that a review score of 1 and 2 is negative, and 4 and 5 is positive (on a scale of 5 stars). Samples of score 3 are ignored.
In the dataset, the labels are as follows: class 1 is the negative and class 2 is the positive. 
Each class has 1,800,000 training samples and 200,000 testing samples.
The fields in the raw data include the title and review text.

# End Goal
The data is given to us already classified as a negative or positive review. Our first goal is to filter on the negative reivews and run a small sample on Amazon Comprehend to receive it's estimatation of five distinct topic groupings.
After analyzing the newly grouped topics, we formed our own name for each topic and declare those as labels on the sampled data. Then we train a blazing text classifier to predict the labels (topics) on the remaining negative labels.
