# Mooshimeter-PythonAPI
A python API relying on the BLED112 to talk to the Mooshimeter

Setup / Dependencies:
 -- Python 2.X
 -- pyserial
        Run “python -m pip install pyserial” in the command line (needs pip to be installed, but is already included in up-to-date python installations)
 -- bglib
        Get the bglib.py file from https://github.com/jrowberg/bglib/tree/master/Python
		Option 1: Copy bglib.py to this folder
		Option 2: Copy bglib.py in your Python Lib directory (usually C:/PythonXX/Lib)

Example.py:
This script is meant to demonstrate use of the Mooshimeter and BGWrapper classes.
The script does the following:
- Scan for BLE devices
- Filter for Mooshimeters
- Connect to the Mooshimeter with strongest signal
- Configure the meter to read Voltage in 60V range and Current in 10A range
- Begin streaming data and printing the results to the console
