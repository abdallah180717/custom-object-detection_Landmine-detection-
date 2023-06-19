# custom-object-detection_Landmine-detection-
raspberry pi 4 yolov5 custom object detection_Landmine detection 

sudo git clone https://github.com/abdallah180717/custom-object-detection_Landmine-detection-.git

sudo chown -R abdallah:abdallah custom-object-detection_Landmine-detection-/ 

###if your user name pi:sudo chown -R pi:pi custom-object-detection_Landmine-detection-/##

sudo apt-get install pyqt5-dev-tools

sudo pip3 install labelimg

Step  yolov5 raspberry pi4:  

sudo git clone https://github.com/abdallah180717/yolov5raspberry-pi4.git

cd yolov5raspberry-pi4/

ls   ##(install.sh)output in terminal white font

 
sudo chmod 775  install.sh ##to Activate
 
ls   ##( install.sh)output in terminal green font

sudo  ./install.sh

clear

cd   ### (:pi@raspberrypi)

sudo pip3 install yolov5

clear

sudo chown -R pi:pi /usr/local/lib/python3.9/dist-packages/yolov5

Create 2 folders in: /home/pi

1-freedomtech

2-yoloresult

open Thonny and load file detect.py from 
pi /usr/local/lib/python3.9/dist-packages/yolov5

change lines (56,74)  to :

line 56:source=ROOT / '/home/pi/freedomtech',  # file/dir/URL/glob/screen/0(webcam)

line 74:project='/home/piyoloresult/',  # save results to project/name


Save the file and close.
#####################################################

sudo yolov5 detect                      ##for photo##

sudo yolov5 detect    --source 0       ##for video streem##

#####################################################



open folder: custom-object-detection_Landmine-detection-/img.py from the program  Thonny

you should create a folder name:  images in /home/pi/


connect the USB camera  to your raspberry pi and Run to capture 70 frame 


change line 12 to : cv2.imwrite("/home/pi/images/Fake_landmine%d.jpg" %cpt, frame) 
RUn//for capturing Fake_landmine 70 image

change line 12 to : cv2.imwrite("/home/pi/images/Landmine%d.jpg" %cpt, frame)
RUn//for capturing Landmine 70 image


connect the USB camera  to your raspberry pi and Run to capture 70 frame 






