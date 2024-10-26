# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
 
## Algorithm:
### Step1:
Import the necessary packages

### Step2:
Create the Text using cv2.putText
### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation



 
## Program:
```
Name : LISIANA T
Register no : 2122222240053
```

#### Import the necessary packages

``` Python
import numpy as np
import cv2
import matplotlib.pyplot as plt
```

#### Read and show the Original image

``` Python
image = cv2.imread("fp.jpg")
kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (5, 5))
image_rgb = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
plt.imshow(image_rgb)
plt.title("Original Image")
plt.axis("off")
```



#### Use Opening operation

```
opening_image = cv2.morphologyEx(image, cv2.MORPH_OPEN, kernel)
opening_image_rgb = cv2.cvtColor(opening_image, cv2.COLOR_BGR2RGB)
plt.imshow(opening_image_rgb)
plt.title("Opening Operation")
plt.axis("off")
```


#### Use Closing Operation

```
closing_image = cv2.morphologyEx(image, cv2.MORPH_CLOSE, kernel)
closing_image_rgb = cv2.cvtColor(closing_image, cv2.COLOR_BGR2RGB)
plt.imshow(closing_image_rgb)
plt.title("Closing Operation")
plt.axis("off")


```
## Output:

### Display the Original Image

![Screenshot 2024-10-26 112102](https://github.com/user-attachments/assets/d92dcb2e-5091-4d01-a47d-d3ad9a8559d5)


### Display the result of Opening
![Screenshot 2024-10-26 112108](https://github.com/user-attachments/assets/a7f90968-e7cd-4dec-a2e2-63e05f629d24)


### Display the result of Closing
![Screenshot 2024-10-26 112115](https://github.com/user-attachments/assets/17ed5392-129f-41b6-88d2-fd7d301480fa)



## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
