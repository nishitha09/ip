

**PROGRAM 1: DEVELOP A PROGRAM TO DISPLAY GRAY SCALE IMAGE USING READ AND WRITE OPERATION:**
   
 import cv2<br>
 img=cv2.imread('b1.jpg',0)<br>
 cv2.imshow('b1',img)<br>
 cv2.waitKey(0)<br>
 cv2.destroyAllWindows()<br>
  
**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178444060-1c6d34fd-3ebe-4127-87cc-94a2fb7e1861.png)

**PROGRAM 2: DEVELOP A PROGRAM TO DISPLAY IMAGE USING MATPLOTLIB**
 
 import matplotlib.image as mping<br>
 import matplotlib.pyplot as plt<br>
 img=mping.imread('f2.jpg')<br>
 plt.imshow(img)<br>
 
 **OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178444384-50f41d8f-61f0-43bb-bd01-2a68218079d8.png)
 
**PROGRAM 3:DEVELOP A PROGRAM TO PERFORM LINEAR TRANSFORMATION:**

from PIL import Image<br>
img=Image.open('l1.jpg')<br>
img=img.rotate(180)<br>
img.show()<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178444653-1645cde6-84ab-425c-b2e0-2285b07781bf.png)

**PROGRAM 4:DEVELOP PROGRAM TO CONVERT COLOR STRING TO RGB COLOR VALUES:**

from PIL import ImageColor<br>
img1=ImageColor.getrgb("yellow")<br>
print(img1)<br>
img2=ImageColor.getrgb("red")<br>
print(img2)<br>
img3=ImageColor.getrgb("pink")<br>
print(img3)<br>
img4=ImageColor.getrgb("blue")<br>
print(img4)<br>

**OUTPUT:<br>**
(255, 255, 0)<br>
(255, 0, 0)<br>
(255, 192, 203)<br>
(0, 0, 255)<br>

**PROGRAM 5:DEVELOP PROGRAM TO CREATE IMAGE USING COLORS:**

from PIL import Image<br>
img=Image.new("RGB",(200,400),(0, 0, 255))<br>
img.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939284/173813696-f552419d-9b39-4595-bf01-92f689afc915.png)

**PROGRAM 6:DEVELOP A PROGRAM TO VISUALIZE THE IMAGE USING VARIOUS COLOR SPACE:**

import cv2<br>
import matplotlib.pyplot as plt<br>
import numpy as np<br>
img=cv2.imread('6.jpg')<br>
plt.imshow(img)<br>
plt.show()<br>
img=cv2.cvtColor(img,cv2.COLOR_BGR2RGB)<br>
plt.imshow(img)<br>
plt.show()<br>
img=cv2.cvtColor(img,cv2.COLOR_RGB2HSV)<br>
plt.imshow(img)<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178444941-22505385-1d9e-497a-9573-ff70bff7a87c.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178446532-b9b97c60-93f3-4583-9bfb-e02d172978cb.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178446664-c6bdb21f-d7b9-406c-bfa0-f0f100434534.png)<br>

**PROGRAM 7:WRITE A PROGRAM TO DISPLAY IMAGE ATTRIBUTE:**

from PIL import Image<br>
image=Image.open('16.jpg')<br>
print("Filename:",image.filename)<br>
print("Format:",image.format)<br>
print("Mode:",image.mode)<br>
print("size:",image.size)<br>
print("Width:",image.width)<br>
print("Height:",image.height)<br>
image.close()

**OUTPUT:<br>**
Filename: 16.jpg<br>
Format: JPEG<br>
Mode: RGB<br>
size: (600, 398)<br>
Width: 600<br>
Height: 398<br>

**PROGRAM 8:CONVERT ORIGINAL IMAGE TO GRAY SCALE AND THEN TO BINARY:** 

import cv2<br>
#read the image file<br>
img=cv2.imread('b2.jpg')<br>
cv2.imshow("RGB",img)<br>
cv2.waitKey(0)<br>
#gray scale<br>
img=cv2.imread('b2.jpg',0)<br>
cv2.imshow("Gray",img)<br>
cv2.waitKey(0)<br>
#Binary image<br>
ret,bw_img=cv2.threshold(img,127,255,cv2.THRESH_BINARY)<br>
cv2.imshow("Binary",bw_img)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178447330-cfcec33b-8f32-4903-8464-ae75e2a749b5.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178447670-c74210bd-031b-4159-b0f8-2ceee4e26204.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178447726-cce526ad-5d19-48e6-bf08-5a9568be22f4.png)<br>

**PROGRAM 9:RESIZE THE ORIGINAL IMAGE**
import cv2<br>
img=cv2.imread('b4.jpg')<br>
print('original image length width',img.shape)<br>
cv2.imshow('original image',img)<br>
cv2.waitKey(0)<br>
#to show the resized image
imgresize=cv2.resize(img,(150,160))<br>
cv2.imshow('Resized image',imgresize) <br>
print('Resized image length width',imgresize.shape)<br>
cv2.waitKey(0)<br>

**OUTPUT:<br>**
original image length width (705, 564, 3)<br>
Resized image length width (160, 150, 3)<br>
 
![image](https://user-images.githubusercontent.com/97939491/178448146-4e7875ec-57f0-4179-83e0-82951d20d7f2.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178448225-662a0718-9623-487e-8ec3-fb4b1e0b426e.png)<br>

**PROGRAM 10 :WRITE PROGRAM TO READ IMAGE USING URL:**

from skimage import io<br>
import matplotlib.pyplot as plt<br>
url='https://dpbfm6h358sh7.cloudfront.net/images/5391016/1165772661.jpg'<br>
image=io.imread(url)<br>
plt.imshow(image)<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939284/175005167-37733182-adc1-4404-b89c-e98949093711.png)

**PROGRAM 11:WRITE THE PROGRAM TO MASK AND BLUR THE IMAGE:**

import cv2<br>
import matplotlib.image as mpimg<br>
import matplotlib.pyplot as plt<br>
img=cv2.imread('Nemo.jpg')<br>
plt.imshow(img)<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939284/175016581-f6306b36-20bf-4e24-bb37-078e583ec0a5.png)<br>

hsv_img=cv2.cvtColor(img,cv2.COLOR_RGB2HSV)<br>
light_orange=(1,190,200)<br>
dark_orange=(18,255,255)<br>
mask=cv2.inRange(img,light_orange,dark_orange)<br>
result=cv2.bitwise_and(img,img,mask=mask)<br>
plt.subplot(1,2,1)<br>
plt.imshow(mask,cmap="gray")<br>
plt.subplot(1,2,2)<br>
plt.imshow(result)<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939284/175018103-8f9c2618-3c9e-4b98-820a-aefe1a99c8e0.png)<br>

light_white=(0,0,200)<br>
dark_white=(145,60,255)
mask_white=cv2.inRange(hsv_img,light_white,dark_white)<br>
result_white=cv2.bitwise_and(img,img,mask=mask_white)<br>
plt.subplot(1,2,1)
plt.imshow(mask_white,cmap="gray")<br>
plt.subplot(1,2,2)<br>
plt.imshow(result_white)<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939284/175021322-e0c791b4-b034-459b-872a-fdab3c014de8.png)

final_mask=mask+mask_white<br>
final_result=cv2.bitwise_and(img,img,mask=final_mask)<br>
plt.subplot(1,2,1)<br>
plt.imshow(final_mask,cmap="gray")<br>
plt.subplot(1,2,2)<br>
plt.imshow(final_result)<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939284/175022161-6a5274ee-c347-4a21-b126-471b2e687a6e.png)<br>

blur=cv2.GaussianBlur(final_result,(7,7),0)<br>
plt.imshow(blur)<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939284/175022486-66bbc556-701b-4919-a3f5-f046379189e8.png)

**PROGRAM 12: WRITE A PROGRAM TO PERFORM ARITHMETIC OPERATION ON IMAGE:**

import cv2<br>
import matplotlib.image as mpimg<br>
import matplotlib.pyplot as plt<br>

#Reading image files<br>
img1=cv2.imread('flo1.jpg')<br>
img2=cv2.imread('flo2.jpg')<br>

#Applying Numpy addition on images<br>
fimg1=img1+img2<br>
plt.imshow(fimg1)<br>
plt.show()<br>

#Saving the ouput image<br>
cv2.imwrite('output.jpg',fimg1)<br>
fimg2=img1-img2<br>
plt.imshow(fimg2)<br>
plt.show()<br>

#saving the ouput image<br>
cv2.imwrite('output.jpg',fimg2)<br>
fimg3=img1*img2<br>
plt.imshow(fimg3)<br>
plt.show()<br>

#Saving the output image<br>
cv2.imwrite('output.jpg',fimg3)<br>
fimg4=img1/img2<br>
plt.imshow(fimg4)<br>
plt.show()<br>

#saving the output image<br>
cv2.imwrite('output.jpg',fimg4)<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178452658-68fa523a-9923-4f9a-a5bb-2bab4109c077.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178452761-d96f382e-413a-4d93-bf65-16e1776fcfa8.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178452865-47950bce-48c5-4250-9d31-84ce5c67111c.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178452916-c567004a-4d69-46fd-8fe2-b1bebbe1647f.png)<br>

**PROGRAM 13: DEVELOP A PROGRAM TO CAHNGE A IMAGE TO DIFFERENT COLOR SPACES:**

import cv2<br> 
img=cv2.imread('D:\\R.jpg')<br> 
gray=cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)<br> 
hsv=cv2.cvtColor(img,cv2.COLOR_BGR2HSV)<br> 
lab=cv2.cvtColor(img,cv2.COLOR_BGR2LAB)<br> 
hls=cv2.cvtColor(img,cv2.COLOR_BGR2HLS)<br> 
yuv=cv2.cvtColor(img,cv2.COLOR_BGR2YUV)<br> 
cv2.imshow("GRAY image",gray)<br> 
cv2.imshow("HSV image",hsv)<br> 
cv2.imshow("LAB image",lab)<br> 
cv2.imshow("HLS image",hls)<br> 
cv2.imshow("YUV image",yuv)<br> 
cv2.waitKey(0)<br> 
cv2.destroyAllWindows()<br> 

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178454236-802fe2c9-e15f-4897-b7b8-315bcb891228.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178454307-e05af90c-8cdf-4091-bde6-78d38095305c.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178454399-85208802-0aef-4d72-9261-d79abce69a31.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178454439-47e8eefd-38fd-410b-bd56-8e16896c6fe4.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178454484-95c1d79b-1467-4daa-ad34-d3e28b32dfbb.png)<br>

**PROGRAM 14 :PROGRAM TO CREATE IMAGE USING 2D ARRAY:**

import cv2 as c<br>
import numpy as np<br>
from PIL import Image
array=np.zeros([100,200,3],dtype=np.uint8)<br>
array[:,:100]=[255, 192, 203]<br>
array[:,100:]=[0,0,255]<br>
img=Image.fromarray(array)<br>
img.save('image1.png')<br>
img.show()<br>
c.waitKey(0)<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939284/175276384-61662c7b-8a30-4104-b4ad-327a1a03b6e0.png)

**PROGRAM 15:PROGRAM TO PERFORM BITWISE OPERATION:**

import cv2<br>
import matplotlib.pyplot as plt<br>
image1=cv2.imread('3.jpg',1)<br>
image2=cv2.imread('3.jpg')<br>
ax=plt.subplots(figsize=(15,10))<br>
bitwiseAnd=cv2.bitwise_and(image1,image2)<br>
bitwiseOr=cv2.bitwise_or(image1,image2)<br>
bitwiseXor=cv2.bitwise_xor(image1,image2)<br>
bitwiseNot_img1=cv2.bitwise_not(image1)<br>
bitwiseNot_img2=cv2.bitwise_not(image2)<br>
plt.subplot(151)<br>
plt.imshow(bitwiseAnd)<br>
plt.subplot(152)<br>
plt.imshow(bitwiseOr)<br>
plt.subplot(153)<br>
plt.imshow(bitwiseXor)<br>
plt.subplot(154)
plt.imshow(bitwiseNot_img1)<br>
plt.subplot(155)<br>
plt.imshow(bitwiseNot_img2)<br>
cv2.waitKey(0)<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178456927-8e7d0805-7eb9-4584-a40a-ed8213ede7d6.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178457049-d94bbf24-311d-4986-846e-a92cd5a25a63.png)

**PROGRAM 16:PROGRAM TO PERFORM BLURRING THE IMAGE:**

importing libraries<br>
import cv2<br>
import numpy as np<br>
image=cv2.imread('g.jpg')<br>
cv2.imshow('Original Image',image)<br>
cv2.waitKey(0)<br>
#Gaussian Blur<br>
Gaussian=cv2.GaussianBlur(image,(7,7),0)<br>
cv2.imshow("Gaussian blurring",Gaussian)<br>
cv2.waitKey(0)<br>
#Median Blur<br>
median=cv2.medianBlur(image,5)<br>
cv2.imshow('Median Blurring',median)<br>
cv2.waitKey(0)<br>
#Bilateral Blur<br>
bilateral=cv2.bilateralFilter(image,9,75,75)<br>
cv2.imshow('Bilateral Blurring',bilateral)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178458244-6804c63f-16fb-444c-8769-d2466978917d.png)
![image](https://user-images.githubusercontent.com/97939491/178458331-faa3d068-d411-4b4d-a8c6-ccf1233eed86.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178458409-06e8c8a5-dd73-43b0-84a0-6267b05d3389.png)
![image](https://user-images.githubusercontent.com/97939491/178458506-17c581f0-5e12-4a95-b04d-d69dc0985c70.png)

**PROGRAM 17:PROGRAM TO PERFORM IMAGE ENHANCEMENT:**

from PIL import Image<br>
from PIL import ImageEnhance<br>
image=Image.open('19.jpg')<br>
image.show()<br>
enh_bri=ImageEnhance.Brightness(image)<br>
brightness=1.5<br>
image_brightened=enh_bri.enhance(brightness)<br>
image_brightened.show()<br>
enh_col=ImageEnhance.Color(image)<br>
color=1.5<br>
image_colored=enh_col.enhance(color)<br>
image_colored.show()<br>
enh_con=ImageEnhance.Contrast(image)<br>
contrast=1.5<br>
image_contrasted=enh_con.enhance(contrast)<br>
image_contrasted.show()<br>
enh_sha=ImageEnhance.Sharpness(imag<br>)<br>
sharpness=3.0<br>
image_sharped=enh_sha.enhance(sharpness)<br>
image_sharped.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178459237-7c2f1ef6-4b0e-40f8-b4fe-ad540ccf1aa5.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178459281-c970b2e8-bc70-4589-a0de-5a56d8615424.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178459335-ff1c09c9-202c-4fd9-b637-16a01646016c.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178459374-4b664932-83dd-41f0-b60c-723bd7340152.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178459421-d2b87e85-2752-4978-a501-8d0247e0e8f2.png)<br>

**PROGRAM 18:PROGRAM TO PERFORM MORPHOLOGICAL OPERATIONS:**

import cv2<br>
import numpy as np<br>
from matplotlib import pyplot as plt<br>
from PIL import Image,ImageEnhance<br>
img=cv2.imread('b2.jpg',0)<br>
ax=plt.subplots(figsize=(20,10))<br>
kernel=np.ones((5,5),np.uint8)<br>
opening=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernel)<br>
closing=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernel)<br>
erosion=cv2.erode(img,kernel,iterations=1)<br>
dilation=cv2.dilate(img,kernel,iterations=1)<br>
gradient=cv2.morphologyEx(img,cv2.MORPH_GRADIENT,kernel)<br>
plt.subplot(151)<br>
plt.imshow(opening)<br>
plt.subplot(152)<br>
plt.imshow(closing)<br>
plt.subplot(153)<br>
plt.imshow(erosion)<br>
plt.subplot(154)<br>
plt.imshow(dilation)<br>
plt.subplot(155)<br>
plt.imshow(gradient)<br>
cv2.waitKey(0)<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178459539-58a25f84-58b7-4b48-b38e-c5862fdc7bf1.png)

**PROGRAM 19:DEVELOP A PROGRAM TO
(i)READ THE IMAGE
(ii)WRITE (SAVE) THE GRAY SCALE IMAGE
(iii)DISPLAY ORIGINAL IMAGE AND GRAY SCALE IMAGE:**

import cv2<br>
OriginalImg=cv2.imread('b1.jpg')<br>
GrayImg=cv2.imread('b1.jpg',0)<br>
isSaved=cv2.imwrite('D:/i.jpg',GrayImg)<br>
cv2.imshow('Display Original Image',OriginalImg)<br>
cv2.imshow('Display Grayscale Image',GrayImg)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
if isSaved:<br>
     print('The image is successfully saved.')<br>
     
**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178711706-314add0a-9386-4a9e-9eac-61d3344ef1fb.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178711832-af98e611-cd33-45ce-88e6-6f32f8514468.png)<br>

**PROGRAM 20: SLICING WITH BACKGROUND:**

import cv2<br>
import numpy as np<br>
from matplotlib import pyplot as plt<br>
image=cv2.imread('b1.jpg',0)<br>
x,y=image.shape<br>
z=np.zeros((x,y))<br>
for i in range (0,x):<br>
    for j in range(0,y):<br>
        if(image[i][j]>50 and image[i][j]<150):<br>
            z[i][j]=255<br>
        else:<br>
            z[i][j]=image[i][j]<br>
equ=np.hstack((image,z))<br>
plt.title('Gray level slicing with background')<br>
plt.imshow(equ,'gray')<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178712823-ad57859f-b838-4d6b-ad4c-73a12e28cefa.png)<br>

**PROGRAM 21:SLICING WITHOUT BACKGROUNG:**

import cv2<br>
import numpy as np<br>
from matplotlib import pyplot as plt<br>
image=cv2.imread('b1.jpg',0)<br>
x,y=image.shape<br>
z=np.zeros((x,y))<br>
for i in range (0,x):<br>
    for j in range(0,y):<br>
        if(image[i][j]>50 and image[i][j]<150):<br>
            z[i][j]=255<br>
        else:<br>
            z[i][j]=image[i][j]<br>
equ=np.hstack((image,z))<br>
plt.title('Gray level slicing w/o background')<br>
plt.imshow(equ,'gray')<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178715584-3fdeb980-37b6-4565-a2ae-ddc3e38d6663.png)<br>

**PROGRAM 22: ANALYSE THE IMAGE DATA USING HISTOGRAM:**
import cv2<br>
from matplotlib import pyplot as plt<br>
img = cv2.imread('b1.jpg',0)<br>
plt.hist(img.ravel(),256,[0,256])<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178961125-21995c0e-95be-40c8-b4af-057e7aa97186.png)<br>

import cv2<br>
from matplotlib import pyplot as plt<br>
img = cv2.imread('b1.jpg',0)<br>
histr = cv2.calcHist([img],[0],None,[256],[0,256])<br>
plt.plot(histr)<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178963075-d94a1112-31ef-4f40-a302-93d58837fca3.png)<br>

from skimage import io<br>
import matplotlib.pyplot as plt<br>
image = io.imread('b1.jpg')<br>
plt.hist(image.ravel(), bins = 256, color = 'orange', )<br>
plt.hist(image[:, :, 0].ravel(), bins = 256, color = 'red', alpha = 0.5)<br>
plt.hist(image[:, :, 1].ravel(), bins = 256, color = 'Green', alpha = 0.5)<br>
plt.hist(image[:, :, 2].ravel(), bins = 256, color = 'Blue', alpha = 0.5)<br>
plt.xlabel('Intensity Value')<br>
plt.ylabel('Count')<br>
plt.legend(['Total', 'Red_Channel', 'Green_Channel', 'Blue_Channel'])<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178963461-b91aa4f1-7dbb-4b9a-8527-4678cfbb8fc7.png)<br>

import cv2<br>
import numpy as np<br>
img=cv2.imread('b1.jpg')<br>
hist=cv2.calcHist([img],[0],None,[256],[0,256])<br>
plt.hist(img.ravel(),256,[0,256])<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178963807-fe01a9c2-276c-4e98-b77d-bcce1a99dea9.png)<br>
