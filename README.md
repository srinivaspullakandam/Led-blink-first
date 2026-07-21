The control board is the core of a circuit. After programming, it can be used to control other components in the circuit to achieve intended functions.
There are multiple versions of the Freenove control board.
following:
Freenove Control Board (minina)

Digital I/O ports is used to connect to other components or modules, to receive an input signal, or to send a control signal. Usually, we name it by adding a "D" in front of the number, such as D13 (pin 13).

USB interface is used to provide power, upload code or communicate with PC.

LED L is connected to digital I/O port 13 (pin 13).

LED TX, RX is used to indicate the state of the serial communication.

DC interface is connected DC power to provide power for the board.

Power ports can provide power for electronic components and modules.

Analog I/O ports can be used to measure analog signals.

LED ON is used to indicate the power state.


Getting Ready (Important)
Before starting building the projects, you need to make some preparation first, which is so crucial that you must not skip.

Arduino Software (IDE) is used to write and upload the code for Arduino Board.
First, install Arduino Software (IDE): visit https://www.arduino.cc/en/software/

Select and download corresponding installer based on your operating system. If you are a Windows user, please select the "Windows" to download and install the driver correctly.
After the downloading completes, run the installer. For Windows users, there may pop up an installation dialog box of driver during the installation process. When it is popped up, please allow the installation.
After installation is completed, an shortcut will be generated in the desktop.

Programs written with Arduino IDE are called sketches. These sketches are written in a text editor and are saved with the file extension.ino. The editor has features for cutting/pasting and for searching/replacing text. The console displays text output by the Arduino IDE, including complete error messages and other information. The bottom right-hand corner of the window displays the configured board and serial port. The toolbar buttons allow you to verify and upload programs, open the serial monitor, and access the serial plotter.

1) Open Arduino IDE. Click Tools>Board>Boards Manager...on the menu bar.
2) Enter Arduino UNO R4 in the searching box, and select ”Arduino UNO R4” and click on Install.
3) Click Yes in the pop-up “dpinst-amd64.exe”installation window. (Without it, you will fail to communicate with Arduino.) Thus far, we have finished installing the development support package.
4) Open the example sketch "Blink".
5) Select the board corresponding to the board you have in hands. Here we take Freenove Control Board (minina) as an example:
Select board "Arduino Uno R4 Minima". (Freenove control board is compatible with this board.)
6)Connect control board to your computer with USB cable.
Select the port. Note: Your port may be different from the following figure. On Windows: It may be COM4, COM5 (Arduino Uno R4 Minima) or something like that. On Mac: It may be /dev/cu.usbserial-710, /dev/cu.usemodem7101 (Arduino Uno R4 Minima) or something like that.
Need help? Contact support@freenove.com █
On Linux: It may be /dev/ttyUSB0, /dev/ttyACM0 or something like that.

Note: If there is more than one port and you cannot decide which one to choose, disconnect the USB cable and check the port. Then connect the USB cable and check the port again. The new one is the correct port.
Click "Verify" button.
The code is being compiled.
Wait a moment for the compilation to be completed.Shows the code size and percentage of space occupation. If there is an error in the code, the compilation will fail and the details are shown here.
Click "Upload" button.
Wait a moment, and then the uploading is completed.
After that, we will see the LED marked with "L" on the control board start blinking. It indicates that the code is running now!
