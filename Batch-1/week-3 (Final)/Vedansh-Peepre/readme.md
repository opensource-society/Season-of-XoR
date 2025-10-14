this is finl readme
challenges faced, complete description, resources used, how to use?

## complete description
Hey! this is my **Sentiment analysis** project, trained on 1.6 million tweets dataset from kaggle.

It tells the sentiment behind tweets -whether it is positive(1) or negative(0).

Dataset - Sentiment140 tweets dataset <br>
Data pre-processing - using PorterStemmer function <br>
Vectorizer - used Tfidf vectorizer <br>
Model - A basic LogisticRegression model <br>

Resources used-
1. GeeksForGeeks tutorial of Tweets Sentiment Analysis
2. Google Colab for the entire code notebook
3. Kaggle for dataset

## how to use the model
1. download the `trained_model.sav` file
2. run the following commands for loading the model <br>
   ```
   loaded_model = pickle.load(open('<PATH>', 'rb')) 
   ```
   replace `<PATH>` with the path of the `trained_model.sav` file that you''ve downloaded
3. use the following code for using the model
   ```
   print(X_test[200])

   X_new = X_test_vec[<num>]
   print('Actual value =', Y_test[<num>])

   prediction = loaded_model.predict(X_new)
   print(prediction)

   if (prediction[0] == 0):
     print('The tweet is negative')
   else:
     print('The tweet is positive')
   ```
   replace the `<num>` with any number, say 200

## challenges faced
it was great working on this project, i've gathered some really good ground knowledge on python libraries, machine learning models & how to train them, and working on a project all-in-all. <br>
but it would be false to say that i haven't faced any challenges, conversation over -here's the list!
1. struggling with Google Colab's free tier limitations. as the ml and stemming works took time, i had a salty time managing runtimes and constantly keeping the tab and pc screen on
2. managing time. with my college works (assignments, tests) and other commitments, i had to assign the nights for this

But all of them were successfully overpowered at the end, and here's the submission

```
NOTE: this project is not available in GUI format, to test the model, we'll have to run the commands in a python file / notebook
```
