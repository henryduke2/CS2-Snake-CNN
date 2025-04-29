# Venomous Snake Detection
Case study github repo

## Contents

A convolutional neural network running a binary classification whether a snake is venomous or nonvenomous based on images from 4 different North American species. The snakes images used to build the model are the diamondback, sidewinder, green snake, and gartner snake.

## Software and Platform 

The platforms used to run this project are Google Colab and Jupyter Notebook, with the following packages utilized: zipfile, os, ImageDataGenerator from tensorflow.keras.preprocessing.image, pandas, numpy, matplotlib.pyplot, tensorflow, shutil, MobileNetV2 from tensorflow.keras.applications, Sequentiel from tensorflow.keras.models, GlobalAveragePooling2D from tensorflow.keras.layers, Dense from tensorflow.keras.layers, Dropout from tensorflow.keras.layers, classification_report, confsuion_matrix, ConfusionMatrixDisplay, accuracy_score, precision_score, recall_score, f1_score all from sklearn.metrics. The image data was downloaded from images.cv and manipulated into one snake.zip file with all four species of snake. The zipfile and os functions were used to read the zip file into the coding platforms. A GPU through UVA Rivanna systems was used with 56 gigabytes of storage, 1 core, and 2 hours of run time. This project was executed on both mac and windows platforms.

## Map 

### DATA folder:
- Snake Photos: A link to a seperate repository (https://github.com/henryduke2/snake-cnn-project) which contains a zip file of all snake images divided into training and testing sets and classified as venomous or nonvenomous within each set. All photos were downloaded from the site images.cv
- Data_Appendix.pdf: The data appendix with all data sets and variables explained.

### SCRIPTS
- 1_Preprocessing_and_EDA: Processing the image data into python and performing explanatory data analysis.
- 2_Snake_Model: Processing the image data into python and running a pre-trained convolutional neural network to classify which snake photos are venomous and nonvenomous.

## LICENSE
- MIT License dictating how this data and analysis can be used.

## Reproducing Results

To start reproduicng results, you first must access the examplezip file of all of the snake photos from the seperate repository. Within this zip file, the images are already seperated into train and test data. Within each train and test folder, they are seperated into venomous and nonvenomous folders containing the images of the snake. All images are from images.cv. Feel free to add more species of snake from the site to create a more useful and predictvie model.

Once the file is downloaded, the images are processed in the beginning of both scripts. Open the 1_Preprocessing_and_EDA script to process the image to and to analyze the exploratory data analysis which will show you properties, dimensions, and sample of the snake data.

Next, you will open the 2_Snake_model script. Within this script you will be able to process the image data, use MobileNetV2 to create a convolutional neural network model, and analyze the performance statistics of the model.
