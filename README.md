## EX 10: OPENING--CLOSING
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
Developed By: VISHAL M.A
Register NO: 212222230177
```
``` Python
# Import the necessary packages
import cv2
import numpy as np

# Create the Text using cv2.putText
img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'VISHAL', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
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
![vishal](https://github.com/vishal21004/OPENING--AND-CLOSING/assets/119560110/fb8e624b-530f-46e5-9fcb-084b231c4efe)


### Display the result of Opening
![vishal](https://github.com/vishal21004/OPENING--AND-CLOSING/assets/119560110/6c7b667c-e0f2-4086-b359-c2ea4948f0b3)


### Display the result of Closing
![vishal](https://github.com/vishal21004/OPENING--AND-CLOSING/assets/119560110/82600e71-3986-4322-b57c-cbe12341cc34)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
