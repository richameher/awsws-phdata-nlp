# Amazon Review Sentiment Analysis
To predict whether an Amazon product review is negative and why it's negative.

# Datasets
Amazon review dataset: https://s3.amazonaws.com/fast-ai-nlp/amazon_review_polarity_csv.tgz
Review score 1 and 2 as negative, and 4 and 5 as positive. Samples of score 3 is ignored. 
In the dataset, class 1 is the negative and class 2 is the positive. 
Each class has 1,800,000 training samples and 200,000 testing samples.
The fields in the raw data include the title and review text.

# End Goal
The data is given to us already classified as a negative or positive review. Our first goal is to filter on the negative reivews and run a small sample on Amazon Comprehend to get topics. After understanding the topics, we pick the top n topics and apply those labels on that data. Then we train a classifier to predict the labels (topics) on the remaining negative labels. 
