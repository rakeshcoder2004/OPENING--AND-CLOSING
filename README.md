# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages


### Step2:
Read the image

### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

### Step6:
Display all the output images

 
## Program:
```
Developed By: Rakesh V
Register NO: 212222110036
```
``` Python
# Import the necessary packages
import cv2
import numpy as np

# Create the Text using cv2.putText
img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'AAKASH SURESH', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
cv2.imshow('created_text', img)
cv2.waitKey(0)

# Create the structuring element
struct_ele = np.ones((9, 9), np.uint8)

# Use Opening operation
opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)

# Use Closing Operation
closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)

# Close all windows
cv2.destroyAllWindows()
```
## Output:

### Display the input Image
![image](https://github.com/rakeshcoder2004/OPENING--AND-CLOSING/assets/121490890/d31dfeab-e9dd-47ec-84ec-45e1c9f28cd2)

### Display the result of Opening
![image](https://github.com/rakeshcoder2004/OPENING--AND-CLOSING/assets/121490890/ec0cbbd0-a264-4c37-8193-ff71d8b9b9a7)


### Display the result of Closing
![image](https://github.com/rakeshcoder2004/OPENING--AND-CLOSING/assets/121490890/aec999cb-215a-457f-97b8-cad42fea2bde)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
