# Teensy4.0-TF-lite-micro
Repo with Tensorflow lite for MCUs example code modified to work with Teensy 4.0. [Source](https://github.com/tensorflow/tensorflow/tree/master/tensorflow/lite/micro/examples)

## Currently working
* Hello World sine generator
* Person Detection

## To Do
- [ ] Wake word detection

## Troubleshooting 
If there is an error that states somesort of CMSIS compiler header file does not exist, please navigate to "tensorflow\lite\micro\tools\make\downloads\cmsis\CMSIS\Core\Include"
in your "Arduino\libraries" folder and ensure that cmsis_complier.h and cmsis_gcc.h both exist. If something is missing, you can find these files in [this repo](https://github.com/ARM-software/CMSIS_5/tree/develop/CMSIS/Core/Include) where you can add them to your local directory
