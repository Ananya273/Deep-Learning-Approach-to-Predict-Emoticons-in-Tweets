# Emoticon prediction in twitter with Bidirectional LSTM
This project aims to predict the emoticon a user would use for a tweet. We study the sentiment of a sentence and do a multi class classification to assign it an emoticon.

**Datasets**

* train.csv
  * Unnamed-0- row number
  * TEXT- tweet
  * Label- emoticon (number mapping to the corresponding emoticon)
  
* mapping.csv
  * Unnamed-0- row number
  * emoticons- emoticon
  * number- number used to create the map between train.csv and mapping.csv
  
* test.csv (same columns as train.csv)

**Exploratory Data Analysis**

  * Used different data visualization techniques to get more insights into the data using Matplotlib and Seaborn packages
  
  * Created a dictionary to generate mapping between the emoticons and labels that helps in preprocessing of the data.
   
**Data Preprocessing**

  * Used `TweetTokenizer` to tokenise sentenences
  
  * Used `Glove package` by Stanford NLP group for word embeddings
  
  * Performed `SMOTE` to take care of the imbalanced data set
  
**Training the model**

  * Used `Bidirectional LSTM` to train using `keras`.
  
  * Used three hidden layers with `ReLU` activation functions,  `softmax` function and `adam` optimiser.
  
 *Accuracy obtained is 82.26 percent*
  
  
  
