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
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By: Sanjay Kumar S S
### Register Number: 212221240048
i) #To Read,display the image
```
import cv2

img = cv2.imread("zoro.png")
cv2.imshow("read_pic",img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
ii) #To write the image
```
cv2.imwrite("write_pic.png",img)
```
iii) #Find the shape of the Image
```python3
print(img.shape)
```
iv) #To access rows and columns

```python3
img = cv2.imread("zoro.png")
for i in range(350,400):
    for j in range(800,1100):
        img[i][j] = [104, 104, 104]
cv2.imshow("row_pic.png",img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
v) #To cut and paste portion of image
```python3
img = cv2.imread("zoro.png")
img[700:1000,600:900] = img[300:600,1100:1400]
cv2.imshow("cut_pic.png",img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

## Output:

### i) Read and display the image

<br>
<img height = "350" src="https://user-images.githubusercontent.com/93427246/224912715-a4bde0bf-810f-4381-a0d1-73c31c8a0745.png">
<br>


### ii)Write the image

<br>
<img height = "350" src="https://user-images.githubusercontent.com/93427246/224912824-b835017c-7fd8-4df2-a8f6-5aaab411a4a4.png">

<br>

### iii)Shape of the Image

<br>
<img height = "250" src="https://user-images.githubusercontent.com/93427246/224912942-d8d67a54-75d9-4546-975b-36bc6bae11f0.png">

<br>

### iv)Access rows and columns
<br>
<img height = "350" src="https://user-images.githubusercontent.com/93427246/224913008-322c2baf-2b97-45de-b8ca-49d4c2d00833.png">
<br>

### v)Cut and paste portion of image
<br>
<img height = "350" src="https://user-images.githubusercontent.com/93427246/224913070-e416ddfb-31e0-46ac-a0a9-93e322199a66.png">

<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


