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

