# COVID-19-chest-X-ray-analysis
The aim of this work is to develop a model to classify X-ray images of the chest to detect COVID-19 positive cases by using transfer learning based on the VGG-19.

Data Source : The data set for this implementation is taken from kaggle COVID-19 Radiography Database -  https://www.kaggle.com/tawsifurrahman/covid19-radiography-database

# Background
Since the beginning of 2020, COVID-19 had a large impact on the entire world. The concerning infection rate makes governments to take actions to limit social interactions, with consequences for trade, transport and economy – resulting in in the shutdown of countries and job loss for many people.

An accurate diagnosis is challenged by time and staff, resulting from shortcomings in personal resources and the pressure of detecting COVID-19 without delaying diagnosis. However, an accurate diagnosis is crucial – wrong diagnosis carry the risk of worsen the pandemic in case COVID-19 positive patients get misdiagnosed (false negatives) and thus do not isolate.

To address the time constrains, research uses deep learning techniques to extract the information needed from those medical images to save critical time (Ilyas et al., 2020; Shoeibi et al., 2020, 2020). A successful model would address the need of screening patients accurately in real-time and enable an instant clinical reaction (Asif et al., 2020). As a first step towards a screening tool, an algorithm is needed that can detect COVID-19 form X-ray images.


# Goal
Develop a model to classify X-ray images of the chest to detect COVID-19 positive cases by using transfer learning based on the VGG-19.

# Files

# Specifications

Requirements: Python 3.8, Keras, Tensorflow

Data Source : The data set for this implementation is taken from kaggle COVID-19 Radiography Database - https://www.kaggle.com/tawsifurrahman/covid19-radiography-database

Data descritpion: The dataset contains 219 COVID-19 images, 1,345 pneumonia images and 1,341 healthy images, for a total of 2,905 images. The images are uniformly formatted, labelled and sized, and ready to be fed into the model for analysis.

Pre-processing: down-sizing the images from 1024x1024 pixel to 224x224 pixel to minimize the processing time of the model

Train-Test-Split: 33%, stratified sampling

Model Architecture: VGG-19 (frozen weights), additional layers (one functional layer, two drop out layers, three dense layers, softmax activation function in the final layer)

