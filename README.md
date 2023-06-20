## custom-object-detection_Landmine-detection-
### raspberry pi 4 yolov5 custom object detection_Landmine detection: 

```
sudo git clone https://github.com/abdallah180717/custom-object-detection_Landmine-detection-.git

sudo chown -R abdallah:abdallah custom-object-detection_Landmine-detection-/ 
```
if your user name pi:sudo chown -R pi:pi custom-object-detection_Landmine-detection-/

```
sudo apt-get install pyqt5-dev-tools

sudo pip3 install labelimg
```
#### Step  yolov5 raspberry pi4:  

```
sudo git clone https://github.com/abdallah180717/yolov5raspberry-pi4.git
cd yolov5raspberry-pi4/
ls   
```
(install.sh)output in terminal white font

```
sudo chmod 775  install.sh
```
to Activate

```
ls
```
( install.sh)output in terminal green font
```
sudo  ./install.sh
```
cd
```  
(:pi@raspberrypi)
```
sudo pip3 install yolov5
```
sudo chown -R pi:pi /usr/local/lib/python3.9/dist-packages/yolov5
```
Create 2 folders in: /home/pi

1-freedomtech

2-yoloresult

open Thonny and load file detect.py from 
pi /usr/local/lib/python3.9/dist-packages/yolov5

change lines (56,74)  to :

line 56:
```
source=ROOT / '/home/pi/freedomtech',  # file/dir/URL/glob/screen/0(webcam)
```
line 74:

```
project='/home/piyoloresult/',  # save results to project/name
```

Save the file and close.
#####################################################

sudo yolov5 detect                      ##for photo##

sudo yolov5 detect    --source 0       ##for video streem##

#####################################################



open folder: custom-object-detection_Landmine-detection-/img.py from the program  Thonny

you should create a folder name:  images in /home/pi/


connect the USB camera  to your raspberry pi and Run to capture 70 frame 


change line 12 to :
```
 cv2.imwrite("/home/pi/images/Fake_landmine%d.jpg" %cpt, frame) 
RUn//for capturing Fake_landmine 70 image
```
change line 12 to :
```
 cv2.imwrite("/home/pi/images/Landmine%d.jpg" %cpt, frame)
RUn//for capturing Landmine 70 image
```

connect the USB camera  to your raspberry pi and Run to capture 70 frame 

Open Terminal :
```
labelImg  
```
you will see program interface

label Fake_Landmine and real Landmine based your database:


![image](https://github.com/abdallah180717/custom-object-detection_Landmine-detection-/assets/90546119/e6f2ae9b-bb05-45ad-a9c3-bc69a87cb355)
![image](https://github.com/abdallah180717/custom-object-detection_Landmine-detection-/assets/90546119/11cc2a04-984f-4bbf-8c8a-f0c4a59cd926)
![image](https://github.com/abdallah180717/custom-object-detection_Landmine-detection-/assets/90546119/760b62eb-59be-4634-9379-bab7e84daac4)
![image](https://github.com/abdallah180717/custom-object-detection_Landmine-detection-/assets/90546119/0c80742c-03ee-4454-bf8c-6808acd086a5)

after finishing  the label Save all data in(validation,
training)   create a folder  /home/pi/data/

1-images:
-validation
-training

2-labels:
-validation
-training

![image](https://github.com/abdallah180717/custom-object-detection_Landmine-detection-/assets/90546119/489b41cf-ff43-4100-b4bd-ae7ec0de2f40)
![image](https://github.com/abdallah180717/custom-object-detection_Landmine-detection-/assets/90546119/875dbffb-95c8-4638-8c2f-e081f38b9201)

```
sudo zip -r  data.zip data/*
```

```
sudo zip -r  data.zip data/*
```
![image](https://github.com/abdallah180717/custom-object-detection_Landmine-detection-/assets/90546119/d1b2a6c8-b656-4df2-88d7-b2f695e3f606)

**upload a zip file to Google Drive**
![image](https://github.com/abdallah180717/custom-object-detection_Landmine-detection-/assets/90546119/cc92fc7b-4c9b-4f79-a94f-d1c021ac79e8)



open google  drive and  add a new  Google Colaboratory
then upload **yolov5customobj.ipynb**

![image](https://github.com/abdallah180717/custom-object-detection_Landmine-detection-/assets/90546119/29f53bea-5a09-41ac-b1f4-b25833a85d7e)


![image](https://github.com/abdallah180717/custom-object-detection_Landmine-detection-/assets/90546119/371bfdd5-e2c1-43e5-8efa-24634c6df3e3)



![ice_screenshot_20230620-110416](https://github.com/abdallah180717/custom-object-detection_Landmine-detection-/assets/90546119/6c1c2f41-1cb4-476d-a163-54ad03960dd0)


![Uploading image.png…]()













