# Real-Time-Recognition-of-Indian-Sign-Language

The project achieves recognition of Indian Sign Language using hand gestures from live video capture. Implemented using Python with OpenCV, TensorFlow and Keras.

## Introduction 

A gesture is a pattern which may be static, dynamic or both, and is a form of non verbal communication in which bodily motions convey information. 
Communication is an important aspect when it comes to sharing or expressing information, feelings, and it brings people closer to each other with better understanding. 
When it comes to disabled persons - deaf and dumb people, it becomes tougher for them to communicate using natural language. 
So, they use Sign Language to communicate with themselves and with the entire world. 

Sign language is composed of visual gestures and signs, which are used by deaf and mute for their talking and communication. 
It is a well-structured code gesture where every sign has a specific meaning allotted to it. 
These signs are not only used for alphabets or numeric but also for common expressions like greetings and sentences. 
There are 143 existing different sign languages all over the world, mainly American Sign Language (ASL), British Sign Language, French Sign Language, Japanese Sign Language, and Indian Sign Language (ISL). 

However, normal people find it difficult to understand sign language as they do not have mostly any prior education or experience in this. 
To spread awareness about sign language in our country, this project implements a real-time recognition of the Indian Sign Language. 
ISL uses both hands similar to British Sign Language and is similar to International Sign Language. 
ISL alphabets are derived from British Sign Language and French Sign Language alphabets. 
Unlike its American counterpart which uses one hand, ISL uses both hands to represent alphabets. 
Because of this reason, there is less research and development in this field. 
This project goal is to take the simple step in connecting the social and communication bridge between regular people and the disabled people with the help of Indian Sign Language.

## Prerequisites

1. [Python](https://www.python.org/downloads/) (64-bit for compatibility with Tensorflow)
2. [Anaconda](https://www.anaconda.com/products/individual)
3. Jupyter Notebook (IDE) 

Now, ```pip install``` the following dependencies:

1. numpy
2. OpenCV
3. Tensorflow (better to create a [virtual environment](https://www.tensorflow.org/install/pip))
4. Keras
5. scikit-image (skimage)

## Running 

1. Clone the repository to your system or download and extract the zipped folder. 
2. Open Jupyter Notebook in the Tensorflow virtual environment and navigate to the folder. 

### Using the saved model *islcnnmodel.h5*

1. Run ***Camera_Interface.ipynb*** to open live video capture. Predict in real time using hand gestures of the ISL.

### To create a new model from scratch

**Datasets:**
- [train_dataset](https://drive.google.com/drive/folders/1A6Swp8UDFqiYGzetnHADW7OkFozI5VVG?usp=sharing) : contains the original images for ISL
- [train_processed](https://drive.google.com/drive/folders/1jPZV32mCO1Rg6ZToVswSIp5-G9rkpAC3?usp=sharing) : contains the preprocessed images for training
- [test_processed](https://drive.google.com/drive/folders/1boqHZ2VhTFEtEZkrRvvJOHGHc1ye-dsH?usp=sharing) : contains the preprocessed images for testing

Download the datasets and place in the same folder.

You may use the three datasets directly or to create your own version of preprocessed images with specified dimensions and masking, run ***preprocessing.ipynb***. This automatically
preprocesses the images and stores them in the alphabet folder-wise manner. 

**Creating the Model:**

1. Run ***ISL_CNN.ipynb*** to create a new CNN model using the preprocessed images. CNN parameters may be changed according to your requirements. 
The model automatically creates a saved model named 'islcnnmodel1.h5'.
2. Load the model in ***Camera_Interface.ipynb*** and run to open live video capture. Predict in real time using hand gestures of the ISL.

## Workflow



