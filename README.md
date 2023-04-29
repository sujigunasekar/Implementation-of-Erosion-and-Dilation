# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
Algorithm:
## Step1:
Import the necessary packages.

## Step2:
Create the Text using cv2.putText.

## Step3:
Create the structuring element.

## Step4:
Erode the image using cv2.erode().

## Step5:
Dilate the image using cv2.dilate().


 
## Program:

``` Python
# Import the necessary packages
import numpy as np
import cv2
import matplotlib.pyplot as plt

# Create the Text using cv2.putText
img1=np.zeros((100,500),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX_SMALL

# Create the Text using cv2.putText
cv2.putText(img1,'SUJI G',(10,90),font,2,(255),5,cv2.LINE_AA)
plt.imshow(img1,cmap='gray')

# Create the structuring element
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))

# Erode the image
img_erode=cv2.erode(img1,kernel1)
plt.imshow(img_erode,cmap='gray')

# Dilate the image
img_dilate=cv2.dilate(img1,kernel1)
plt.imshow(img_dilate,cmap='gray')

```
## Output:

### Display the input Image
![OL](https://user-images.githubusercontent.com/119559822/235293436-71df0c55-5642-4ffe-bc7c-44ef3474dc0a.png)


### Display the Eroded Image
![OL2](https://user-images.githubusercontent.com/119559822/235293454-be583150-6d23-46f8-9084-d9b5ba62c46a.png)


### Display the Dilated Image
![;L](https://user-images.githubusercontent.com/119559822/235293466-93cc5bde-94a2-4858-8c84-d8715d52fdd6.png)


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
