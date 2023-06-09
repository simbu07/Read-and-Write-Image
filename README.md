## Ex-1   READ AND WRITE AN IMAGE

### AIM:
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

### Software Required:
Anaconda - Python 3.7
### Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
### Program:
```
Developed By: Silambarasan K
Register Number: 212221230101
```
**i) To Read,display the image**
```python3

import cv2
pic=cv2.imread("img1.png",1)
cv2.imshow("212221240005",pic)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
**ii) To write the image**
```python3
import cv2
pic=cv2.imread("img1.png",1)
cv2.imshow("212221230101",pic)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
**iii) Find the shape of the Image**
```python3
import cv2
pic = cv2.imread('img1.png',1)
print(pic.shape)


```
**iv) To access rows and columns
**
```python3
 import random
import cv2
pic=cv2.imread("img1.png",1)
for i in range(100):
    for j in range(pic.shape[1]):
        pic[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("212221230101",pic)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
**v) To cut and paste portion of image**
```python3
import cv2
pic=cv2.imread("img1.png",1)
crop=pic[300:400,300:400]
pic[50:150,50:150]=crop
cv2.imshow("212221230101",pic)
cv2.waitKey(0)
cv2.destroyAllWindows()


```

### Output:

### i) Read and display the image

![r1](https://user-images.githubusercontent.com/94525786/225218666-34f686b1-9a50-48a2-98c8-7ba65618b96d.png)


### ii)Write the image

![r2](https://user-images.githubusercontent.com/94525786/225218754-cf05bcfa-950f-4e6f-87fa-47bd45b03dab.png)

### iii)Shape of the Image

![r3](https://user-images.githubusercontent.com/94525786/225218543-6af168af-49fb-4bc1-b34e-ce2476b89771.png)


### iv)Access rows and columns
![r4](https://user-images.githubusercontent.com/94525786/225218549-816133fb-4cb6-455b-970d-dce2ec695b51.png)


### v)Cut and paste portion of image

![r5](https://user-images.githubusercontent.com/94525786/225218618-8a1b3827-fc61-4ac5-9097-5c1967bffba3.png)

### Result:
Thus the images are read, displayed, and written successfully using the python program.


