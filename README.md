# Strabismus Detection Tensorflow Model

This Tensorflow Model can classify Strabismus eyes and No Strabismus Eyes as normal by Image of eyes.

## Model Description

The model has 4 convolutional layers with max pooling between them. layers use 64, 96, 128 and 204 filters respectively. A flatten layer comes after these convolutional layers to flat the created 3d tensors. Then the extracted features gave to a 512 units fully connected layer followed by two other fully connected layers that has 256 and 128 units respectively.

### Test Results

Results on the test data after training:

| Measure           | Value |
| ----------------- | ----- |
| Balanced Accuracy | 70.8% |
| Sensitivity       | 66.6% |
| Specificity       | 75%   |

### Model Input Data

The model gets 23:9 ratio image of eyes as input to detect strabismus. A sample image of input data is given below.
![Sample Image](./example/normal.jpg)

## Usage Instructions

You can use use this model in two ways.

1. Use presented function with python.
2. Use model in your way.

### Use presented function with python

To use "strabismus_predict" function give it image path as string.
