# Text Classifier: Movie Reviews
Training a text classifier that categorizes movie reviews from the Large Movie Review Dataset @ Stanford AI Lab (Python).

# Goal
Train a text classifier that categorizes movie reviews in "positive" and "negative".

# Data
Large Movie Review Database: http://ai.stanford.edu/~amaas/data/sentiment/

Andrew L. Maas, Raymond E. Daly, Peter T. Pham, Dan Huang, Andrew Y. Ng, and Christopher Potts. (2011). Learning Word Vectors for Sentiment Analysis. The 49th Annual Meeting of the Association for Computational Linguistics (ACL 2011).

# Steps
- Step 1: Read all the text files from aclImdb/train/pos/ and aclImdb/train/neg/ into a pandas DataFrame called train with two columns: review (the text itself) and sentiment (positive or negative). Do the same thing with aclImdb/test and save it to a different DataFrame. If the dataset is too large for your machine, use a sample. (Hint: Use the glob module) (2 points)
- Step 2: Preprocess the text using CountVectorizer or TfidfVectorizer from scikit-learn, adding a preprocessor that removes spurious 
tags from the text, or alternatively removing them from the dataframes beforehand (1 point)
- Step 3: Apply the Vectorizer to the train data, fit a logistic regression, and compute the accuracy score (1 point)
- Step 4: Concatenate the train and test data, and use GridSearchCV to optimize the C hyperparameter of the logistic regression (1 point)

# References
I have forked and referenced from Jitendra Reddy's excellent Github repository online, primarily with regards to PyPrind (progress indicator feature) and the initial data loading loop. The title of the repository is "Movie Review Classifier."
Link: https://github.com/g10draw/movie_review_classifier
