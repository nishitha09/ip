

**PROGRAM 1: DEVELOP A PROGRAM TO DISPLAY GRAY SCALE IMAGE USING READ AND WRITE OPERATION:**
   
 import cv2<br>
 img=cv2.imread('b1.jpg',0)<br>
 cv2.imshow('b1',img)<br>
 cv2.waitKey(0)<br>
 cv2.destroyAllWindows()<br>
  
**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178444060-1c6d34fd-3ebe-4127-87cc-94a2fb7e1861.png)<br>

**PROGRAM 2: DEVELOP A PROGRAM TO DISPLAY IMAGE USING MATPLOTLIB**
 
 import matplotlib.image as mping<br>
 import matplotlib.pyplot as plt<br>
 img=mping.imread('f2.jpg')<br>
 plt.imshow(img)<br>
 
 **OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178444384-50f41d8f-61f0-43bb-bd01-2a68218079d8.png)<br>
 
**PROGRAM 3: DEVELOP A PROGRAM TO PERFORM LINEAR TRANSFORMATION:**

from PIL import Image<br>
img=Image.open('l1.jpg')<br>
img=img.rotate(180)<br>
img.show()<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/178444653-1645cde6-84ab-425c-b2e0-2285b07781bf.png)<br>

**PROGRAM 4: DEVELOP PROGRAM TO CONVERT COLOR STRING TO RGB COLOR VALUES:**

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

**PROGRAM 5: DEVELOP PROGRAM TO CREATE IMAGE USING COLORS:**

from PIL import Image<br>
img=Image.new("RGB",(200,400),(0, 0, 255))<br>
img.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939284/173813696-f552419d-9b39-4595-bf01-92f689afc915.png)<br>

**PROGRAM 6: DEVELOP A PROGRAM TO VISUALIZE THE IMAGE USING VARIOUS COLOR SPACE:**

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

**PROGRAM 7: WRITE A PROGRAM TO DISPLAY IMAGE ATTRIBUTE:**

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

**PROGRAM 8: CONVERT ORIGINAL IMAGE TO GRAY SCALE AND THEN TO BINARY:** 

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

**PROGRAM 9: RESIZE THE ORIGINAL IMAGE:**

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

**PROGRAM 10: WRITE PROGRAM TO READ IMAGE USING URL:**

from skimage import io<br>
import matplotlib.pyplot as plt<br>
url='https://dpbfm6h358sh7.cloudfront.net/images/5391016/1165772661.jpg'<br>
image=io.imread(url)<br>
plt.imshow(image)<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939284/175005167-37733182-adc1-4404-b89c-e98949093711.png)<br>

**PROGRAM 11: WRITE THE PROGRAM TO MASK AND BLUR THE IMAGE:**

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
![image](https://user-images.githubusercontent.com/97939284/175021322-e0c791b4-b034-459b-872a-fdab3c014de8.png)<br>

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
![image](https://user-images.githubusercontent.com/97939284/175022486-66bbc556-701b-4919-a3f5-f046379189e8.png)<br>

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
![image](https://user-images.githubusercontent.com/97939491/179968143-79b68637-ac3a-408b-ab94-35b9c5ed13dd.png)<br>
![image](https://user-images.githubusercontent.com/97939491/179968234-e5cc2b1c-9bae-4562-a373-903e57711979.png)<br>

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

**PROGRAM 14: PROGRAM TO CREATE IMAGE USING 2D ARRAY:**

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
![image](https://user-images.githubusercontent.com/97939284/175276384-61662c7b-8a30-4104-b4ad-327a1a03b6e0.png)<br>

**PROGRAM 15: PROGRAM TO PERFORM BITWISE OPERATION:**

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
![image](https://user-images.githubusercontent.com/97939491/178457049-d94bbf24-311d-4986-846e-a92cd5a25a63.png)<br>

**PROGRAM 16: PROGRAM TO PERFORM BLURRING THE IMAGE:**

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
![image](https://user-images.githubusercontent.com/97939491/178458244-6804c63f-16fb-444c-8769-d2466978917d.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178458331-faa3d068-d411-4b4d-a8c6-ccf1233eed86.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178458409-06e8c8a5-dd73-43b0-84a0-6267b05d3389.png)<br>
![image](https://user-images.githubusercontent.com/97939491/178458506-17c581f0-5e12-4a95-b04d-d69dc0985c70.png)<br>

**PROGRAM 17: PROGRAM TO PERFORM IMAGE ENHANCEMENT:**

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

**PROGRAM 18: PROGRAM TO PERFORM MORPHOLOGICAL OPERATIONS:**

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
![image](https://user-images.githubusercontent.com/97939491/178459539-58a25f84-58b7-4b48-b38e-c5862fdc7bf1.png)<br>

**PROGRAM 19: DEVELOP A PROGRAM TO
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

**PROGRAM 21: SLICING WITHOUT BACKGROUNG:**

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

**PROGRAM 23: PROGRAM TO PERFORM BASIC IMAGE DATA ANALYSIS USING INTENSITY TRANSFORMATION:**

%matplotlib inline<br>
import imageio<br>
import matplotlib.pyplot as plt<br>
import warnings<br>
import matplotlib.cbook<br>
warnings.filterwarnings("ignore",category=matplotlib.cbook.mplDeprecation)<br>
pic=imageio.imread('b1.jpg')<br>
plt.figure(figsize=(6,6))<br>
plt.imshow(pic);<br>
plt.axis('off');<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/179960709-0e464594-e1d0-4ea0-b5bd-a1734c426261.png)<br>

negative=255-pic #neg=(L-1)-img<br>
plt.figure(figsize=(6,6))<br>
plt.imshow(negative);<br>
plt.axis('off');<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/179963212-3080864b-4274-4442-aaf6-bd182220c6fd.png)<br>

%matplotlib inline<br>
import imageio<br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>
pic=imageio.imread('b1.jpg')<br>
gray=lambda rgb:np.dot(rgb[...,:3],[0.299,0.587,0.114])<br>
gray=gray(pic)<br>
max_=np.max(gray)<br>
def log_transform():<br>
    return(255/np.log(1+max_))*np.log(1+gray)<br>
plt.figure(figsize=(5,5))<br>
plt.imshow(log_transform(),cmap=plt.get_cmap(name='gray'))<br>
plt.axis('off')<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/179963476-d63afc71-e5c0-4b17-8a06-885e79633ce6.png)<br>

import imageio<br>
import matplotlib.pyplot as plt<br>
#Gamma encoding<br>
pic=imageio.imread('b1.jpg')<br>
gamma=2.2#Gamma<1~Dark; Gamma>1~Bright<br>
gamma_correction=((pic/255)**(1/gamma))<br>
plt.figure(figsize=(5,5))<br>
plt.imshow(gamma_correction)<br>
plt.axis('off');<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/179963686-f1721d0c-fc53-40eb-bb5f-6a22f2517a2d.png)<br>

**PROGRAM 24: PROGRAM TO PERFORM BASIC IMAGE MANIPULATION:
              (a)SHARPNESS
              (b)FLIPPING
              (C)CROPPING**<br>
              
#Image sharpen<br>
from PIL import Image<br>
from PIL import ImageFilter<br>
import matplotlib.pyplot as plt<br>
#Load the image<br>
my_image=Image.open('l1.jpg')<br>
#use sharpen function<br>
sharp=my_image.filter(ImageFilter.SHARPEN)<br>
#save the image<br>
sharp.save('D:/image_sharpen.jpg')<br>
sharp.show()<br>
plt.imshow(sharp)<br>
plt.show()<br>            
   
**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/179964623-08dbf17a-46d0-40c4-b940-b5545926f2b6.png)<br>

#Image flip<br>
import matplotlib.pyplot as plt<br>
#Load the image<br>
img=Image.open('l1.jpg')<br>
plt.imshow(img)<br>
plt.show()<br>
#use the flip function<br>
flip=img.transpose(Image.FLIP_LEFT_RIGHT)<br>
#save the image<br>
flip.save('D:/image_flip.jpg')<br>
plt.imshow(flip)<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/179964858-7a1b01e3-07f4-466e-904c-6522f2fce920.png)<br><br>

#Importing Image class from PIL module<br>
from PIL import Image<br>
import matplotlib.pyplot as plt<br>
#opens a image in RGB mode<br>
im=Image.open('l1.jpg')<br>
#size of image in pixels<br>
width,height=im.size<br>
#cropped image of above dimension<br>
#(It will not change original image)<br>
#(It is not mandatory)<br>
im1=im.crop((50,50,200,200))<br>
#shows the image in image viewer<br>
im1.show()<br>
plt.imshow(im1)<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/179965098-719145fd-88ac-477b-b651-3e5a35fe959d.png)<br>

**PROGRAM 25: 

from PIL import Image<br>
from numpy import asarray<br>
img = Image.open('b1.jpg')<br>
numpydata = asarray(img)<br>
print(numpydata)<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/180194281-681889cd-e40e-4201-93a6-df1674e7eb2c.png)<br>
![image](https://user-images.githubusercontent.com/97939491/180194439-9a0407d8-ab82-41b4-b815-c676f80b054d.png)<br>

from PIL import Image<br>
import matplotlib.pyplot as plt<br>
input_image = Image.new(mode="RGB", size=(1000, 1000),color="pink")<br>
pixel_map = input_image.load()<br>
width, height = input_image.size<br>
z = 100<br>
for i in range(width):<br>
    for j in range(height):<br>
        if((i >= z and i <= width-z) and (j >= z and j <= height-z)):<br>
            pixel_map[i, j] = (230,230,250)<br>
        else:<br>
            pixel_map[i, j] = (216,191,216)<br>
for i in range(width):<br>
    pixel_map[i, i] = (0, 0, 255)<br>
    pixel_map[i, width-i-1] = (0, 0, 255)<br>
plt.imshow(input_image)<br>
plt.show()<br>  

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/180194708-8ef101d0-f077-4b46-a79f-a58c56d1a3b1.png)<br>

import numpy as np<br>
import matplotlib.pyplot as plt<br>
arr = np.zeros((256,256,3), dtype=np.uint8)<br>
imgsize = arr.shape[:2]<br>
innerColor = (255, 255, 255)<br>
outerColor = (0, 0, 0)<br>
for y in range(imgsize[1]):<br>
    for x in range(imgsize[0]):<br>
        distanceToCenter = np.sqrt((x - imgsize[0]//2) ** 2 + (y - imgsize[1]//2) ** 2)<br>
        distanceToCenter = distanceToCenter / (np.sqrt(2) * imgsize[0]/2)<br>
        r = outerColor[0] * distanceToCenter + innerColor[0] * (1 - distanceToCenter)<br>
        g = outerColor[1] * distanceToCenter + innerColor[1] * (1 - distanceToCenter)<br>
        b = outerColor[2] * distanceToCenter + innerColor[2] * (1 - distanceToCenter)<br>
        arr[y, x] = (int(r), int(g), int(b))<br>
plt.imshow(arr, cmap='gray')<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/180194894-a76dcfe0-302c-431d-8dbc-fc10700a06a5.png)<br>

import numpy as np<br>
import matplotlib.pyplot as plt<br>   
imgsize=(650,650)<br>
image = Image.new('RGB', imgsize)<br>
innerColor = [153,0,0]<br>
for y in range(imgsize[1]):<br>
    for x in range(imgsize[0]):<br>
         distanceToCenter =np.sqrt((x - imgsize[0]/2) ** 2 + (y - imgsize[1]/2) ** 2)<br>
         distanceToCenter = (distanceToCenter) / (np.sqrt(2) * imgsize[0]/2)<br>
         r = distanceToCenter + innerColor[0] * (1 - distanceToCenter)<br>
         g =  distanceToCenter + innerColor[1] * (1 - distanceToCenter)<br>
         b =  distanceToCenter + innerColor[2] * (1 - distanceToCenter)<br>
         image.putpixel((x, y), (int(r), int(g), int(b)))<br>
plt.imshow(image)<br>
plt.show()<br>  

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/180195119-41c5980a-4f9a-4562-a12b-813f88f89dbe.png)<br>

from PIL import Image<br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>
w, h = 512, 512<br>
data = np.zeros((h, w, 3), dtype=np.uint8)<br>
data[0:100, 0:100] = [255, 0, 0]<br>
data[100:200, 100:200] = [255, 0, 255]<br>
data[200:300, 200:300] = [0, 255, 0]<br>
data[300:400, 300:400] = [255, 255, 0]<br>
data[400:500, 400:500] = [0, 255, 255]<br>
img = Image.fromarray(data, 'RGB')<br>
img.save('my.png')<br>
plt.imshow(img)<br>
plt.show()<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/180202825-69ff90b6-56f3-420d-9a6f-ed642f9fd8e1.png)<br>

from PIL import Image<br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>
w, h = 512, 512<br>
data = np.zeros((h, w, 3), dtype=np.uint8)<br>
data[0:120, 0:512] = [255, 255, 255]<br>
data[120:256, 0:512] = [218, 218, 218]<br>
data[256:320, 0:512] = [0, 0,0]<br>
data[320:420, 0:512] = [218, 218,218]<br>
data[420:512, 0:512] = [255, 255,255]<br>
#red patch in upper left<br>
img = Image.fromarray(data, 'RGB')<br>
img.save('img8.jpg')<br>
img.show()<br>
plt.imshow(img)<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/181432254-70101d64-ee44-4c5d-9879-01290879defe.png)<br>

#Python3 program for printing<br>
#the rectangular pattern<br>
 #Function to print the pattern<br>
def printPattern(n):<br>
    arraySize = n * 2 - 1;<br>
    result = [[0 for x in range(arraySize)]<br>
                 for y in range(arraySize)];<br>
    #Fill the values<br>
    for i in range(arraySize):<br>
        for j in range(arraySize):<br>
            if(abs(i - (arraySize // 2)) ><br>
               abs(j - (arraySize // 2))):<br>
                result[i][j] = abs(i - (arraySize // 2)) ;<br>
            else:<br>
                result[i][j] = abs(j - (arraySize // 2)) ;<br>
    #Print the array<br>
    for i in range(arraySize):<br>
        for j in range(arraySize):<br>
            print(result[i][j], end = " ");<br>
        print("");<br>
#Driver Code<br>
n = 3;<br>
printPattern(n);<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/181432644-fdfd3bb2-78c1-407f-80a6-ddf93ef9b589.png)

**PROGRAM 26:PROGRAM TO FIND THE AVERAGE, MAXIMUM,MINIMUM AND STANDARD DEVIATION PIXEL VALUE FROM THE IMAGE:**

import cv2<br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>
img=cv2.imread("f1.JPG",0)<br>
img=cv2.cvtColor(img,cv2.COLOR_BGR2RGB)<br>
plt.imshow(img)<br>
np.average(img)<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/181433384-98896e6f-940f-4071-8628-6168e853daa4.png)<br>

import cv2<br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>
img=cv2.imread('f1.jpg' )<br>
plt.imshow(img)<br>
plt.show()<br>
max_channels = np.amax([np.amax(img[:,:,0]), np.amax(img[:,:,1]),np.amax(img[:,:,2])])<br>
print(max_channels)<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/181433650-450c9826-c6c4-4633-a424-50de94ea260c.png)<br>

import cv2<br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>
img=cv2.imread('f1.jpg' )<br>
plt.imshow(img)<br>
plt.show()<br>
min_channels = np.amin([np.min(img[:,:,0]), np.amin(img[:,:,1]),np.amin(img[:,:,2])])<br>
print(min_channels)<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/181433895-44198a1b-6c52-4d42-aafa-4f368a8f5863.png)<br>

from PIL import Image,ImageStat<br>
import matplotlib.pyplot as plt<br>
im=Image.open('f1.jpg')<br>
plt.imshow(im)<br>
plt.show()<br>
stat=ImageStat.Stat(im)<br>
print(stat.stddev)<br>

**OUTPUT:<br>**
![image](https://user-images.githubusercontent.com/97939491/181434168-6c786e1f-52a5-4ee9-91c1-5f33b11dc673.png)<br>

**PROGRAM 27: PROGRAM TO PERFORM EDGE DETECTION:** 

import cv2<br>
#Read the original image<br>
img = cv2.imread('l2.jpg')<br>
#Display original image<br>
cv2.imshow('Original', img)<br>
cv2.waitKey(0)<br>
#Convert to graycsale<br>
img_gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)<br>
#Blur the image for better edge detection<br>
img_blur = cv2.GaussianBlur(img_gray, (3,3), 0)<br>
#Sobel Edge Detection<br>
sobelx = cv2.Sobel(src=img_blur, ddepth=cv2.CV_64F, dx=1, dy=0, ksize=5) # Sobel Edge Detection on the X axis<br>
sobely = cv2.Sobel(src=img_blur, ddepth=cv2.CV_64F, dx=0, dy=1, ksize=5) # Sobel Edge Detection on the Y axis<br>
sobelxy = cv2.Sobel(src=img_blur, ddepth=cv2.CV_64F, dx=1, dy=1, ksize=5) # Combined X and Y Sobel Edge Detection<br>
#Display Sobel Edge Detection Images<br>
cv2.imshow('Sobel X', sobelx)<br>
cv2.waitKey(0)<br>
cv2.imshow('Sobel Y', sobely)<br>
cv2.waitKey(0)<br>
cv2.imshow('Sobel X Y using Sobel() function', sobelxy)<br>
cv2.waitKey(0)<br>
#Canny Edge Detection<br>
edges = cv2.Canny(image=img_blur, threshold1=100, threshold2=200) # Canny Edge Detection<br>
#Display Canny Edge Detection Image<br>
cv2.imshow('Canny Edge Detection', edges)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>

**OUTPUT:**<br>
![image](https://user-images.githubusercontent.com/97939491/186401184-19797d7f-6095-4631-8694-610ab7189fc5.png)<br>
![image](https://user-images.githubusercontent.com/97939491/186401348-b1b202f1-c1ae-477b-b1cb-f864f784b121.png)<br>
![image](https://user-images.githubusercontent.com/97939491/186401490-2678a49a-8e6a-48ed-8453-98a5dd1f44c0.png)<br>
![image](https://user-images.githubusercontent.com/97939491/186401610-b11652e0-230d-4692-b7b7-4e1a06ab55c8.png)<br>
![image](https://user-images.githubusercontent.com/97939491/186401716-b96698f3-99ce-433f-9e95-2a90370c2eb8.png)<br>


**PROGRAM 28: IMAGE FILTERING**

import matplotlib.pyplot as plt<br>
%matplotlib inline<br>
from skimage import data,filters<br>
image = data.coins()<br>
#... or any other NumPy array!<br>
edges = filters.sobel(image)<br>
plt.imshow(edges, cmap='gray')<br>

**OUTPUT:**<br>
![image](https://user-images.githubusercontent.com/97939491/186404519-7c86f0cb-fa98-47fb-b05c-95fefb234bc9.png)<br>

**PROGRAM 29: MASK AN IMAGE**

import numpy as np<br>
from skimage import data<br>
import matplotlib.pyplot as plt<br>
%matplotlib inline<br>
image = data.camera()<br>
type(image)<br>
np.ndarray #Image is a numpy array<br>
mask = image < 87<br>
image[mask]=255<br>
plt.imshow(image, cmap='gray')<br>

**OUTPUT:**<br>
![image](https://user-images.githubusercontent.com/97939491/186405913-9d2bac6b-3280-4113-9bca-53a17cbecf1e.png)<br>

**PROGRAM 30: BASIC PILLOW FUNCTION**

from PIL import Image,ImageChops,ImageFilter<br>
from matplotlib import pyplot as plt<br>
#create a PIL Image objects<br>
x = Image.open("x.png")<br>
o = Image.open("o.png")<br>
#Find out attributes of Image objects<br>
print('size of the image:',x.size,'colour mode:',x.mode)<br>
print('size of the image:',o.size,'colour mode:',o.mode)<br>
#plot 2 images one besides the other<br>
plt.subplot(121),plt.imshow(x)<br>
plt.axis('off')<br>
plt.subplot(122),plt.imshow(o)<br>
plt.axis('off')<br>
#multiply images<br>
merged=ImageChops.multiply(x,o)<br>
#adding 2 images<br>
add=ImageChops.add(x,o)<br>
#convert colour mode<br>
greyscale = merged.convert('L')<br>
greyscale<br>

**OUTPUT:**<br>
![image](https://user-images.githubusercontent.com/97939491/187875215-184c4abd-2cd7-4c6d-869f-0aeea0659781.png)<br>

#More Attributes<br>
image=merged<br>
print('image size:',image.size,<br>
      '\ncolor mode:',image.mode,<br>
      '\nimage width:',image.width,'|also represented by:',image.size[0],<br>
      '\nimage height:',image.height,'|also represented by:',image.size[1],)<br>

**OUTPUT:**<br>
![image](https://user-images.githubusercontent.com/97939491/187875807-5abd9d6c-ba20-4d7e-bc02-3a8fd6691f27.png)<br>

#mapping the pixels of the image so we can use them as coordinates<br>
pixel = greyscale.load()<br>
#a nested loop to parse through all the pixels in the image<br>
for row in range(greyscale.size[0]):<br>
    for column in range(greyscale.size[1]):<br>
        if pixel[row,column]!=(255):<br>
            pixel[row,column]=(0)<br>
greyscale<br>

**OUTPUT:**<br>
![image](https://user-images.githubusercontent.com/97939491/187876075-7fec098d-9d5c-4373-ae72-a2d2942a5fa6.png)<br>

#1.invert image<br>
invert = ImageChops.invert(greyscale)<br>
#2.invert by subtraction<br>
bg = Image.new('L',(256,256),color=(255))#create a new image with a solid white background<br>
subt = ImageChops.subtract(bg, greyscale)#subtract image from background<br>
#3.rotate<br>
rotate = subt.rotate(45)<br>
rotate<br>

**OUTPUT:**<br>
![image](https://user-images.githubusercontent.com/97939491/187876447-2ea6e375-a78f-4552-90d0-a7ac400b89e8.png)

#gaussian blur<br>
blur=greyscale.filter(ImageFilter.GaussianBlur(radius=1))<br>
#edge dtection<br>
edge = blur.filter(ImageFilter.FIND_EDGES)<br>
edge<br>

**OUTPUT:**<br>
![image](https://user-images.githubusercontent.com/97939491/187876785-b8177c2c-5a72-43c4-8e18-6964d8f09a0b.png)<br>

#change edge colours<br>
edge = edge.convert('RGB')<br>
bg_red = Image.new('RGB',(256,256),color=(255,0,0))<br>
filled_edge = ImageChops.darker(bg_red,edge)<br>
filled_edge<br>

**OUTPUT:**<br>
![image](https://user-images.githubusercontent.com/97939491/187877091-7b53c425-0cc6-4f8a-a10a-230d48ff49a0.png)<br>

#save image in the directory<br>
edge.save('processed.png')<br>

**PROGRAM 31: IMAGE RESTORATION**

import numpy as np<br>
import cv2<br>
import matplotlib.pyplot as plt<br>
#open the image<br>
img = cv2.imread('dimage_damaged.png')<br>
plt.imshow(img)<br>
plt.show()<br>
#Load the mask<br>
mask = cv2.imread('dimage_mask.png',0)<br>
plt.imshow(mask)<br>
plt.show()<br>
#Inpaint<br>
dst = cv2.inpaint(img, mask, 3,cv2.INPAINT_TELEA)<br>
#Write the output<br>
cv2.imwrite('dimage_inpainted.png',dst)<br>
plt.imshow(dst)<br>
plt.show()<br>

**OUTPUT:**<br>
![image](https://user-images.githubusercontent.com/97939491/187878133-47f343c5-6b5d-48dc-af5b-4234f8e37e01.png)<br>
![image](https://user-images.githubusercontent.com/97939491/187878191-e44aa331-f4bf-4838-8b1d-89c237794f8a.png)<br>
![image](https://user-images.githubusercontent.com/97939491/187878269-ae8b697a-19cf-48a4-81e4-0730b263fc5c.png)<br>

import numpy as np<br>
import matplotlib.pyplot as plt<br>
import pandas as pd<br>
plt.rcParams['figure.figsize']=(10,8)<br>

def show_image(image,title='Image',cmap_type='gray'):<br>
    plt.imshow(image,cmap=cmap_type)<br>
    plt.title(title)<br>
    plt.axis('off')<br>

def plot_comparison(img_original,img_filtered,img_title_filtered):<br>
    fig,(ax1,ax2)=plt.subplots(ncols=2,figsize=(10,8),sharex=True,sharey=True)<br>
    ax1.imshow(img_original,cmap=plt.cm.gray)<br>
    ax1.set_title('original')<br>
    ax1.axis('off')<br>
    ax2.imshow(img_filtered,cmap=plt.cm.gray)<br>
    ax2.set_title(img_title_filtered)<br>
    ax2.axis('off')<br>
    
from skimage.restoration import inpaint<br>
from skimage.transform import resize<br>
from skimage import color<br>

image_with_logo = plt.imread('imlogo.png')<br>
#Initalize the mask<br>
mask = np.zeros(image_with_logo.shape[:-1])<br>
#Set the pixels where the logo is to 1<br>
mask[210:272,360:425] = 1<br>
#Apply inpainting to remove the logo<br>
image_logo_removed = inpaint.inpaint_biharmonic(image_with_logo,<br>
                                              mask,<br>
                                              multichannel=True)<br>
#Show the original and logo removed images<br>
plot_comparison(image_with_logo,image_logo_removed,'Image with logo removed')<br>

**OUTPUT:**
![image](https://user-images.githubusercontent.com/97939491/187879218-a1bb9804-e323-4dea-969b-e60b86b99e5d.png)<br>

from skimage.util import random_noise<br>
fruit_image = plt.imread('fruitts.jpeg')<br>
#Add noise to the image<br>
noisy_image = random_noise(fruit_image)<br>
#Show the original and resulting image<br>
plot_comparison(fruit_image, noisy_image, 'Noisy image')<br>

**OUTPUT:**<br>
![image](https://user-images.githubusercontent.com/97939491/187879454-7e5aa509-30cb-4ff0-898c-e2b5099800ab.png)<br>

import matplotlib.pyplot as plt<br>
from skimage.restoration import denoise_tv_chambolle<br>
noisy_image = plt.imread('noisy.jpg')<br>
#Apply total variation filter denoising<br>
denoised_image=denoise_tv_chambolle(noisy_image,multichannel=True)<br>
#Show the noisy and denoised image<br>
plot_comparison(noisy_image,denoised_image,'Denoised Image')<br>

**OUTPUT:**<br>
![image](https://user-images.githubusercontent.com/97939491/187879723-8eac3ad1-d139-4e13-9c77-93199f53014c.png)<br>

from skimage.restoration import denoise_bilateral<br>
landscape_image = plt.imread('noisy.jpg')<br>
#Apply bilateral filter denoising<br>
denoised_image = denoise_bilateral(landscape_image,multichannel=True)<br>
#Show original and rsulting images<br>
plot_comparison(landscape_image,denoised_image,'Denoised Image')<br>

**OUTPUT:**<br>
![image](https://user-images.githubusercontent.com/97939491/187880046-8e1eb660-a5c9-4fae-a3c0-6d3224bbc548.png)<br>

from skimage.segmentation import slic<br>
from skimage.color import label2rgb<br>
face_image = plt.imread('face.jpg')<br>
#Obtain the segmentation with 400 regions<br>
segments = slic(face_image, n_segments=400)<br>
#Put segments on top of original image to compare<br>
segmented_image = label2rgb(segments,face_image,kind='avg')<br>
#Show the segmented image<br>
plot_comparison(face_image, segmented_image,'segmented image, 400 superpixels')<br>

**OUTPUT:**

def show_image_contour(image, contours):<br>
    plt .figure()<br>
    for n, contour in enumerate(contours):<br>
        plt.plot(contour[:,1],contour[:,0],linewidth=3)<br>
    plt.imshow(image, interpolation='nearest',cmap='gray_r')<br>
    plt.title('contours')<br>
    plt.axis('off')<br>

from skimage import measure,data<br>
#obtain the horse image<br>
horse_image = data.horse()<br>
#Find the contours with a contstant level value of 0.8<br>
contours = measure.find_contours(horse_image,level=0.8)<br>
#Shows the image with contours found<br>
show_image_contour(horse_image,contours)<br>

**OUTPUT:**<br>
![image](https://user-images.githubusercontent.com/97939491/187880789-806b4a7c-b49f-4b37-9144-74acf5233973.png)<br>

from skimage.io import imread<br>
from skimage.filters import threshold_otsu<br>
image_dices = imread('diceimg.png')<br>
#Make the image grayscale<br>
image_dices = color.rgb2gray(image_dices)<br>
#obtain the optimal thresh value<br>
thresh = threshold_otsu(image_dices)<br>
#Apply thresholding<br>
binary = image_dices > thresh<br>
#Find contours at a constant value of 0.8<br>
contours = measure.find_contours(binary,level=0.8)<br>
#Show the image<br>
show_image_contour(image_dices,contours)<br>

**OUTPUT:**<br>
![image](https://user-images.githubusercontent.com/97939491/187881162-9bd23df3-1890-4ec8-bf0b-99943b7fe5a4.png)<br>

#create list with the shape of each contour<br>
shape_contours=[cnt.shape[0] for cnt in contours]<br>
#Set 50 as the maximum size of the dots shape<br>
max_dots_shape=50<br>
#Counts dots in contours excluding bigger than dots size<br>
dots_contours=[cnt for cnt in contours if np.shape(cnt)[0]<max_dots_shape]<br>
#Shows all contours found<br>
show_image_contour(binary,contours)<br>
#Print the dice's number<br>
print('Dices dots number:{}.'.format(len(dots_contours)))<br>

**OUTPUT:**<br>
![image](https://user-images.githubusercontent.com/97939491/187881509-d89c6a87-9477-42ec-9f66-3d28adde2768.png)<br>

**PROGRAM: EDGE DETECTION**

#Canny Edge detection<br>
import cv2<br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>
plt.style.use('seaborn')<br>
loaded_image = cv2.imread("Shape.png")<br>
loaded_image = cv2.cvtColor(loaded_image,cv2.COLOR_BGR2RGB)<br>
gray_image = cv2.cvtColor(loaded_image,cv2.COLOR_BGR2GRAY)<br>
edged_image = cv2.Canny(gray_image, threshold1=30, threshold2=100)<br>
plt.figure(figsize=(20,20))<br>
plt.subplot(1,3,1)<br>
plt.imshow(loaded_image, cmap="gray")<br>
plt.title("original Image")<br>
plt.axis("off")<br>
plt.subplot(1,3,2)<br>
plt.imshow(gray_image,cmap="gray")<br>
plt.axis("off")<br>
plt.title("GrayScale Image")<br>
plt.subplot(1,3,3)<br>
plt.imshow(edged_image,cmap="gray")<br>
plt.axis("off")<br>
plt.title("Canny Edge Detected Image")<br>
plt.show()<br>

**OUTPUT:**
![image](https://user-images.githubusercontent.com/97939491/187903094-c86edd46-eded-4bbc-991f-d8e10bdd0ab8.png)<br>

#Laplacian and Sobel Edge detecting methods<br>
import cv2<br>
import numpy as np<br>
from matplotlib import pyplot as plt<br>
# Loading image<br>
#imge = cv2.imread('SanFrancisco.jpg',) <br>
imge = cv2.imread('Shape.png',)<br>
#converting to gray scale<br>
gray = cv2.cvtColor(imge, cv2.COLOR_BGR2GRAY)<br>
# remove noise<br>
img = cv2.GaussianBlur (gray,(3,3),0)<br>
#convolute with proper kernels<br>
laplacian = cv2.Laplacian (img,cv2.CV_64F)<br>
sobelx = cv2.Sobel(img,cv2.CV_64F,1,0,ksize=5) # x <br>
sobely = cv2.Sobel(img,cv2.CV_64F,0,1,ksize=5) # y<br>
plt.subplot(2,2,1), plt.imshow(img,cmap = 'gray')<br>
plt.title('Original'), plt.xticks([]), plt.yticks([])<br>
plt.subplot(2,2,2), plt.imshow(laplacian, cmap = 'gray')<br>
plt.title('Laplacian'), plt.xticks([]), plt.yticks([])<br>
plt.subplot(2,2,3), plt.imshow(sobelx, cmap = 'gray')<br>
plt.title('Sobel x'), plt.xticks([]), plt.yticks([]) <br>
plt.subplot(2,2,4), plt.imshow(sobely,cmap = 'gray')<br>
plt.title('Sobel Y'), plt.xticks([]), plt.yticks([])<br>
plt.show()<br>

**OUTPUT:**
> ![image](https://user-images.githubusercontent.com/97939491/187903252-6a5a91fd-9e80-4e9b-8283-6e4292977280.png)<br>

#Edge detection using Prewitt operator<br>
import cv2<br>
import numpy as np<br>
from matplotlib import pyplot as plt <br>
img = cv2.imread('Shape.png')<br>
gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)<br>
img_gaussian = cv2.GaussianBlur (gray, (3,3),0)<br>
#prewitt<br>
kernelx = np.array([[1,1,1], [0,0,0],[-1,-1,-1]])<br>
kernely = np.array([[-1,0,1],[-1,0,1],[-1,0,1]])<br>
img_prewittx = cv2.filter2D (img_gaussian, -1, kernelx) <br>
img_prewitty = cv2.filter2D(img_gaussian, -1, kernely)<br>
cv2.imshow("Original Image", img)<br>
cv2.imshow("Prewitt x", img_prewittx)<br>
cv2.imshow("Prewitt y", img_prewitty)<br>
cv2.imshow("Prewitt", img_prewittx + img_prewitty)<br>
cv2.waitKey()<br>
cv2.destroyAllwindows()<br>

**OUTPUT:**<br>


#Roberts Edge Detection- Roberts cross operator<br>
import cv2<br>
import numpy as np<br>
from scipy import ndimage<br>
from matplotlib import pyplot as plt<br>
roberts_cross_v = np.array([[1, 0],<br>
                            [0,-1]])<br>
roberts_cross_h = np.array([[0, 1],        <br>
                            [-1, 0 ]] )<br>
img = cv2.imread("Shape.png",0).astype('float64')<br>
img/=255.0<br>
vertical = ndimage.convolve( img, roberts_cross_v )<br>
horizontal=ndimage.convolve( img, roberts_cross_h)<br>
edged_img = np.sqrt( np.square (horizontal) + np.square (vertical))<br>
edged_img*=255<br>
cv2.imwrite("output.jpg",edged_img)<br>
cv2.imshow("OutputImage", edged_img)<br>
cv2.waitKey()<br>
cv2.destroyAllWindows()<br>

**OUTPUT:**<br>

