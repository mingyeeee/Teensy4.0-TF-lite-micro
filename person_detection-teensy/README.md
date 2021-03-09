# Person Detection from Tensorflow Lite For Micro Examples 
Uses an Arducam mini 2mp plus and several LEDs to indicate detection and inference.
[Source code](https://github.com/tensorflow/tensorflow/tree/master/tensorflow/lite/micro/examples/person_detection/arduino)

## Modifictions 
* Added code to arduino_image_provider.cpp to improve camera performance
* Added code to person_detect_model.cpp to allocate model into flash memory because the teensy's RAM is partitioned so the model does not fit
* Modified arduino_detection_responder.cpp to work with external LEDs instead of the builtin led found on the Arduino Nano 33 Sense

## Hardware Setup
Arducam Pins | Teensy Pin
------------ | -------------
CS | 7
MOSI | 11
MISO | 12
SCK | 13
GND | GND
VCC | 3.3V
SDA | 18
SCL | 19

LED | Teensy Pin
------------ | -------------
Red (person detected) | 2
Green (no person detected) | 1
Blue (inference indicator) | 0

## Software Setup
Follow the steps for Arduino on this Tensorflow README [here](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/lite/micro/examples/person_detection/README.md) for instructions on setting up the necessary libraries  

Place this folder with the files into the Arduino directory and upload to your Teensy 4.0
