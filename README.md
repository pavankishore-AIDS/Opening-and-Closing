# Opening-and-Closing

## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step 1:
Import the necessary packages.

### Step 2:
Read the image.

### Step 3:
Create the structuring element.

### Step 4:
Use Opening operation.

### Step 5:
Use Closing Operation.

### Step 6:
Display all the output images.

 
## Program:

``` Python
# Developed By   : Pavan Kishore.M
# Register Number: 2122212300076

# Import the necessary packages

import cv2
import matplotlib.pyplot as plt

# Opening The Image

img=cv2.imread("vin.png")
plt.imshow(img)

# Create the structuring element

kernel=cv2.getStructuringElement(cv2.MORPH_CROSS,(11,11))

# Use Opening operation

img1=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernel)
plt.imshow(img1)

# Use Closing Operation

img2=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernel)
plt.imshow(img2)

```
## Output:

### Display the input Image
![v1](https://github.com/pavankishore-AIDS/Opening-and-Closing/assets/94154941/680e76fa-90f0-49cb-aabc-286a8c300a6e)

### Display the result of Opening

![v24](https://github.com/pavankishore-AIDS/Opening-and-Closing/assets/94154941/2d923daf-e898-468b-9ef3-3a46560a06a6)

### Display the result of Closing
![v3](https://github.com/pavankishore-AIDS/Opening-and-Closing/assets/94154941/7820aa77-0fb8-412b-8ea4-56b47692bb5b)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
