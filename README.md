# Fish-Identification-using-Siamese CNN

Demo video available (skip till minute 4 to check fish identification)

## Introduction
In this project, we tackle the issue of fish species recognition. It is a very tedious and time consuming task if done manually.
Traditionally, cnns are the state of the art models to classify images (typically using softmax to give a probability distribution over classes. However, cnns have two major drawbacks, the first being the very large number of samples required per class, and the need to retrain if a new class is to be introduced

## Dataset 
The dataset used is composed of 468 classes corresponding to 4415 images; averaging ~10 images per class. It is clear that a traditional cnn approach is not possible
Additionally, we have scrapped and labelled google images for 220 species using python scripts 

## Conclusion
A testing accuracy of 66% was achieved and an f-measure of 0.65 vs 1.5% accuracy for a baseline rbf svm
We have successfully trained on 107 species, with the ability to dynamically add new classes without the need to retrain; this is achieved because we are not actually classifying images into classes but rather finding an index of similarity between two given images. In theory, any number of species can be added if at least one labelled image per class is introduced

![sample1](/Picture1.png)
