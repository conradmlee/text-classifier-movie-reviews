# Text Classifier: Movie Reviews
Training a text classifier that categorizes movie reviews from the Large Movie Review Dataset @ Stanford AI Lab.

## Introduction
We train a text classifier to categorize movie reviews from the Large Movie Review Dataset into "positive" and "negative" classes. This classifier primarily uses CountVectorizer (to tokenize and pre-process the text) and LogisticRegression (as a classifier). In addition, we plot a Confusion Matrix to visualize the results, and use GridSearchCV to find the best parameters.

## Data
Large Movie Review Database: http://ai.stanford.edu/~amaas/data/sentiment/

Andrew L. Maas, Raymond E. Daly, Peter T. Pham, Dan Huang, Andrew Y. Ng, and Christopher Potts. (2011). Learning Word Vectors for Sentiment Analysis. The 49th Annual Meeting of the Association for Computational Linguistics (ACL 2011).

## Steps
- 1) Data Loading
- 2) Preprocess text using CountVectorizer (from scikit-learn)
- 3) Apply the Vectorizer to the train data, fit a logistic regression, and compute the accuracy score
- 4) Concatenate the train and test data, and use GridSearchCV to optimize the C hyperparameter of the logistic regression

## References
I have forked and referenced from Jitendra Reddy's excellent Github repository online, primarily with regards to PyPrind (progress indicator feature) and the initial data loading loop. The title of the repository is "Movie Review Classifier."

- Link: https://github.com/g10draw/movie_review_classifier
