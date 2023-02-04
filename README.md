# Mouse-Cursor-Control-Sytem-Using-Gesture-Recognition

This model will contactlessly take inputs from the user and carry out all necessary actions, taking into account the useful aspects of virtual mouse operations. The steps that this model takes to accomplish this are as follows:

1) In ROI, the model will take user input in the form of hand gestures via webcam. To concentrate on gestures, I have marked the Region of Interest (ROI) with a green box in the output window. 

2) In order to accurately process the foreground gesture, the received image is processed with OpenCV and the background is subtracted from the ROI.

3) It will go through pre-processing steps like morphological transformation, applying a hand-drawn contour, and drawing the convex hull to remove noise.

4) The cursor's coordinates are determined by detecting the centroid of input while drawing the hand contour, and then the contour is extracted. 

5) The number of blobs has been counted. 

  5.1 Only one blob needs to be input if the cursor only needs to move across the screen. 
  5.2 However, left-clicking can be performed with two fingers. 
  5.3 Three or four fingers for performing the appropriate right click

TECHNOLOGY USED:

Python 3.9

OpenCV 4.5.1

NumPy

Win10 as OS
