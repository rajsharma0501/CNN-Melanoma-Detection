# Melanoma Detection
> multiclass classification model using a custom convolutional neural network in TensorFlow to identify the Melanoma from given skin disease picture

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
This project aims to build a Convolutional Neural Network (CNN) model to detect melanoma, a dangerous type of skin cancer, from skin lesion images. Early detection can save lives, making it essential to develop an accurate and reliable model.
The dataset used for this project consists of 2.3k train images  split into training and validation sets. The goal was to train a CNN model capable of classifying lesions as melanoma or benign (non-cancerous).
Various techniques, including data augmentation (e.g., rotations), were employed to prevent overfitting and improve model performance. The final model achieves good accuracy without the need for batch normalization, showing that a simpler architecture with proper regularization can perform well.


---

Model Architecture

Convolutional Layers:

Layer 1: 32 filters

Layer 2: 64 filters

Layer 3: 128 filters


Dense Layer: 128 units

Dropout Regularization:

0.2 after each convolutional layer

0.5 after the final convolutional layer

0.25 after the dense layer


Output Layer: Softmax activation for classification

Optimizer: Adam with default learning rate (0.001)

Loss Function: Categorical Crossentropy


## Conclusions
The final model achieved 85% training accuracy and 80% validation accuracy, indicating that it generalizes reasonably well across unseen data. Removing batch normalization simplified the model, and with appropriate dropout regularization, the model was able to mitigate overfitting.

While the current model performs well, further improvements can be achieved by fine-tuning hyperparameters, increasing the dataset size, or employing advanced architectures like transfer learning models (e.g., ResNet or InceptionV3). Future work will also explore additional augmentation strategies to further enhance generalization.


## Technologies Used
- tensorflow - v2.17
- matplot - v3.9.1
- python - v3.12
- numpy - v1.26.4
- Augmentor - v0.2.12
<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->


## Contact
Created by [sharma.rajcse@gmail.com] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
