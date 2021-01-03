# Visual representation learning Tutorials
## Leren & Beslissen 2021

This repository serves as an introduction to deep learning for UvA students Leren & Beslissen course 2021 for the visual representation learning project. The repository consist of tutorial notebooks on deep learning and pytorch, autoencoders and Convolutional Neural Networks.

## Table Of Contents

### Tutorials

Under tutorials you can find notebooks on the following topics.

* [Part 1: Deep Learning & Pytorch](https://github.com/martinetoering/visual-representation-learning-tutorials/tree/master/tutorials/part-1-pytorch-deep-learning)
    * Tensors and Neural Networks 
    * Training and backpropagation
    * Validation and Inference
    * Loading images and Transfer learning
* [Part 2: ConvNets & Visualization](https://github.com/martinetoering/visual-representation-learning-tutorials/tree/master/tutorials/part-2-convnets-and-visualization)
    * Convolutional Neural Networks on CIFAR-10
    * Convolutional Visualization and Filters
* [Part 3: Autoencoders](https://github.com/martinetoering/visual-representation-learning-tutorials/tree/master/tutorials/part-3-autoencoders)
    * Introduction to Autoencoders on MNIST: Simple Autoencoder, Convolutional Autoencoder and Denoising Autoencoder

---

## Resources 

Here you can find some resources that might be useful to you, in addition to the references found in the project description.

* Consider using [Google Colab](https://colab.research.google.com/) if you need access to more computing power. To learn more, see the [Colab intro](https://colab.research.google.com/notebooks/intro.ipynb).

* Additional resources on CNNs:
    * [Stanford CS231n](http://cs231n.github.io/)
    * [Colah's blog](https://colah.github.io/)
    * [Intuitive explanation ConvNets](https://ujjwalkarn.me/2016/08/11/intuitive-explanation-convnets/)
    
* Additional resources on representation learning and Autoencoders:
    * [Autoencoder Wikipedia](https://en.wikipedia.org/wiki/Autoencoder)
    * [Representation learning blog](https://neptune.ai/blog/understanding-representation-learning-with-autoencoder-everything-you-need-to-know-about-representation-and-feature-learning)

* Additional resources on self-supervised learning (Note: might not be beginner-friendly)
    * [Self-supervised learning simple introduction](https://medium.com/analytics-vidhya/what-is-self-supervised-learning-in-computer-vision-a-simple-introduction-def3302d883d)
    * [Self-supervised learning blog](https://lilianweng.github.io/lil-log/2019/11/10/self-supervised-learning.html)


---


## Getting Started

We recommend to configure and manage an environment with Anaconda, a package and environment manager.

### Overview
Using Anaconda consists of the following:

1. Install [`miniconda`](http://conda.pydata.org/miniconda.html) on your computer, by selecting the latest Python version for your operating system. If you already have `conda` or `miniconda` installed, you should be able to skip this step and move on to step 2.
2. Create and activate * a new `conda` [environment](http://conda.pydata.org/docs/using/envs.html).

---

### 1. Installation

**Download** the latest version of `miniconda` that matches your system.

|        | Linux | Mac | Windows | 
|--------|-------|-----|---------|
| 64-bit | [64-bit (bash installer)][lin64] | [64-bit (bash installer)][mac64] | [64-bit (exe installer)][win64]
| 32-bit | [32-bit (bash installer)][lin32] |  | [32-bit (exe installer)][win32]

[win64]: https://repo.continuum.io/miniconda/Miniconda3-latest-Windows-x86_64.exe
[win32]: https://repo.continuum.io/miniconda/Miniconda3-latest-Windows-x86.exe
[mac64]: https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh
[lin64]: https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh
[lin32]: https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86.sh

**Install** [miniconda](http://conda.pydata.org/miniconda.html) on your machine. Detailed instructions:

- **Linux:** http://conda.pydata.org/docs/install/quick.html#linux-miniconda-install
- **Mac:** http://conda.pydata.org/docs/install/quick.html#os-x-miniconda-install
- **Windows:** http://conda.pydata.org/docs/install/quick.html#windows-miniconda-install

### 2. Create and Activate the Environment

For Windows users, these following commands need to be executed from the **Anaconda prompt** as opposed to a Windows terminal window. For Mac, a normal terminal window will work. 

#### Git and version control
These instructions also assume you have `git` installed for working with Github from a terminal window, but if you do not, you can download that first with the command:
```
conda install git
```

**Now, we're ready to create our local environment!**

1. Clone the repository, and navigate to the downloaded folder. This may take a minute or two to clone due to the included image data.
```
git clone https://github.com/martinetoering/visual-representation-learning-tutorials
```

2. Create (and activate) a new environment, named `deep-learning` with Python 3.6. If prompted to proceed with the install `(Proceed [y]/n)` type y.

	- __Linux__ or __Mac__: 
	```
	conda create -n deep-learning python=3.6
	source activate deep-learning
	```
	- __Windows__: 
	```
	conda create --name deep-learning python=3.6
	activate deep-learning
	```
	
	At this point your command line should look something like: `(deep-learning) <User>:deep-learning-v2-pytorch <user>$`. The `(deep-learning)` indicates that your environment has been activated, and you can proceed with further package installations.

3. Install PyTorch and torchvision; this should install the latest version of PyTorch.
	
	- __Linux__ or __Mac__: 
	```
	conda install pytorch torchvision -c pytorch 
	```
	- __Windows__: 
	```
	conda install pytorch -c pytorch
	pip install torchvision
	```

6. Install a few required pip packages, which are specified in the requirements text file (including OpenCV).
```
pip install -r requirements.txt
```


#### _Acknowledgement - References_

* _The majority of the tutorial notebooks are from the lab assignments of the Udacity's [Deep Learning Nanodegree program](https://www.udacity.com/course/deep-learning-nanodegree--nd101)_

* _Other materials come from the Stanford CS231n course_
