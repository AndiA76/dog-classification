# Dog Image Classification using CNNs and Pytorch

## Overview

This project from Udacity's nano-degree course "Deep-Learning" is about Dog Classification (and human face detection) using different Convolutional Neural Networkds (CNNs). The task is to set up an App that can detect dogs and human faces in color images and predict the breed if a dog is detected.

The project is broken down in subtasks starting with human face detection using face detectors from OpenCV, then dog breed classification using publicly available pre-trained CNN models, dog breed detection using a CNN built from scratch and using transfer learning on a feature detector taken from a pre-trained model, which is combined with a new classifier head that is trained for dog breed detection. The project closes with defining the above mentioned App that can detect dogs and human faces in color images and predict the breed if a dog is detected.

* Step 0: Import Datasets
* Step 1: Detect Humans
* Step 2: Detect Dogs
* Step 3: Create a CNN to Classify Dog Breeds (from Scratch)
* Step 4: Create a CNN to Classify Dog Breeds (using Transfer Learning)
* Step 5: Write your Algorithm
* Step 6: Test Your Algorithm

The project is implemented as a Jupyter notebook and can be found there: [Project Notebook](dog_app.ipynb)

## Installation

### 1. Install Anaconda with Python

In order to run the notebook please download and install [Anaconda](https://docs.anaconda.com/anaconda/install/) with Python 3.6 on your machine. Further packages that are required to run the notebook are installed in a virtual environment using conda.

### 2. Create a Virtual Environment

In order to set up the prerequisites to run the project notebook you should create a virtual environment, e. g. using conda, Anaconda's package manager, and the following command

```
conda create --name deep-learning
```

The virtual environment needs to be activated by

```
activate deep-learning
```

### 3. Download the project from github

You can download the project from github as a zip file to your Downloads folder from where you can unpack and move the files to your local project folder. Or you can clone from Github using the terminal window. Therefore, you need to prior install git on your machine e. g. using

```
conda install -c anaconda git
```

When git is installed you can create your local project version. Therefore, navigate to your project folder and clone the project from github using the command

```
git clone https://github.com/AndiA76/dog-classification.git
```

Then change to the project directory

```
cd dog-classification
```

### 4. Install Pytorch with GPU support

In order to run the project notebook you need to install Pytorch. If you wish to install Pytorch with GPU support you also need to take care of your CUDA version and some [dependencies with Pytorch](https://pytorch.org/get-started/previous-versions/). I have used Ubuntu 18.04 LTS with CUDA 10.0 and Python 3.6 to run the project notebook. Therefore you need to enter the following installation command:

CUDA 10.0
```
conda install pytorch==1.2.0 torchvision==0.4.0 cudatoolkit=10.0 -c pytorch
```

### 5. Further requirements 

Besides Pytorch you need to install a couple of further packages, which are required by the project notebook. The packages are specified in the [requirements.txt](requirements.txt) file (incl. OpenCV for Python). You can install them using pip resp. pip3:

```
pip install -r requirements.txt
```

### 6. Download the dataset

In order to run the notebook you need to download the required human and dog datasets:
* Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip).  Unzip the folder and place it in this project's home directory, at the location `/dogImages`. 

* Download the [human dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip).  Unzip the folder and place it in the home directory, at location `/lfw`.  

### 7. Run the notebook

Now start a Jupyter notebook to run the project using following command

```
jupyter notebook
```

Navigate to your local project folder in the Jupyter notebook and open [dog_app.ipynb](dog_app.ipynb) file and run it.