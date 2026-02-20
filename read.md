# Sentiment Analysis to Detect Mental Health Status


### Can mental health status or underlying mental illnesses be detected in text patterns? How we communicate often shows how we are feeling. This is a neural network designed to attempt to detect signs of anxiety, depression, suicidal thoughts, or normalcy in text messages. 
<br>

***
<br>

#### <u>Methods</u>: 
* I wanted to attempt to make my own custom model so I can implement the more optimized algorithms we learned in class. I read about FFN implementation as that is often used for classification and keeps some positionality. 
* vectorization: I used BPE as it more effectivly tokenizes text for the model to read. 
* embedding: I was able to encorperate an embedding step to attempt to have similar words put near each other, since for sentiment I want to know that bad, terrible, horrible etc. are related.
* dropout: I added a function called Dropout to help prevent overfitting in training as I don't have a very large amount of training data. 
* training: I used smaller batch training because I saw with large batches it was very slow and was getting stuck. The smaller batches helped it find the minimum faster and more accurately. <br>
<br>

***

####  <u>Key Results</u>: 
- In comparison to lab 1, my new model performed much better, with []

I believe that with using stronger encoders or models like BERT results could be better tuned for nuance, and also other illnesses. The training data is limited, and maybe some of the text isn't as expansive. With more time I could get more data from reddit or other sources and combine them for a larger breath of ways people talk. 

***
<br>

<u>How to Run</u>:
1. clone repository
2. open portfolio.ipynb in google colab or alternative
3. data is pulled through kaggle, link in jupyter notebook
4. run! everything is in the one file