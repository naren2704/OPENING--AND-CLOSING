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
Developed By: NARENDRAN.B
Register NO: 212222240069
```
``` Python
# Import the necessary packages
import cv2
import numpy as np

# Create the Text using cv2.putText
img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'JANANI.V.S', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
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

![WhatsApp Image 2024-04-23 at 10 41 12_4b6f46bc](https://github.com/naren2704/OPENING--AND-CLOSING/assets/118706984/f3ce33b8-22e2-4191-8643-3f87e9b6810c)


### Display the result of Opening

![WhatsApp Image 2024-04-23 at 10 41 26_62f3aeec](https://github.com/naren2704/OPENING--AND-CLOSING/assets/118706984/3b81b189-714a-4521-aa72-7cca2365b3d3)



### Display the result of Closing

![WhatsApp Image 2024-04-23 at 10 41 40_e7de2cec](https://github.com/naren2704/OPENING--AND-CLOSING/assets/118706984/eb522f78-927d-4b6e-9432-092819d65cd4)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
