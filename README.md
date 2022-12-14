# Restaurant-Sentiment-Analysis-with-Gaussian-Naive-Bayes--XGBoost-and-Neural-Network

## Executive Summary  

#### About Data:  

* I used Restaurant Review dataset where can be downloaded from Kaggle.  
* Dataset type is tsv, so the data was seperated with 'tab'. 
* Dataset has 900 entry and 2 columns which are called 'Review' and 'Liked'.  

#### Preprocessing the dataset  

* Removed the stopwords from Review statements 
* Used Porter Stemmer for finding their root. 
* Removed any punctuation and transformed lowercase all words. 
* Transformed the words into the numeric value by usin CountVectorizer.  

#### Build the Models  

* Gaussian Naive Bayes, XGBoost and Neural Network was used in this project. 
* Confusion matrix and Classification Report were used to evaluate the model. 
* Neural Network was designed with one input, two hidden layer and one output layer. 
* ReLu and Sigmoid activation functions were used. * Adam optimizer was used and Binary Cross Entropy was used as a loss function. 
* 8 epochs and 35 batch size were used to train the dataset. (I tried with 16 epochs but this caused overfitting. So, I decrease the epochs gradually and the best epochs is 8.)  

#### Evaluate the Models  

* Gaussian Naive Bayes has 0.73 accuracy, XGBoost 0.72, and Neural Network 0.78 accuracy score. 
* Also, Gaussian Naive Bayes F1 Score is 0.72, XGBoost 0.74, and Neural Network 0.82 F1 Score. 
* All in all, Neural Network is realiable model. It can be used to classify the Review Sentences.
