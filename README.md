# Facemask Detection using CNN to contain the spread of COVID-19
    As this pandemic became new normal it is important to wear a face mask and make sure whether people around us wear a face mask. This project uses TensorFlow to classify whether person is wearing a facemask or not. Labelled data is used to train a model which is further tested on a different testing dataset. First single frame of image is fetched using OpenCV and passed to the viola-jones face detector. After the face detection it is passed to VGG16 which is a CNN architecture used to classify whether face ROI contains a face mask or not. Finally, boundary of boxes is drawn for all faces with their class probabilities.

## Usability
* Unzip the zipped folder on your machine.
* Import the project in PyCharm.  
* Install the dependencies from requirements.txt
* Run the mask_classifier.py to train the model.
* After the training is complete run the face_mask_detection.py to start program to detect face mask.

> face_mask_detection.py : Detects face using Viola Jones and classifies the face in the input video stream as masked or not using the saved model. 

> mask_classifier.py :  Loads and preprocesses the data before training the VGG16 model        and genrerates accuracy and classification report.
  
> maskclassifier.model : Stores the trained model to classify images as mask or without mask.

>requirements.txt : List of dependencies required.

>dataset : Contains images for training the model.


## Libraries Required:
* numpy~=1.22.3
* pandas~=1.4.1
* matplotlib~=3.5.1
* sklearn~=0.0
* tensorflow~=2.8.0
* keras~=2.8.0
* opencv-python~=4.5.5.64
* scikit-learn~=1.0.2


## Collaborators:
1. Akshar Awari aba7569@rit.edu
2. Shravan Kanchan sk4906@rit.edu
3. Rohan Parkar rp9679@rit.edu



