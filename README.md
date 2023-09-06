# COLOR-CONVERSION
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Import opencv
<br>

### Step2:
Read the original Image.
<br>

### Step3:
Store the required conversion of the image in a variable.
<br>

### Step4:
Show the image stored in the given variable.
<br>

### Step5:
Destroy all the windows and end the program.
<br>

## Program:
### Developed By: Aldrin Lijo J E
### Register Number:2122222240007
### i) Convert BGR and RGB to HSV and GRAY
```
import cv2
starry = cv2.imread('b.jpeg')
cv2.imshow('Original Image', starry)
hsv_image = cv2.cvtColor(starry,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV',hsv_image)
hsvImage1=cv2.cvtColor(starry,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV',hsvImage1)
grayImage = cv2.cvtColor(starry,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',grayImage)
grayImage1 = cv2.cvtColor(starry,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',grayImage1)
cv2.waitKey(0)
cv2.destroyAllWindows()


```
### ii)Convert HSV to RGB and BGR
```
import cv2
hsv_image2 = cv2.imread('b.jpeg')
cv2.imshow('Original HSV Image',hsv_image2)
RGBImage = cv2.cvtColor(hsv_image2,cv2.COLOR_HSV2RGB)
cv2.imshow('BGR2HSV',RGBImage)
BGRImage = cv2.cvtColor(hsv_image2,cv2.COLOR_HSV2BGR)
cv2.imshow('RGB2HSV',BGRImage)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
### iii)Convert RGB and BGR to YCrCb
```
import cv2
boom = cv2.imread('b.jpeg')
cv2.imshow('Original HSV Image',boom)
YCrCb_image = cv2.cvtColor(boom, cv2.COLOR_RGB2YCrCb)
cv2.imshow('BGR2HSV',YCrCb_image)
YCrCb_image1 = cv2.cvtColor(boom, cv2.COLOR_BGR2YCrCb)
cv2.imshow('RGB2HSV',YCrCb_image1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
### iv)Split and Merge RGB Image
```
import cv2
image = cv2.imread('b.jpeg')
blue = image[:,:,0]
green = image[:,:,1]
red = image[:,:,2]
cv2.imshow('B-Channel',blue)
cv2.imshow('G-Channel',green)
cv2.imshow('R-Channel',red)
mergeBgr = cv2.merge((blue,green,red))
cv2.imshow('Merged BGR image',mergeBgr)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
### v) Split and merge HSV Image
```
import cv2
image = cv2.imread('b.jpeg')
hsv = cv2.cvtColor(image,cv2.COLOR_BGR2HSV)
h,s,v = cv2.split(hsv)
cv2.imshow('Hue - Image',h)
cv2.imshow('Saturation - Image',s)
cv2.imshow('Gray - Image',v)
mergedHSV = cv2.merge((h,s,v))
cv2.imshow('Merged HSV Image',mergedHSV)
cv2.waitKey(0)
cv2.destroyAllWindows()
```




## Output:
### i) BGR and RGB to HSV and GRAY
![org](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/0c9deca2-73bf-4b67-8cbe-081e050f70a2)
![rgb2hsv](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/aa4b5d22-134c-4b35-9306-9af9e6bb0338)
![bgr2hsv](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/0a9a66a7-92ee-4bc8-a101-51b3800029ab)
![rgb2gray](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/6d6ef58d-804c-43d4-b49e-f4ac169b998b)
![rgb2hsv](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/a35dfdcb-af41-408f-957d-5498973923ce)

<br>
<br>

### ii) HSV to RGB and BGR
![2](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/f2b3b371-357b-479f-a64f-44818bd8b4ac)

![2(1)](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/75e05a2e-1c1c-4b9d-9708-92b9c39aaf2c)

![image](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/cec61ddb-f944-4320-ace2-02b7a6522da0)

<br>
<br>

### iii) RGB and BGR to YCrCb
![3(1)](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/6d50d833-1e13-44f9-8f9a-86427e1c881b)

![3(2)](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/8b7697c0-8d9c-48ca-94c3-7206af200284)

![3(3)](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/673a951d-e364-459d-93a8-0516df6d5455)

<br>
<br>

### iv) Split and merge RGB Image
![4(1)](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/3bffc00f-beec-44da-81fe-f23cf4546c7c)

![4(2)](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/4dfc2e4a-d26d-46b4-8c36-e40fbb47aebe)

![4(4)](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/0b9dd05a-599c-4043-badd-58f526add4eb)

![4(3)](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/39b90418-2a60-41ff-9d71-91c6e7b0b350)

<br>
<br>

### v) Split and merge HSV Image

![5(1)](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/061fd679-b274-412c-af06-9878c33c9fab)

![5(2)](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/a0c077d9-9af3-4ab6-961c-64b3341ebbbf)

![5(3)](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/92b0130a-d19e-428e-935b-b220aa03aaa6)

![5(4)](https://github.com/aldrinlijo04/COLOR-CONVERSION/assets/118544279/97bedfd8-f807-4dc6-8e9c-96e34f7fcd27)

<br>
<br>


## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
