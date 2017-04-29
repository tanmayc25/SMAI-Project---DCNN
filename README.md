# Doubly Convolutional Neural Network

### SMAI Project by
>  Akanksha Baranwal - 201430015

> Parv Parkhiya - 201430100

> Prachi Agrawal - 201401014

> Tanmay Chaudhari - 201430012

### Original Paper
> [Doubly Convolutional Neural Networks] (NIPS 2016) by Shuangfei Zhai, Yu Cheng, Weining Lu and Zhongfei (Mark) Zhang

### Repository Content

- *final project* contains main DCNN code written in python
- *forword pass* contains Matlab code of forword pass for understanding and proof of concept
- *Correlation* contains python code to extract weights from caffee model, matlab code to find averaged max transalation correlation of a layer, ploted results  

### Pre-requisites
Code is written in python and would require following libraries:

- numpy
- theano (tensor)
- lasagne

Our Code is tested on Ubuntu 14.04 amd64 without CUDA but should run on any OS satisfying above pre-requisites.
### Downloading Dataset
- Code is tested on [MNIST] dataset which is dataset that comprises of handwritten digits.
- Code will automatically download dataset or can manually placed in the project directory as **mnist.pkl.gz**. 

### Setting Various Parameters

Default Parameters:
```sh    
num_epochs = 100
learning_rate = 1e-2 
metafilter_shape = [(2, 1, 6, 6), (4, 2, 6, 6)]
image_shape = (1, 28, 28)
kernel_size = 5
kernel_pool_size = 2
learning_decay = 1e-5
dropout_rate = 0.5
batch_size = 200
```
These parameters can be found and changed just below main function declaration.

### Running the code

You can run the code using following command.

```sh
sudo python main_final.py
```
*Note: sudo access is required is to write results in a file*

### Architecture
![DCNN and CNN Architecture](http://i.imgur.com/ZLaaimu.png "Architecture")

### Results


![Alt text](http://www.arbormaxtree.com/wp-content/uploads/2014/10/Raleigh-Tree-Removal-1024x884.jpg "Optional title")


### Links

[Getting Started with CNN Lasagne]
[Lasagne Docs]: https://lasagne.readthedocs.io/en/latest/
[Theano Docs]: http://deeplearning.net/software/theano/library/index.html



[Doubly Convolutional Neural Networks]: <https://papers.nips.cc/paper/6340-doubly-convolutional-neural-networks.pdf>
[MNIST]: <yann.lecun.com/exdb/mnist/>
[Getting Started with CNN Lasagne]: <http://luizgh.github.io/libraries/2015/12/08/getting-started-with-lasagne/>
[Lasagne Docs]: <https://lasagne.readthedocs.io/en/latest/>
[Theano Docs]: <http://deeplearning.net/software/theano/library/index.html>
