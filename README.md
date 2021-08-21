# Densely Connected Convolutional Networks


DenseNets with <b>L</b> layers has <b>L(L+1)/2</b> direct connections. They address this shortcoming by reducing the size of the modules and by introducing more connections between layers. In fact, the output of each layer flows directly as input to all subsequent layers of the same feature dimension as illustrated in their <b>Figure 1</b>. This increases the dependency between the layers and thus reduces redundancy.

<img src="https://github.com/Engelbert107/Densely-Connected-Convolutional-Networks/blob/main/DenseNet4Blocks.png" width="550" height="400">

<h2>Why multiple densely connected dense blocks?</h2>

For this DenseNet we did a concatenation of features and to be able to perform the concatenation operation, we need to make sure that the size of the feature maps that we are concatenating is the same.

It clear that we can’t just keep the feature maps the same size throughout the network. But an essential part of concvolutional networks is down-sampling layers that change the size of feature maps.

Thus to facilitate both down-sampling in this architecture (<b>Figure 1</b>) and feature concatenation, the authors divided the network into multiple densely connected dense blocks.

<img src="https://github.com/Engelbert107/Densely-Connected-Convolutional-Networks/blob/main/DeepDenseNet.png" width="1200" height="220">

<img src="https://github.com/Engelbert107/Densely-Connected-Convolutional-Networks/blob/main/DenseNetForImageNet.png" width="1000" height="480">
