# TheInvisibleEye
I have designed and developed a cost-effective camera system to enhance security through real time video streaming. 
It has been done by integrating the ESP-32 Camera module to enable live streaming capabilities, an RFID reader for authorized access control and a Bluetooth module for 
receiving notifications on a mobile phone.
Components used:  
ESP32 Camera: The ESP32 camera will perform live streaming. It will do the face recognition task as well. The moment any unknown face is detected, it’ll click a picture of the 
same and the photo will get saved in the device connected with the camera. The photo will be saved on google drive too. 
RFID sensor: The RFID sensor’s task is to detect “known” users who’ll be having a RFID tag/key. If it detects the presence via the tag/key, the automated door will open else 
it will ll remain closed. 
PIR Sensor: Its major task is to detect motion. 
Bluetooth module: For sending messages to the receiver’s phone number if unknown people are detected. 

Structure of the project: 

The ESP32 camera will continue live streaming. 
If a RFID sensor detects the person with the key/tag, the ESP32 camera will click its picture just to be sure with extra security. 
If the RFID sensor doesn’t detect anything but the PIR does for around 2 minutes (i.e. an unknown person is encountered), a message will be sent to the receiver’s phone number. 
If both RFID and PIR sensors don’t detect anything, live streaming continues.
