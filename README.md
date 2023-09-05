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
houseImage = cv2.imread('pic.jpeg')
cv2.imshow('Original HSV Image',houseImage)
YCrCb_image = cv2.cvtColor(houseImage, cv2.COLOR_RGB2YCrCb)
cv2.imshow('BGR2HSV',YCrCb_image)
YCrCb_image1 = cv2.cvtColor(houseImage, cv2.COLOR_BGR2YCrCb)
cv2.imshow('RGB2HSV',YCrCb_image1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
### iv)Split and Merge RGB Image
```
import cv2
image = cv2.imread('pic.jpeg')
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
image = cv2.imread('pic.jpeg')
hsv = cv2.cvtColor(image,cv2.COLOR_BGR2HSV)
h,s,v = cv2.split(hsv)
cv2.imshow('Hue - Image',h)
cv2.imshow('Saturation - Image',s)
cv2.imshow('Gray - Image',v)
mergedHSV = cv2.merge((h,s,v))
cv2.imshow('Merged HSV Image',mergedHSV)
cv2.waitKey(0)
cv2.destroyAllWindow
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
![Screenshot 2023-08-31 223209](https://github.com/Yamunaasri/COLOR-CONVERSION/assets/115707860/b3e792e3-dede-4b9f-9e23-0f46f48e0bc2)


![Screenshot 2023-08-31 223840](https://github.com/Yamunaasri/COLOR-CONVERSION/assets/115707860/8a6b5301-7f65-48d3-8a9b-5d2cfc1fddf4)


![Screenshot 2023-08-31 223850](https://github.com/Yamunaasri/COLOR-CONVERSION/assets/115707860/957b3893-5393-41d5-98b4-fb792b705a66)

<br>
<br>

### iv) Split and merge RGB Image
![Screenshot 2023-08-31 224046](https://github.com/Yamunaasri/COLOR-CONVERSION/assets/115707860/4c66f5dd-fd1d-460c-830b-fc12febbe9e4)

![Screenshot 2023-08-31 224100](https://github.com/Yamunaasri/COLOR-CONVERSION/assets/115707860/a828f477-bdd1-435a-b2bd-37469798915c)

![Screenshot 2023-08-31 224109](https://github.com/Yamunaasri/COLOR-CONVERSION/assets/115707860/88e83cc3-1e65-4779-8307-1fc6ef1d1229)

![Screenshot 2023-08-31 224121](https://github.com/Yamunaasri/COLOR-CONVERSION/assets/115707860/273aa11f-2365-4205-a7c3-19af58309887)

<br>
<br>

### v) Split and merge HSV Image

![Screenshot 2023-08-31 224353](https://github.com/Yamunaasri/COLOR-CONVERSION/assets/115707860/50eccce3-9396-45cb-9dd3-ecf28fe84a24)

![Screenshot 2023-08-31 224404](https://github.com/Yamunaasri/COLOR-CONVERSION/assets/115707860/1b90bdcc-c3a3-47f2-86f2-b66e0d3b6f0f)

![Screenshot 2023-08-31 224415](https://github.com/Yamunaasri/COLOR-CONVERSION/assets/115707860/481486cc-fcf8-430f-aa8d-97e2b6222f6a)

![Screenshot 2023-08-31 224430](https://github.com/Yamunaasri/COLOR-CONVERSION/assets/115707860/648ae816-2dbc-4f61-98d5-b4f7a81c2a33)

<br>
<br>


## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
