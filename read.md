# Sentiment Analysis to Detect Mental Health Status

Can mental health status or any underlying illnesses be detected in text patterns? This is a neural network designed to attempt to detect signs of anxiety, depression, suicidal thoughts, or normalcy in text messages. 

<u>Methods</u>: I used BPE for vectorization as it more effectivly splits text for models to read. I built my own model using ReLU and Dropout to make sure each layer is normalized and prevent overfitting. I used batch training as the original set of data kept causing my model to get stuck, so smaller groups for training helped it find the minimum. 

<u>Key Results</u>: In comparison to lab 1, my new model performed much better, with []

I believe that with using stronger encoders or models like BERT results could be better tuned for nuance, and also other illnesses. The training data is limited, and maybe some of the text isn't as expansive. With more time I could get more data from reddit or other sources and combine them for a larger breath of ways people talk. 


<u>How to Run</u>:
1. clone repository
2. open portfolio.ipynb in google colab or alternative
3. data is pulled through kaggle, link in jupyter notebook
4. run! everything is in the one file