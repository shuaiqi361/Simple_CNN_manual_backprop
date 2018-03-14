# Simple_CNN_manual_backprop
## This code is an implementation of a simple CNN without using tensorflow built-in optimization functions, we are dealing with a binary classificaton problem, classify MNIST digit 0 and 1.

### For simplicity, the network is defines as the follows:

#### 1. Input layer is a tensor [#image, 28, 28]

#### 2. Images are vonvolved with 2 5-by-5 filters(stride 1) and feed into a Relu activation function produce [#image, 24, 24]

#### 3. An average pooling layer is stacked after the Relu activation function, with a kernel size 2-by-2, and stride 2 [#image, 12, 12]

#### 4. Then the 2 feature maps are vectorizes to form a fully connected layer[#image, 288], and then pass through a sigmoid node and finally produce the output [#image, 1]

##### The gradients computed manually are compared with the gradients computed by tf.gradients() function, the results for the weights between fully connected layer and output, also the weights for the first filter are printed in the source code.
