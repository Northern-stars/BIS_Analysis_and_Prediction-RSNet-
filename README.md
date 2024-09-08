This project is a model designed to do both BIS analysing and predicting in the same time.<br>
The RSNet_LSTM.py is the model that using DRSN and LSTM. The ResNet_LSTM.py is the model using ResNet+LSTM. The pretrained model is of the same name.<br>
To get data, the input_original.py is used. You can decide which cases of operation is needed and download them into two .npy file as train or test case. The two numpy array will be saved to ./data.<br>
The input_eeg_filtered.py is a signal filter which can reduce the high-frequency noises in the signal. Filtered data will be saved to the ./data_filtered folder.<br>
Code explaination:<br>
The train function(epoch) is used to start the training process with no pretrained model, and save trained model to ./RSNet_LSTM.pth. The variable "epoch" is set as the training epochs. <br>
The following_train(epoch) is used to do the training process with pretrained model. The path of model parameters is ./RSNet_LSTM.pth. And the model will be saved to the same path.
The test function is used to test the model with one test dataset.<br>
The sequence test is used to test the model with a number of test dataset. The dataloader of the sequence of test dataset is the sequence_dataloader.<br>
