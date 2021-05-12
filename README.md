# ESP32cam-motion-detection
This is a motion detection system built on the ESP32-CAM board and a PIR sensor module that also sends an email with the image as an attachment. 

The board spends most of the time in sleep mode and wakes up to take an image once motion is detected. Once motion is detected, an interrupt routine is triggered. It takes the picture of the intruder or whatever, saves it on the file memory system of the board called SPIFFs, then using STMP protocols, it sends the image to a designated mail.
