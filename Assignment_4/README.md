# CMPE 258, HW 4 Abhishek Bais

Part 1 : Numpy
a) Mini batch gradient descent along with appropriate learning rate.
b) Dropout, initialize the random weights of network properly.
c) Basic image augmentations to supplement the training data.
d) Should use 3 or more layers for training (not 2 as in example ).
e) Should use relu activation layer in right places like python code.
f) Should normalize the input before training (scaling the input).
g) Should use appropriate learning rate.
h) Should provide appropriate metrics, visualization.
i) Should display top common errors like in below link.

Accuracy without dropout layer, 25 epochs: 98.01%
Accuracy with dropout layer, 25 epochs: 97.83%
Accuracy with dropout layer + image augmentation (Phd trained params), 25 epochs: 99.23%

Extra points if you hit 99% test accuracy with these changes (very challenging given you are not using CNNs).
Achieved accuracy of 99.23% without CNN

Part 2 : Keras
Tried both without and with CNN with dropout layer, adaptive learning rate, 
patience =5, and image augmentation (Phd trained params), 10 epochs
Accuracy with dropout layer + Flatten + CNN, 10 epochs = 
