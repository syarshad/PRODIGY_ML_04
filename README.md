This project focuses on building a machine learning model to classify hand gesture images into different categories using Convolutional Neural Networks (CNN) implemented with the Keras library. The dataset used contains images of hand gestures from various categories.

# Methods Used:

## Data Collection:
The dataset consists of images of hand gestures from different categories such as palm, fist, thumb, index, etc.
Each category is represented by a subdirectory containing images corresponding to that category.

## Data Preprocessing:
Images were loaded using the OpenCV library (cv2) and converted to grayscale.
Images were resized to a standard size (IMG_SIZE x IMG_SIZE) to ensure uniformity.

## Feature Extraction:
The grayscale images were used as input data for training the CNN model.

## Model Architecture:
A Sequential model was defined using Keras.
The model consists of convolutional layers (Conv2D), activation layers (Activation), max-pooling layers (MaxPool2D), dropout layers (Dropout), and fully connected layers (Dense).
ReLU activation was used for the convolutional layers, and softmax activation was used for the output layer to obtain class probabilities.

## Model Training:
The model was compiled with categorical cross-entropy loss and the RMSprop optimizer.
Training was performed using the fit method on the training data for a specified number of epochs.

## Model Evaluation:
Model performance was evaluated using the test data, and metrics such as accuracy were calculated.
The confusion matrix was generated to visualize the classification performance across different categories.

# Results:
The CNN model achieved a test accuracy of approximately 99.88%, indicating high performance in classifying hand gesture images.
The loss and accuracy plots demonstrate that the model successfully learned to classify hand gestures over the training epochs.
