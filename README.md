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
### Developed By:SHAIK KHADAR BASHA
### Register Number:212220230045
i) #To Read,display the image
```
  import cv2
  color_img=cv2.imread('KHADAR.jpeg',1)
  gray_img=cv2.imread('KHADAR.jpeg',0)
  cv2.imshow('KHADAR',color_img)
  cv2.imshow('KHADAR',gray_img)
  cv2.waitKey(0)
```
ii) #To write the image
```
 import cv2
 color_img=cv2.imread('KHADAR.jpeg',1)
 cv2.imwrite('KHADAR.jpeg',color_img)
 cv2.imshow('KHADAR',color_img)
 cv2.waitKey(0)


```
iii) #Find the shape of the Image
```
  import cv2
  import random
  color_img=cv2.imread('KHADAR.jpeg',1)
  print(color_img.shape)

```
iv) #To access rows and columns

```
  import cv2
  import random 
  for i in range (100):
      for j in range(color_image.shape[1]):
         color_image[i][j]= [random.randint (0,255), random.randint(0, 255), random.randint(0,255)]
      import matplotlib.pyplot as plt
  plt.imshow (color_image[200:670,200:670])

```
v) #To cut and paste portion of image
```
  import cv2
  color_img=cv2.imread('KHADAR.jpeg',-1)
  tag=color_image[150:200,150:200]
  color_image[25:75,25:75]=tag
  plt.imshow(color_image)
```

## Output:

### i) Read and display the image

![Read   Display image](https://user-images.githubusercontent.com/75235233/161425939-578aa576-5412-420e-ba4f-2e2b82fa3337.png)
![Read   Display Gray image](https://user-images.githubusercontent.com/75235233/161425947-a53ed142-27bb-4e86-b95e-49b90efd768b.png)

### ii)Write the image
![Write](https://user-images.githubusercontent.com/75235233/161425965-ee15bb1b-8130-48e4-a806-26198a5f7309.png)


### iii)Shape of the Image
![Write](https://user-images.githubusercontent.com/75235233/161425974-c87f85d6-5d1c-491f-9a32-15e7dbf4e2be.png)



### iv)Access rows and columns

![Access](https://user-images.githubusercontent.com/75235233/161425983-7d74084c-c42a-4c87-8cfc-b948241c16a2.png)

### v)Cut and paste portion of image
![Cut portion](https://user-images.githubusercontent.com/75235233/161425996-9c759e6a-b1f7-4880-922a-91869807d70d.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


