# Next-Word-Prediction-using-Deep-Learning
Next Word Prediction (also called Language Modeling) is the task of predicting what word comes next. Given three words of a sentence, it should predict next word. I am using LSTM (Long-Short Term Memory) here. Note: LSTM comes under Recurrent Neural Network (RNN) architecture used in the field of deep learning. A common LSTM unit is composed of a cell, an input gate, an output gate and a forget gate.

![image](https://user-images.githubusercontent.com/76472345/201672814-93012ec8-6a88-4ad2-b278-5f78d0db3a4e.png)
Application Language Modelling
1) Mobile keyboard text recommendation
 ![image](https://user-images.githubusercontent.com/76472345/201672937-09c5f1d3-c1a9-459a-a154-9c592d43f7c3.png)

2) Whenever we search for something on any search engine, we get many suggestions and, as we type new words in it, we get better recommendations according to our searching context. So, how will it happen???
 ![image](https://user-images.githubusercontent.com/76472345/201672978-7d66d09a-239c-48ec-bcad-343ba6fc3cbd.png)

It is possible through LSTM (Long short-term memory) model that will predict next words of sentence.


# The working of our project is:-
1)	Firstly, we import libraries for training and building models.
2)	Now, we will upload files in google colab python.
3) Data cleaning using regular expressions, stop words removal, lemmatization.
4) Then, we will apply tokenization and made some other changes and storing it in token.pkl
5) Also, we did conversion of string/text into numeric representation and we also this sequence data for input text and output word id and stored in empty list. 
6) we now convert this list into array and then, divide input and output word id. 
7)Now, we convert class vectors to binary class matrix for using loss function as categorical cross entropy.
8) Now, we create model sequence of neural network and define embedded layer, BI-LSTM layer and BI-Dense layer.
9) Now, we train model and saving each checkpoint in next_words.h5 and stores best fit model and evaluate weighs at each interval. Also, we use epochs for fitting model and optimizer Adam() for compiling and better learning of model at each iteration.
10) Now, we load model and tokenizer file for prediction.
11) we define Predict_next_words() function ,where, we convert text into  array using sequence and then, use argmax to return max value .
12) later, we iterate each item of dictionary that are in tokenizer file.


