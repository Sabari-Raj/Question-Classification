# Question-Classification
 Identify Question Type: Given a question, the aim is to identify the category it belongs to. The four categories to handle for this assignment are : Who, What, When, Affirmation(yes/no) and label any sentence that does not fall in any of the above four as "Unknown" type.
 
 First the data is in text format so I used pandas to create a table and separate the dependant and independant variable.
 Then used label encoder to convert the label into numerical form.
As the main part of question was to guess what kind of question it is, I used stopwords to keep the words like 'what', 'how', 'where' and removed the remaining words. 
Then split the dataset, with 20% being the test dataset.
Then for word vectorization ie to convert the text to numerical feature vectors, I used TF-IDF. This is an acronym that stands for “Term Frequency — Inverse Document” Frequency which are the components of the resulting scores assigned to each word.

Some of the most popular machine learning algorithms for creating text classification models include the naive bayes family of algorithms and support vector machines and here I tried both and I got the following accuracies


![rsz_1ml](https://user-images.githubusercontent.com/52276498/95874863-ff058100-0d8e-11eb-8660-442fd2752720.png)

Here as you can see the accuracy score of naive bayes is 89.22 while that of SVM is 94.94.Hence I later used SVM as its accuracy was more.

HOW TO RUN THE CODE

I used the Kaggle notebook, so just edit the path of the dataset (dataset file is uploaded as well) then just run.
