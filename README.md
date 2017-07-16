# Hand-gesture-recognition

### INTRODUCTION
This project implements a hand recognition and hand gesture recognition system using OpenCV on Python 2.7. A histogram based approach is used to separate out a hand from the background image. Background cancellation techniques are used to obtain optimum results. The detected hand is then processed and modelled by finding contours and convex hull to recognize finger and palm positions and dimensions. Finally, a gesture object is created from the recognized pattern which is compared to a defined gesture dictionary.

**Platform:** Python 3.5

**Libraries:** OpenCV 3, Numpy

**Hardware Requirements:** Camera/Webcam

### USAGE

Run HandRecognition.py to begin the program.

**Note for Windows users:**
Remove this line from all .py files: '#!/usr/bin/python' or else you might get some error.

You will find a window that shows your camera feed. Notice a rectangular frame on the right side of the window. That's the frame where all the detection and recognition works.

To begin, keep your hand and body outside the frame, so as to capture just the background environment, and press 'b'. This will capture the background and create a model of it. This model will be used to remove background from every frame captured once the program setup is complete. 

Now, you have to capture your hand histogram. Place your hand over the 9 small boxes in the frame so as to capture the maximum range of shades of your hand. Don't let any shadow or air gap show on the boxed areas for best results. Press 'c' to capture the hand and generate a histogram. 

The setup is now complete. Now you will see, by keeping your hand inside the rectangular frame, it gets detected and you will notice a circle inside your palm area, with lines projecting out from it towards your fingers. Try moving your hands, hiding a few fingers or giving it one of the sample gestures implemented in the program.
 

They are:

1. "V" with your index and middle finger

2. A flipped "L" with thumb and index finger

3. Pointing with your index finger in vertical position

**Note:** Press 'q' at any time to stop the program or 'r' to restart the program.
