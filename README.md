# kaggle_fake_news_classifier_LSTM

## Problem Statetment

TO develop a machine learning model to identify when an article might be fake news, based in the training data provided

## Data Matrix

The Data matris is of the shape of (, 4)
Data matrix has columns namely:
 * title : title of the news story
 * author : author the story
 * text :  content of the story
 * label : target variable(classification of story whether fake or not)

## Data Preproessing and vectorinzing the model

### Tokeninzation
* Each story is tokenized using stem function of PorterStemmer object of nltk library
* The stem tokenization is used over lemmatization because stemming works bettern in news stories

## one-hot represenation of the model
* The stories are converted into one hot represenattion with voc-size 5000.
* So each word will be respresented a number between 0 and 5000

## Word embedding vectorization model and training 
* the data is vectorized using Embedding layer of keras
* the compiled deep learning model architecture is shown below 
![alt text](https://github.com/SHINE1607/kaggle_fake_news_classifier_LSTM/blob/master/images/model.png)



## Performance metrics and accuracy¶
validation score obtaiend is  : 0.9212924606462303
confusion matrix for validation data is shown below 
![alt text](https://github.com/SHINE1607/kaggle_fake_news_classifier_LSTM/blob/master/images/confusion_matrix.png)

Test data score obtained is: 0.92179








