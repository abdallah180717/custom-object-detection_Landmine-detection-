# custom-object-detection_Landmine-detection-
raspberry pi 4 yolov5 custom object detection_Landmine detection 

sudo git clone https://github.com/abdallah180717/custom-object-detection_Landmine-detection-.git

sudo chown -R abdallah:abdallah custom-object-detection_Landmine-detection-/ 

###if your user name pi:sudo chown -R pi:pi custom-object-detection_Landmine-detection-/##

sudo apt-get install pyqt5-dev-tools

sudo pip3 install labelimg

Step  yolov5 raspberry pi4:  

sudo git clone https://github.com/abdallah180717/yolov5raspberry-pi4.git




open folder: custom-object-detection_Landmine-detection-/img.py from the program  Thonny

you should create a folder name:  images  ,in /home/pi/

change line 12 to : cv2.imwrite("/home/pi/images/Fake_landmine%d.jpg" %cpt, frame) //for capturing Fake_landmine 

connect the USB camera  to your raspberry pi and Run 






