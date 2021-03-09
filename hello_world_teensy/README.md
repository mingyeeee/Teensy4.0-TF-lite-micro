# Hello World from Tensorflow Lite Micro Examples
Generates a sine function and displays it on the builtin led (led will pulse)
[Source](https://github.com/tensorflow/tensorflow/tree/master/tensorflow/lite/micro/examples/hello_world/arduino)

## Modifications 
* Modified arduino_output_handler.cpp to work with Teensy 4.0
* [Useful forum post](https://forum.pjrc.com/threads/57441-Tensorflow-on-Teensy)

## Setup 
Follow the instruction for Arduino to install the necessary libraries found on the [Tensorflow repo](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/lite/micro/examples/hello_world/README.md)
Place this folder with files into your Arduino folder and upload to your Teensy 4.0. 

## Troubleshooting
I had an issue with some CMSIS files missing the Tensorflow Lite for Micros library, check [this README](https://github.com/mingyeeee/Teensy4.0-TF-lite-micro/blob/main/README.md) for more info
