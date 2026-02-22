# Sentiment Analysis to Detect Mental Health Status


### Can mental health status or underlying mental illnesses be detected in text patterns? How we communicate often shows how we are feeling. This is a neural network designed to attempt to detect signs of anxiety, depression, suicidal thoughts, or normalcy in text messages. 

***

###  <u>Key Results</u>: 

After training my model, it was determined to be just over 76% accurate. While I was hoping for higher, with it being a small model I made, and the training data not being as robust as I would have wished, it is a large improvement to lab 1 results! While my sentiment model still is having trouble detecting anxiety, it has greatly improved picking out suicidal ideation and depression and normal. I think that with more training data with diverse examples of anxiety, and a more detailed model would improve the score. 

***

### <u>Methods</u>: 
* I wanted to attempt to make my own custom model so I can implement the more optimized algorithms we learned in class.
* vectorization: I used BPE as it more effectivly tokenizes text for the model to read. 
* embedding: I was able to incorporate an embedding step to attempt to have similar words put near each other, since for sentiment I want to know that bad, terrible, horrible etc. are related.
* dropout: I added a function called Dropout to help prevent overfitting in training as I don't have a very large amount of training data. 
* training: I used smaller batch training because I saw with large batches it was very slow and was getting stuck. The smaller batches helped it find the minimum faster and more accurately. <br>
<br>

***

### How to Run:
1. clone repository
2. open sentiment_model_work.ipynb in google colab or alternative
3. data is pulled through kaggle, link in jupyter notebook
4. run! everything is in the one file

### Requirements:
| Library | Version |
|---|---|
| pandas | 2.2.2 |
| numpy | 2.0.2 |
| matplotlib | 3.10.0 |
| scikit-learn | 1.6.1 |
| sentence-transformers | 5.2.3 |
| tokenizers | 0.22.2 |
| torch | 2.10.0+cpu |
| kagglehub | 0.3.13 |
