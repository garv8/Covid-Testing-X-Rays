# Covid-Testing-X-Rays

The COVID-19 Detection CNN is a Convolutional Neural Network designed to identify whether a patient has Covid-19 based on their X-ray images. Leveraging state-of-the-art deep learning techniques, this CNN boasts an impressive accuracy rate of 97%, providing a reliable and efficient solution for early detection of Covid-19 through medical imaging.

## Datasets:
- Positive Cases : https://github.com/ieee8023/covid-chestxray-dataset
- Normal Cases : https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia

## Model Architecture:
The CNN architecture consists of multiple convolutional layers followed by max-pooling layers and dropout regularization for improved generalization. Here's a breakdown of the layers:

Convolutional Layers:
- Layer 1: 32 filters with a kernel size of (3,3) and ReLU activation.
- Layer 2: 64 filters with a kernel size of (3,3) and ReLU activation, followed by max-pooling and dropout.
- Layer 3: 64 filters with a kernel size of (3,3) and ReLU activation, followed by max-pooling and dropout.
- Layer 4: 128 filters with a kernel size of (3,3) and ReLU activation, followed by max-pooling and dropout.
- Layer 5: 128 filters with a kernel size of (3,3) and ReLU activation, followed by max-pooling and dropout.

Fully Connected Layers:
- Flatten layer to transition from convolutional layers to dense layers.
- Dense layer with 64 neurons and ReLU activation, followed by dropout for regularization.
- Output layer with a single neuron and sigmoid activation for binary classification.

The model is compiled using the Adam optimizer and binary crossentropy loss, suitable for binary classification tasks. The accuracy metric is monitored during training.
