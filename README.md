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
Name: Preetha.S
Reg No: 212222230110
```

# Use Opening operation
```
import numpy as np
import cv2
import matplotlib.pyplot as plt
img1=np.zeros((100,400), dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'DataScience',(5,70), font,2,(255),5,cv2.LINE_AA)
kernel=np.ones((5,5),np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image1=cv2.morphologyEx(img1,cv2.MORPH_OPEN,kernel)
plt.imshow(image1)
plt.axis("off")
```



# Use Closing Operation
```
import numpy as np
import cv2
import matplotlib.pyplot as plt
img1=np.zeros((100,400), dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'DataScience',(5,70), font,2,(255),5,cv2.LINE_AA)
kernel=np.ones((5,5),np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image2=cv2.morphologyEx(img1,cv2.MORPH_CLOSE,kernel)
plt.imshow(image2)
plt.axis("off")

```
## Output:

### Display the input Image

![image](https://github.com/Preetha-Senthamilan/OPENING--AND-CLOSING/assets/119390282/e0fed96e-aab8-4c0d-ad76-dd3790aeef5b)



### Display the result of Opening

![image](https://github.com/Preetha-Senthamilan/OPENING--AND-CLOSING/assets/119390282/6e3dbfc6-f681-4cc2-ab28-8e37b4d92c3f)


### Display the result of Closing

![image](https://github.com/Preetha-Senthamilan/OPENING--AND-CLOSING/assets/119390282/e005d642-a921-4624-88f5-baf46c454df8)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
