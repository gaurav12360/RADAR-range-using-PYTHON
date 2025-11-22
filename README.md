# RADAR-range-using-PYTHON

Aim:
To calculate the maximum range of a radar system using the Radar Range Equation and verify the results through Python programming.

Theory:
The Radar Range Equation is a fundamental formula used in radar system design to determine the maximum range at which a radar can detect a target. It is given by:


Procedure
1.	Set Up the Python Environment: Ensure that Python is installed on your system. You can use Anaconda for managing Python packages and environments, or any other Python IDE of your choice.
2.	Import Necessary Libraries: Import the math library in Python.
3.	Define the Radar Range Equation Function: Create a function to calculate the maximum range using the Radar Range Equation.
4.	Input Parameters for the Radar System: Define the input parameters such as transmitted power, transmitter gain, receiver gain, radar frequency, radar cross section, and minimum detectable power.
5.	Calculate the Maximum Range: Use the function to calculate the maximum range of the radar.
6.	Execute the Program: Run the Python script to calculate and display the maximum range of the radar.

Program:
```
pt = 1:5:1000;
gt = 30;
sigma = 1;
smin = 15;
wavelength = 10;
gr = 8;
r = ((pt * gt * gr * wavelength^2 * sigma) ./ ((4 * %pi)^3 * smin)).^(1/4);
subplot(3,1,1);
plot(pt, r);
gt = 1:5:1000;
pt = 12;
subplot(3,1,2);
plot(gt,r);
gr = 1:5:1000;
pt = 14;
subplot(3,1,3)
plot(gr,r);
```
Output waveform:

<img width="763" height="729" alt="image" src="https://github.com/user-attachments/assets/25289a87-6b52-46fd-9a5a-f10db68df32e" />

Tabulation
<img width="772" height="1213" alt="image" src="https://github.com/user-attachments/assets/b772cb00-07b5-4b44-9cc3-98e7768708e8" />



Result:

Thus, the maximum range of a radar system using the Radar Range Equation is verified through a Python program.
