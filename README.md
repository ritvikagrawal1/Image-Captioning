# Image Captioning

This repository contains an implementation of image captioning based on neural network (i.e. CNN + RNN). The model first extracts the image feature by CNN and then generates captions by RNN. CNN is ResNet and RNN is a standard LSTM .


# Network Topology:-

## Encoder
The Convolutional Neural Network(CNN) can be thought of as an encoder. The input image is given to CNN to extract the features. The last hidden state of the CNN is connected to the Decoder.
## Decoder
The Decoder is a Recurrent Neural Network(RNN) which does language modelling up to the word level. The first time step receives the encoded output from the encoder and also the <START> vector.

Dataset used was <a href="http://nlp.cs.illinois.edu/HockenmaierGroup/Framing_Image_Description/KCCA.html">Flickr8k dataset</a>.

# Model Architecture
![input](https://miro.medium.com/max/1000/1*VGzSnYhyhpAAmGkSyOfeig.png)


# Dependencies

* Keras 2.0.7
* Numpy
* Pandas 0.20.3
* Matplotlib
* Pickle

# References

[1] Deep Visual-Semantic Alignments for Generating Image
Descriptions ( Karpathy et-al, CVPR 2015) 

[2] Oriol Vinyals, Alexander Toshev, Samy Bengio, Dumitru Erhan <a href="https://arxiv.org/abs/1411.4555">Show and Tell: A Neural Image Caption Generator</a>

[3] CS231n: Convolutional Neural Networks for Visual Recognition.
( Instructors : Li Fei Fei, Andrej Karpathy, Justin Johnson)
