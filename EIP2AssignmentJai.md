##										Jai Kishan Sharma

##														Batch-2 

### Convolution:

Two signals significantly combine together and form a new signal this mathematical process named as Convolution. One signal flipped to another signal and order of signal's doesn’t matter in convolution.

##### 						2D convolution sliding with one stride:

![alt text](https://github.com/jaikishansharma/EIP2Bathch2/blob/master/Convolution_schematic.gif?raw=true)

#####							Max pooling in convolution layer:

![alt text](https://github.com/jaikishansharma/EIP2Bathch2/blob/master/Pooling_schematic.gif?raw=true)



### Filters/Kernels:

In convolution network we need to transform input image for evaluation so weighted matrix which slides over the input data and perform a elementwise multiplication and summing up the result into a single output pixel and so on, this weighted matrix is called kernel/filter. 

Each filter in Conv layer produces one output channel. Each of the kernel of the filter slides over their respective input channels (like:RGB) and producing a processed version of each channel. These processed versions combined together and form a one channel. 

### Epochs:

To train CNN we need to provide input data volume into the neural network, This input volume for creating a model in CNN is named epochs. But this data we can't provide in one go because of high memory requirement, so we need to divide the amount of data into batches.

If we have 2000 training examples and batch size we considered 400 then it will take 5 iterations to complete 1 epoch.

### 1x1 convolution:

In 1*1 convolution we use kernel which has matrix size 1 so it results same size of filter as input. It means in this CNN process It does not combine the corelated fields. This filter does not care about correlation of information of same feature map. 

### 3x3 convolution:

In 3*3 convolution we use kernel which has matrix size 3 so it results [input-2] size of feature map's if it has 1 stride without any padding. It will combined corelated fields so visual pattern being learned here.

### Feature Maps:

In CNN while we considered any image as an input then through that image we need to extract feature to extract the information, so we need to store this information in feature map for further analysis. When convolution applied on input data using kernel, It will perform element wise matrix multiplication and sum the result, In this process this sum goes into separate matrix which is called Feature Map. In 3D CNN If we have 3 channel (RGB) then each kernel during convolution of input matrix generate 3 feature map.

###Feature Engineering (older computer vision concept):

In this process we use domain knowledge of data to create appropriate feature useful for ML algo's. It will help to predict accurate result. If we extract accurate feature from the data then it will directly proportional to accurate result from algo. There is no such standard for feature extraction from row data that's why some domain knowledge required to analyze and mold it in useful format.

### Activation Function:

This function help CNN to relate similar feature with perticular node and it's applied on all convolution layers. Activation function input's is weighted sum of input channel 

![alt text](https://github.com/jaikishansharma/EIP2Bathch2/blob/master/1*CYB2dyR3EhFs1xNLK8ewiA.gif?raw=true) 

#####weighted sum of input channel  + bias

![alt text](https://github.com/jaikishansharma/EIP2Bathch2/blob/master/1*RYYucIh3U-YFxrIkyQKzRw.gif?raw=true)

now activation function will decide wich node to fire in layer. There are number of different activation functions that uses in this process like: Relu, Softmax etc.





