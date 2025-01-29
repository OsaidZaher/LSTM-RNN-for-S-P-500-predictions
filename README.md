An S&P 500 Long Short-Term Memory recurrent neural network. 
Due to data shuffling and batching, you get different Mean Absolute Error, Mean Squared Error, and Root Mean Squared Error. I tried to combat this by creating a constant seed for tensorflow and numpy and setting deterministic operations.
The model performs well with an MAE of sub-60.

To give credit to how I created the model, I was inspired to do this after finishing "Hands-On Machine Learning with Scikit-Learn, Keras, and Tensorflow: Concepts, Tools, and Techniques to Build Intelligent" by  Aurélien Géron. 
I continuously referenced Chapter 15 (Processing sequences using Rnns and Cnns) to split and process the time series data and create the RNN.
I went back to Chapter 11 (Training Deep Neural Networks) to fine-tune the hyperparameters and regularize the training and validation of the model. It helped tremendously because I struggled with overfitting.

I quickly scanned a few articles when trying to go about creating the model and the only memorable one was this blog by Aashish Naik - "LSTM Neural Network to Predict SP500 Price" which captured a very impressive and simple LSTM model 
which predicted stock prices on older S&P 500 data. https://blog.gopenai.com/lstm-neural-network-to-predict-sp500-price-b2788a110b3a 
Usually, RNNs train with over 100 epochs but I wanted to have a high-speed model. (the author of the article uses over 1000 epochs my model finishes training at 20)

I may revisit this project again but for now, I want to move on to NLP which was my core reason for starting machine learning.


