# ML-2020 AutoEncoder-by-Forest
Typically, autoencoders (AEs) are assotiated with Neural Networks. Yet in [the paper](https://arxiv.org/pdf/1709.09018.pdf) the authors propose to use Decision Tree for AE and claim that their approach has reasonable performance. Here we have reproduced the paper results: we have implemented AE forest algorithm and compared its performance with MLP &amp; CNN  AEs on image datasets (MNIST, CIFAR-10, Omniglot).

![](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/images/autoencoder.png)

The code was written by:

- Egor Sevriugov - Tree ensemble based AE (MNIST, CIFAR-10, Omniglot), 
- Kirill Shcherbakov - CNN based AE (MNIST, CIFAR-10, Omniglot), 
- Maria Begicheva - MLP based AE (MNIST, Omniglot),
- Olga Novitskaya - MLP based AE (CIFAR-10, Omniglot)

**AEbyForest: [Project](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest) | [Paper](https://arxiv.org/pdf/1709.09018.pdf) | [Report](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/AutoEncoder_by_Forest.pdf) | [Presentation](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/presentation/Presentation_AutoEncoder_by_Forest.pdf) | [Video](https://www.dropbox.com/s/v0iiwld87gk658y/zoom_0.mp4?dl=0)**

Train MNIST/Test MNIST
![](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/images/Merged_MNIST.png)

Train CIFAR10/Test CIFAR10
![](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/images/Merged_CIFAR10.png)


## Colab Notebook
- Tree ensemble based AE (MNIST, CIFAR-10, Omniglot): [Google Colab](https://colab.research.google.com/github/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/eForest_models/eForest_ml%20.ipynb) | [Code](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/tree/master/eForest_models)
- CNN based AE (MNIST, CIFAR-10, Omniglot): [Google Colab](https://colab.research.google.com/github/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/CNN_models/CNNs_models.ipynb) | [Code](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/tree/master/CNN_models)
- MLP based AE (MNIST, Omniglot): [Google Colab](https://colab.research.google.com/github/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/MLP_models/MLP_MNIST.ipynb) | [Code](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/MLP_models/MLP_MNIST.ipynb)
- MLP based AE (CIFAR-10, Omniglot): [Google Colab](https://colab.research.google.com/github/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/MLP_models/MLP_CIFAR_10.ipynb) | [Code](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/MLP_models/MLP_CIFAR_10.ipynb)

## Prerequisites
- Python 3
- Google Colaboratory service
- PyTorch 1.4.0, Tensorflow 2.1.0, Keras 2.3.0

## Datasets info
- MNIST and CIFAR-10 datasets were got from keras.datasets module:  [MNIST dataset](https://keras.io/datasets/#mnist-database-of-handwritten-digits) | [CIFAR-10 dataset](https://keras.io/datasets/#cifar10-small-image-classification)
- Omniglot dataset was got from torchvision.datasets module: [Omniglot dataset](https://github.com/pytorch/vision/blob/master/torchvision/datasets/omniglot.py)

## How to launch the code?
To help users better understand and use our code, for each model we created instructions for running the code and reproducing the results:

- eForest instruction for running the code and reproducing the results: [eForest Instruction](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/eForest_models/README.md)

- CNN-AE instruction for running the code and reproducing the results: [CNN-AE Instruction](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/CNN_models/README.md)

- MLP-AE instruction for running the code and reproducing the results: [MLP-AE Instruction](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/MLP_models/README.md)


## Related Projects

- The official implementation for the paper "AutoEncoder by Forest" by Ji Feng and Zhi-Hua Zhou 2017:  [Paper](https://arxiv.org/pdf/1709.09018.pdf) | [Code](https://github.com/kingfengji/eForest)
- Non-official implementation of the paper "AutoEncoder by Forest" by Ji Feng and Zhi-Hua Zhou 2017 by Antoine Passemiers:  [Paper](https://arxiv.org/pdf/1709.09018.pdf) | [Code](https://github.com/AntoinePassemiers/Encoder-Forest)
