# 9dofBlock
Python library for Intel Edison Sparkfun 9DOF block

This is a python library for communicating over I2C with SparkFun's 9DOF block. The 9DOF block uses a 3-axis accel, mag, and gyro from STMicroelectronics LSM9DS0 sensor.  

This library depends upon the intel mraa library and python numpy. If you don't have these, you can install the necessary dependencies using the dependencies.sh script via

sh ./dependencies.sh 

Then, you can run the example file with

python example.py

This file configures your 9DOF block and prints streaming accel, mag, gyro, and temperature data to the terminal window.

Registers for the accel, mag, and gyro configuration are given in the config.py file. Functions for setup, config, read, and write are given in the SF_9DOF.py file.

This is a work in progress. Currently, I'm not sure that the calibration on temperature is correct, but I wasn't too concerned with that sensor. 

For more information on how this works, check out my blog: http://stephaniemoyerman.com/?p=81

