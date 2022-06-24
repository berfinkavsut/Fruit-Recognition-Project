# Fruit Recognition Project

This project was implemented for the summer internship in HAVELSAN in the summer 2020. The task is to detect fruits in images after classification. 

Classification was implemented firstly, and then object detection was done by these following object detection algorithms. 

## Fundamental Algorithms Used in the Object Detector [1]

**1. Image Pyramid**

Image pyramid is a multi-scale representation of an image. The images are resized by subsampling until a stopping criteria.

**2. Sliding Window**

This method is used for sliding the region of interests (ROI) from created image pyramids to
have predictions from image classifier.

**3. Non-Maxima Suppression (NMS)**

After applying image pyramid and sliding window algorithms, the detected boxes from our
CNN image classifier yields overlapping detection boxes for certain classes. NMS gets rid of
the weak overlapping bounding boxes by comparing the confidence ration of other bounding
boxes. So that, multiple detections for one object is avoided.

## Training Models 
Two different classification models were trained. Training and validation graphs were plotted. Confusion matrices were displayed. Prediction result image for classification , and later for object detection were displayed. You cna find the results in summer internship report inside this repository. 

## References 
[1] Rosebrock, Adrian. "Turning Any Cnn Image Classifier Into an Object Detector with Keras, Tensorflow, and Opencv." PyImageSearch. June 22, 2020. https://www.pyimagesearch.com/2020/06/22/turningany-cnn-image-classifier-into-an-object-detector-with-keras-tensorflow-and-opencv/
