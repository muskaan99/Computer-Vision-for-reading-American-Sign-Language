This project is a part of EE541 - A Computational Introduction to Deep Learning. The goal of this project is to accurately predict American Sign Language hand gestures and compare model performance. 

# Setup (Google Colab Notebooks)

We trained the model on Google Colab with a Tesla P100 GPU using Pytorch.

### Instructions for installation of PyTorch: 

* Create conda environment _conda create --name cnn_

* Activating the conda environment _conda activate cnn_

* Installation of pytorch in the conda environment _conda install pytorch torchvision -c pytorch_
 
* After the installation, a new .ipynb file should be opened under the newly created environment.

* Once Pytorch is installed, setup Nvidia GPU drivers if not setup already.

* Download the dataset from [here](https://www.kaggle.com/datasets/grassknoted/asl-alphabet) 

* Download the real-world test dataset from [here](https://www.kaggle.com/datasets/muskaan3299/self-generated-test-set)

* To start training the model, run the respective cells and functions in the notebook.

# Code Structure

* The complete code for the project to train and test multiple models is in ASL_Project.ipynb

# Model Files

* Optimal Neural Network Model: 1.1 GB

* Optimal CNN Model: 287 kB

* Optimal Resnet-50 Model: 104.64 MB

* Optimal MobileNet-V2 Model:14.51 MB


