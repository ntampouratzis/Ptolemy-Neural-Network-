# Ptolemy-Neural-Network
This repo contains a fully connected neural network implementation and also a GRU and LSTM network implementation in Ptolemy II.


# Fully-Connected Network 
A one-hidden layer architecture trained for handwritten digit recognition.

It gets as input a 28x28 grayscale image of a handwritten digit and it produces the probabilities related to the 10 classes of digits from 0 to 9.

It is implemented in Ptolemy II using the Discrete-Event (DE) and the Synchronous Dataflow (SDF) Models of Computation (MoCs).

![test](https://github.com/ntampouratzis/Ptolemy-Neural-Network/blob/master/ptolemy-models/DE-SDF/HandWrittenDigitRecognition/de-sdf_handwrittenDigitImageRecognitionNeuralNet.png)


# GRU and LSTM Networks
These architectures are trained to get hourly weather measurements of 10 days as input and produce as output the prediction of the temperature of the next day at the same specific day-hour.

They are implemented in Ptolemy using an hierarchy of DE-ModalModel-SDF MoCs.

<img src="https://github.com/ntampouratzis/Ptolemy-Neural-Network/blob/master/ptolemy-models/DE-Modal-SDF/GRU/temperaturePredictionUsingGRU.png" width="1226">

<img src="https://github.com/ntampouratzis/Ptolemy-Neural-Network/blob/master/ptolemy-models/DE-Modal-SDF/LSTM/temperaturePredictionLSTM.png" width="1226">

# Ptolemy  II  machine  learning  library
The following figure shows our Ptolemy II machine learning library which is implemented in UserLibrary folder. The library enables  the  designers  to  develop their complex recurrent neural networks using our fundamental structures minimizing the development and verification time.

In order to include our library into your Ptolemy II installation, you may either replace your /home/&lt;username&gt;/.ptolemyII/UserLibrary.xml with our library found in the UserLibrary folder, or you may open our library using vergil (the Ptolemy II editor) and copy our library blocks into your library.

Examples showing the use of the library are the aforementioned GRU and LSTM networks implementations.

<img src="https://github.com/ntampouratzis/Ptolemy-Neural-Network/blob/master/ptolemy-models/UserLibrary/library.png">
