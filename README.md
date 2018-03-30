# Simple_CNN_manual_backprop
## This code is an implementation of a simple CNN without using tensorflow built-in optimization functions, we are dealing with a binary classificaton problem, classify MNIST handwritten digit 0 from other digits

### For simplicity, the network is defines as the following:

#### 1. Input layer is a tensor [#image, 28, 28], MNIST images

#### 2. Images are convolved with one 5-by-5 filter(stride 1) and fed into a Relu activation function producing [#image, 24, 24]

#### 3. A max pooling layer is stacked after the Relu activation function, with a kernel size 3-by-3, and stride 3 [#image, 8, 8]

#### 4. Then the feature map is vectorized to form a fully connected layer[#image, 64], and then squeeze into a sigmoid node and finally produce the output [#image, 1], the sigmoid cross entropy loss is implemented here
