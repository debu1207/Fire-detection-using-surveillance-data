# Fire-detection-using-surveillance-data

In this project, surveillance data is used for training the model.

# Main idea of the Project
The algorithm used is the based on the Residual learning.

In deep CNN, several layers are stacked and trained to the task at hand.
Network learns several low/ mid/ High  level  feature at the end of its layers.

In residual learning, instead of trying to learn some features, we try to learn some residual. Residual can be simply understood as subtraction of feature learned from input of that layer.

Residual Network does this using shortcut connections (directly connecting iput of nth layer to some (n+x)th layer. It has proved that training this form of networks is easier than training simple deep CNNs and also the problem of degrading accuracy is resolved.

# Code Explanation
ResNet50 is used in the code. It is a convolutional neural network which is 50 layers deep.
Residual layers networks are used as a backbone for many computer vision tasks.

Convnets or CNNs are rarely trained from scratch. 
We reuse the base of pretrained model. To the pretrained base we then attach an untrained head. 

We reuse the part of a network that has already learned to Extract features, and attach to it some fresh layers to learn to classify.

Reusing a pretrained model is a technique known as transfer learning. It is so effective, that almost every image classifier these days will make use of it.

# Flowchart of Code
Load the data for preprocessing

Label the data

Splitting of data in training and testing sets

Load the pretrained data (ResNet50)

Adding the head  to the base model for classification

Setting the optimizer and loss function

Training the model

Classification result



