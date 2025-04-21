# Ship-Detection-in-Satellite-Imagery-using-Deep-Learning
## Project Summary

Deep learning-based ship detection satellite imagery using HRSC2016 dataset is the goal of the project. 
The Convolutional Neural Network (CNN) has been used to identify and locate the ships from high-resolution satellite images with the maximum validation accuracy of 92%. 
Besides that, an unsupervised classification model has also been developed which will classify the detected ships into different types based on their visual appearances and characteristics.

## Features
***Ship Detection:*** Satellite picture ship detection with custom CNN model approach for accurate detection.

***Classification of Ships:*** Unsupervised clustering is used for ship classification.

***Interactive Visualization:*** Mechanisms are provided for visual exploration of detection results and ship extraction.

***Sliding Window Detection:*** A sliding window is implemented with non-maximum suppression.

***Balanced Dataset Creation:*** Training data has been developed so that positive and negative samples are balanced.

## Dataset

This project uses the HRSC2016 (High-Resolution Ship Collections 2016) dataset and contains:

+ High-resolution satellite imagery of maritime environment
+ XML annotations with bounding box coordinates for ships
+ Many types, sizes, and orientations of ships
+ The scale and richness of backgrounds including harbors, open sea, and coastal areas

## Ship detection model construction
+ This ship detection model is made up of:
+ Four increasingly bigger convolutional blocks, which range from 32 to 64, 128, and finally, 256 filters.
+ Each convolutional block is followed by batch normalization and maximum pooling at the end.
+ Connected layers at the very end have been regularized using dropout. 
+ Lastly, there is the softmax output layer useful for binary classification of ship versus non-ship classes.

## Results

+ ~95%: Training Accuracy
+ ~92%: Validation Accuracy 
+ ***Performance regarding detection:*** Detecting ships of all sizes, even among the most complex of backgrounds.
+ ***Classification:*** Identifying categories of vessels found through unsupervised learning.

## Requirements
+ Python 3.7
+ TensorFlow 2.4
+ OpenCV 4.5
+ NumPy 1.19
+ Matplotlib 3.3
+ scikit-learn 0.24

## Future Improvements
+ More advanced architectures would be implemented (YOLO, Faster R-CNN).
+ Transfer learning with pre-trained models would be added.
+ Supervised classification would be developed for ship types.
+ Real-time optimization will be done.
+ Create an interactive web interface for detection.
  
## Licensing
This project is licensed under the MIT License.

## Acknowledgements
+ The ship detection benched data set ticketed towards the HRSC2016 dataset creators.
+ TensorFlow and Keras teams have used their deep learning framework as part of the teams' working efforts.
+ The OpenCV community has also been right on target for providing computer vision tools.
