
<p align="center">
<img src="./etc/img/logo.png" width="800">
</p>

**Tensorbag** is a collection of tensorflow tutorial on different Deep Learning and Machine Learning algorithms. The tutorials are organised as **jupyter notebooks** and require *tensorflow >= 1.5*. There is a subset of notebooks identified with the tag **[quiz]** that directly ask to the reader to complete part of the code. In the same folder there is always a complementary notebook with the complete solution.

Datasets
---------

- **XOR**: this dataset is based on the Exclusive OR logical operator. It is a non-linear dataset that can be used for simple tests. There are two input values represented as float, that can be generated in a pre-defined range. The label is a single integer representing True (one) or False (zero). The files are generated using the random uniform method in Tensorflow. The distribution is plotted in Matplotlib and the file are stored as TFRecords. The test (2000 samples) and train (8000 samples) TFRecord files are provided with the repository. [[notebook]](./xor/xor.ipynb)

- **Iris Flowers**: it is a simple dataset of flowers classified using sepal and petal dimensions (four attributes). The data set contains three classes (Setosa, Versicolour, Virginica) of 50 instances each, where each class refers to a type of iris plant. One class (Setosa) is linearly separable from the other two (Versicolour and Virginica), whereas the latter are not linearly separable from each other. The pre-processing produces the training and test files in TFRecord format. The linear version of the dataset can be used to train simple models such as the Perceptron. Ready-to-use TFRecords are included in this repository. [[notebook]](./iris/iris.ipynb)

- **MNIST**: it is a famous dataset of handwritten digits that is commonly used as benchmark in Deep Learning. It has 60k training images, and 10k test images. The tutorial shows how to download and prepare the dataset. The pre-processing produces the training and test files in TFRecord format. [[notebook]](./mnist/mnist.ipynb)

- **CIFAR-10**: it is a dataset of 50k 32x32 color training images, labeled over 10 categories, and 10k test images. The tutorial shows where to download and how to prepare the CIFAR-10 dataset. The pre-processing is done in different ways (Numpy and Tensorflow datasets) and produces training and test files in TFRecord format. [[notebook]](./cifar10/cifar10.ipynb)



Neural Network Architectures
-----------------------------

- **Multi Layer Perceptron (MLP)**: the MLP is an extension of the classical Perceptron. In its standard form it has an input layer, an hidden layer, and an output layer. In 1985 Rumelhart, Hinton and Williams experimentally verified that using an additional layer in the Perceptron and using a new update rule (backpropagation) the network was able to solve the XOR problem. In this tutorial a simple three layers MLP is designed. The model is trained on the XOR dataset (included in the repository). [[notebook]](./mlp/mlp.ipynb) [[quiz]](./mlp/mlp_quiz.ipynb)

- **LeNet-5 Convolutional Neural Network**: implementation of a standard LeNet-5 CNN as described in the [paper](http://www.dengfanxin.cn/wp-content/uploads/2016/03/1998Lecun.pdf) of LeCun et al. (1998). LeNet-5 was designed for handwritten and machine-printed character recognition. In this tutorial the network is trained and tested on the MNIST dataset. [[notebook]](./lenet5/lenet5.ipynb) [[quiz]](./lenet5/lenet5_quiz.ipynb)

- **ResNet Convolutional Network**: description and implementation of a *ResNet-18* as described in the [article](https://arxiv.org/pdf/1512.03385.pdf) of He et al. (2015). ResNet is one of the most famous architectures nowadays, and has been used in ILSVRC and COCO 2015 competitions, winning the 1st places in classification, detection, localization, and segmentation. Here a ResNet-18 is trained and tested on the CIFAR-10 dataset. [[notebook]](./resnet/resnet.ipynb) [[quiz]](./resnet/resnet_quiz.ipynb)

- **Generative Adversarial Network (GAN)**: implementation of a standard GAN as in the [original paper](https://arxiv.org/pdf/1406.2661.pdf) of Goodfellow et al. (2014). The GAN is trained and tested on the CIFAR-10 dataset. [TODO]
