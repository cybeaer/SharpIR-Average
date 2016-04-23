# SharpIR-Average
Arduino Library for getting average distance from the Sharp IR GP2*

Forked from the Arduino page itself at http://playground.arduino.cc/Main/SharpIR

# Changes
Added max Distance for model 1080 (80cm) and changed from cm to mm.

At 30 tries and an tolerance of 98% its near 1mm exact at 67mm to 799mm.

The calculated values are for using with 5V

# How to Install/Use in IDE
to use create a SharpIR Folder in your library folder and paste these files, restart Arduino IDE.

For Details at using in Arduino Project look at the original at http://playground.arduino.cc/Main/SharpIR
quick one here:
//include lib

 #include &lt;SharpIR.h&gt;

//before setup()

 SharpIR sharp(analogSensorPin, 30, 98, 1080);

//at loop for getting distance

 sharp.distance()
