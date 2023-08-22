# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg.
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By:Lokesh N
### Register Number: 212222100023
i) #To Read,display the image
```python
import cv2
image=cv2.imread("tree.png",1)
cv2.imshow("212222100023_lokesh",image)
cv2.waitKey(0)
cv2.destroyAllwindows()

  

```
ii) #To write the image
```python
import cv2
image=cv2.imread("tree.png",1)
cv2.imwrite("tree.png",image)
cv2.imshow("212222100023-lokesh",image)
cv2.waitKey(0)
cv2.destroyAllwindows()



```
iii) #Find the shape of the Image
```python3
import cv2
picture=cv2.imread("tree.png",1)
print(picture.shape)


```
iv) #To access rows and columns

```python3
import random
import cv2
image=cv2.imread("tree.png",1)
for i in range(100):
    for j in range(image.shape[1]):
        image[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("212222100023-lokesh",image)
cv2.waitKey(0)
cv2.destroyAllwindows()


```
v) #To cut and paste portion of image
```python3
import cv2
img = cv2.imread('tree.png', 1)
tag = img[50:110:, 50:110]
img[120:180, 120:180] = tag
cv2.imshow('212222100023-lokesh', img)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image
![Screenshot from 2023-08-22 22-12-59](https://github.com/lokeshnarayanan/READ-AND-WRITE-IMAGE/assets/119393019/9db68d41-95dd-4cc0-8780-1000b037eeb7)


### ii)Write the image

![Screenshot from 2023-08-22 22-18-17](https://github.com/lokeshnarayanan/READ-AND-WRITE-IMAGE/assets/119393019/aec73550-bca2-42ab-9725-378ccbec9b42)


### iii)Shape of the Image

![Screenshot from 2023-08-22 22-19-19](https://github.com/lokeshnarayanan/READ-AND-WRITE-IMAGE/assets/119393019/acadc7d4-1281-4d35-b482-966d73aad7f4)


### iv)Access rows and columns
![Screenshot from 2023-08-22 22-38-23](https://github.com/lokeshnarayanan/READ-AND-WRITE-IMAGE/assets/119393019/530cec4f-9ff0-42cb-9710-d367568bcd9b)


### v)Cut and paste portion of image

![Screenshot from 2023-08-22 22-33-21](https://github.com/lokeshnarayanan/READ-AND-WRITE-IMAGE/assets/119393019/907f99dc-ae9c-4b8e-a4e2-1c5ecfe83c9b)

## Result:
Thus the images are read, displayed, and written successfully using the python program.
