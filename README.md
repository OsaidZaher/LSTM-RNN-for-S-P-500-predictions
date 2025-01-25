An S&P 500 Long Short-Term Memory recurrent neural network. 
Due to data shuffling and batching, you get different Mean Absolute Error, Mean Squared Error, and Root Mean Squared Error. I tried to combat this by creating a constant seed for tensorflow and numpy and setting deterministic operations.
The model performs well with an MAE of sub 80 and my recent commit was sub 70.

To give credit to how I created the model, I was inspired to do this after finishing "Hands-On Machine Learning with Scikit-Learn, Keras, and Tensorflow: Concepts, Tools, and Techniques to Build Intelligent" by  Aurélien Géron. 
I continuously referenced Chapter 15 (Processing sequences using Rnns and Cnns) to split and process the time series data and create the RNN.
I went back to Chapter 11 (Training Deep Neural Networks) to fine-tune the hyperparameters and regularize the training and validation of the model. It helped tremendously because I struggled with overfitting.

I quickly scanned a few articles when trying to go about creating the model and the only memorable one was this blog by Aashish Naik - "LSTM Neural Network to Predict SP500 Price" which captured a very impressive and simple LSTM model 
which predicted stock prices on older S&P 500 data. https://blog.gopenai.com/lstm-neural-network-to-predict-sp500-price-b2788a110b3a 
As of writing, I am unsure how he made such an impressive model  but my best guess would be our data is too different and maybe my processing of the data is not as good (I used his rnn to experiment and it compiled really poorly). 

I may revisit this project again but for now, I want to move on to NLP which was my core reason for starting machine learning.


