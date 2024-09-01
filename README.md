This project is a model designed to do both BIS analysing and predicting in the same time.<br>
The RSNet_LSTM.py is the model that using DRSN and LSTM. The ResNet_LSTM.py is the model using ResNet+LSTM. The pretrained model is of the same name.<br>
To get data, the input_original.py is used. You can decide which cases of operation is needed and download them into two .npy file as train or test case. The two numpy array will be saved to ./data.<br>
The input_eeg_filtered.py is a signal filter which can reduce the high-frequency noises in the signal. Filtered data will be saved to the ./data_filtered folder.<br>

