# Analog clock image training

```
Download the original dataset from kaggle https://www.kaggle.com/datasets/gpiosenka/time-image-datasetclassification
or from:
```
![dataset]("https://www.kaggle.com/datasets/gpiosenka/time-image-datasetclassification/download?datasetVersionNumber=5")


<h3>The Model is trained using the Convolutional Neural Network and the optimizer used to train is adam</h3>
<br>

***
# Information about the dataset

This dataset consists of synthetically generated images of clocks with the clock hands placed on one of 100 different clock faces.
The data set is divided into 144 classes . Classes are labelled in the form hour-min, so for a time like 1:30 the associate class label would be 1-30. The are 12 different hours and 12 different minutes for each hour yielding 12 hours X 12 minutes =144 classes.

<br>


The dataset is divided into train, test and valid subsets. Trained models from this dataset will NOT work well on predicting images downloaded from the internet because it was trained on rectangular hands of fixed length and rectangular shape, whereas hands for downloaded images will in general be different . Hands in the training images are in general black, however on darker clock faces the color of the hands can be of 5 different colors. The images in the dataset are also randomly rotated between 0,-90, +90 and 180 degrees. Did this to make classification a bit more difficult. 

The minute hand in the images always lay directly on one of the 12 minute locations, ie 0 5, 10, etc. The hour hands are adjusted away from the exact hour by the value of the minute hand. For example the hour hand for say time 1:30 is located half way between 1 and 2 on the clock face. 

All images in the dataset are 224 X 224 X 3 jpg format
