Cifar-10 neural-net classifier
======

The CIFAR-10 classifier example. Datasets from [cifar-10 datasets](http://www.cs.toronto.edu/~kriz/cifar.html).

## USAGE
### Data acquisition and shaping:
```
wget https://www.cs.toronto.edu/~kriz/cifar-10-python.tar.gz
gzip -d cifar-10-python.tar.gz
tar -xf cifar-10-python.tar
python data.py
```

### Training

Training can be done in two ways: Simple neural network or Convolutional neural network.

In either case, if you use GPU, add option ```-g 0```. If you want to export result figures, ```-p on``` and write log, ```-l on```.

#### Simple neural network training
```
python  train_nn.py
```

#### Convolutional neural network training

```
python  train_cnn.py
```

Jan, 2016: Googlenet can not be used yet. Please use cnn_alex.py (default in ```train_cnn.py```).

## Requirement
[chainer v1.5.1](http://chainer.org/)

And [other packages](https://github.com/pfnet/chainer#requirements) around chainer.

## Author

[shiba24](https://github.com/shiba24)

