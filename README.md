# eip_assignments
repository for assignments for EIP phase 2

## Assignment 1 :

1. Find 50 misclassified images from the pre-trained ResNet18 Model trained on CIFAR10.
    https://keras.io/examples/cifar10_resnet/ (https://keras.io/examples/cifar10_resnet/)
2. Run GradCam (http://www.hackevolve.com/where-cnn-is-looking-grad-cam/) on these images
3. Create a gallery of your GradCam results



There are two files submitted: 

1.**EIP_Phase2_Assignment1_approach1_v1.ipynb**  : In this file we train a resent model on cifar10 dataset for 200 epochs.We use Imgaug library for image augmentation.The misclassified images are passed to GradCam and a collage of the result images is shown.

2.**EIP_Phase2_Assignment1_approach2_v1.ipynb**: In this file we train a resent model on cifar10 dataset for 200 epochs.We use cut-off/random erasure library for image augmentation.The misclassified images are passed to GradCam and a collage of the result images is shown.



# Assignment 2 :

1. Go through this Post: [https://machinelearningmastery.com/text-generation-lstm-recurrent-neural-networks-python-keras/ (Links to an external site.)](https://machinelearningmastery.com/text-generation-lstm-recurrent-neural-networks-python-keras/)
2. Add these improvements to the final code described in the post:
   1. Predict 500 characters only
   2. Remove all the punctuation from the source text
   3. Train the model on [padded sequences (Links to an external site.)](https://machinelearningmastery.com/data-preparation-variable-length-input-sequences-sequence-prediction/) rather than random sequences of characters. 
   4. Train the model for 100 epochs
   5. Add dropout to the input layer, remove it from the layer before dense layer. Use Dropout value of 0.1 everywhere

​     There are two files submitted:

​	1.**EIP_Phase2_Assignment2_LSTM_Approach1_v1.ipynb** : We use two LSTM layers each with 256 units and dropout of  0.1 after the first LSTM layer.The trained model is used to predict next 500 characters, given a seed.

​	2.**EIP_Phase2_Assignment2_LSTM_Approach1_v2.ipynb** : We use two LSTM layers each with 256 units and dropout of  0.5 after the first LSTM layer.The trained model is used to predict next 500 characters, given a seed. This is just additional exploration done to check if more dropout will improve the performance.There is only slight improvement with increased dropout.