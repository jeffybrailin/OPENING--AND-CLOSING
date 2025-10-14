## Name: Jeffy Brailin T
## Reg.No: 212223040076

# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

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
Use Opening operation.

### Step5:
Use Closing Operation.


 
## Program:

 
# Import the necessary packages
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```

# Create the Text using cv2.putText

```
img = np.zeros((100, 550), dtype = 'uint8')
font = cv2.FONT_ITALIC
cv2.putText(img, 'Ayisha Rinsi K', (5,70), font, 2, (255), 5, cv2.LINE_AA)
n_img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
plt.imshow(n_img)
plt.axis("off")

```


# Create the structuring element

```
kernel = cv2.getStructuringElement(cv2.MORPH_CROSS, (11,11)
```

# Use Opening operation

```
image_open = cv2.morphologyEx(n_img, cv2.MORPH_OPEN, kernel)
plt.imshow(image_open)
plt.axis("off")


```


# Use Closing Operation

```

image_open = cv2.morphologyEx(n_img, cv2.MORPH_OPEN, kernel)
plt.imshow(image_open)
plt.axis("off")


```
## Output:

### Display the input Image

<img width="654" height="147" alt="image" src="https://github.com/user-attachments/assets/507f02dc-aebe-4016-82af-e3f97655866d" />


### Display the result of Opening

<img width="648" height="132" alt="image" src="https://github.com/user-attachments/assets/098cdc65-3bd8-48ab-9ec4-63a70c9c91fc" />


### Display the result of Closing

<img width="653" height="135" alt="image" src="https://github.com/user-attachments/assets/9e1b512b-0bc8-4d0d-b445-60f7f741efdd" />

# Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
