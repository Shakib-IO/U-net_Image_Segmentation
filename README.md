# U-net_Image_Segmentation


 -  So, U-Net is an architecture for semantic segmentation. It consists of a contracting path and an expansive path. The contracting path follows the typical architecture of a convolutional network. It consists of the repeated application of two 3x3 convolutions (unpadded convolutions), each followed by a rectified linear unit (ReLU) and a 2x2 max pooling operation with stride 2 for downsampling. At each downsampling step we double the number of feature channels. Every step in the expansive path consists of an upsampling of the feature map followed by a 2x2 convolution (“up-convolution”) that halves the number of feature channels, a concatenation with the correspondingly cropped feature map from the contracting path, and two 3x3 convolutions, each followed by a ReLU. The cropping is necessary due to the loss of border pixels in every convolution. At the final layer a 1x1 convolution is used to map each 64-component feature vector to the desired number of classes. In total the network has 23 convolutional layers.
--- 
The network Architecture 
<img src = 'https://paperswithcode.com/media/methods/Screen_Shot_2020-07-07_at_9.08.00_PM_rpNArED.png'>


- So this U-net Architecture divided into two sides , the left side for encoding the input and right side is decoding

An excellent explation of U-Net Architecture 
[Explation of U-Net](https://youtu.be/azM57JuQpQI?list=PLZsOBAyNTZwbR08R959iCvYT3qzhxvGOE)

[Paper: U-Net: Convolutional Networks for BiomedicalImage Segmentation](https://arxiv.org/abs/1505.04597)
