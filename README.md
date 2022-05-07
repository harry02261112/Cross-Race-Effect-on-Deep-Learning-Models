# Cross-Race-Effect-on-Deep-Learning-Models

### Groups
* < Yu-Han (Harry) Lin >
* < Abdullah Yousuf >
* < Meng-Hsuan (Michelle) Wu >
* < Feng-Chiao Lee >

### Abstract 

The Cross-Race Effect refers to the effect that people are better at recognizing faces of people of their own race, rather than those of a different race and we are wondering if the machine learning algorithm would encounter the same issue. From our experiment we found basic model like VGG does has subtle cross race effect. However, deeper model like Resnet 50 does not. Possibly due to deeper networks considers more than the superficial features from the image data. Object detection model, on the other hand, performs well on all datasets. It only shows subtle cross-race effect. This might simply be the result that deep learning models are data driven.

### Objective 
* Training object detection models (Yolov5) on specific racial groups and test the model to see if it is able to capture faces of people of other racial groups.
* Training different classification models with the same two structures(Resnet 50 and VGG 16) on each race respectively to classify their age groups. Then observe the predicted accuracy of each trained model on the data that has a different race to it's training data.

### Datasets

* UTKFace data:
    * Two varieties: cropped and uncropped
    * Labels: age, race, gender, date
    * Quantity
        * over 20,000 face images
    * Age Range: 0 to 116
        * Classify image into one of 7 age ranges: 
        0-9, 10-19, 20-29, 30-39, 40-49, 50-59, 60+
    * Race: 5 categories


### Usage
```
./Cross_Race_Effects_on_Resnet_VGG 
```
Contains scripts to train Resnet and VGG on different race datasets
alone with the feature extraction and visualization codes
```
./Cross_Race_Effects_on_yolov5/yolo_each_race_script
```
Contains scripts to train yolov5 on different raace datasets 

### results
