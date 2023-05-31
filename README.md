# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV

## Algorithm:
### Step1:
Import the necessary packages.
### Step2:
Create the Text using cv2.putText.
### Step3:
Create the structuring element.
### Step4:
Erode and Dilate the image.
### Step5:
End Program.

## Program:
```
DEVELOPED BY : Dineshkumar S
REG NO :2122202300012
```
``` Python
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt
# Create the Text using cv2.putText
img1 = np.zeros((100,270), dtype = 'uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'Dinesh',(5,70), font, 2,(255),5,cv2.LINE_AA)
plt.imshow(img1,'gray')
# Create the structuring element
cv2.erode(img1, kernel)
kernel = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
# Erode the image
image_erode1 = cv2.erode(img1,kernel)
plt.imshow(image_erode1, 'gray')
# Dilate the image
image_dilate1 = cv2.dilate(img1, kernel)
plt.imshow(image_dilate1, 'gray')
```
## Output:

### Input Image
![SS1](https://user-images.githubusercontent.com/75234807/173192011-2caaa3cc-45e9-4e6b-bb83-ec62efe7f05f.png)

### Eroded Image
![SS 2](https://user-images.githubusercontent.com/75234807/173192001-2c6f185b-f6ab-49f6-a6f5-59eca937c2a4.png)

### Dilated Image
![SS3](https://user-images.githubusercontent.com/75234807/173192028-61c2823c-ffa1-4d62-b07e-53155c033925.png)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
