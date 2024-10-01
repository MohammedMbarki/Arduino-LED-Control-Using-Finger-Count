# Arduino-LED-Control-Using-Finger-Count
Arduino LED Control Using Finger Count with open cv







## Setup Instructions

> [!IMPORTANT]
> This project requires both Arduino and Python development environments. This tutorial assumes you already have Python and the Arduino IDE installed on your computer. If not, you can follow the installation guides provided below:

- [Arduino IDE Installation Guide](https://docs.arduino.cc/software/ide/)
- [Python Installation Guide](https://wiki.python.org/moin/BeginnersGuide/Download)

In this project, Arduino and Python each play crucial roles:

*Arduino*: Arduino serves as the central controller for the hardware. It receives instructions from the Python script and manages the LEDs based on the detected number of fingers. Communication between the Arduino and the computer occurs through a serial port, allowing the Arduino to respond in real-time to the data received from the Python script.

*Python*: The Python script handles image processing and gesture recognition, utilizing the computer’s camera to detect how many fingers are being shown. By leveraging OpenCV, the script analyzes the image to determine the finger count and sends this data to the Arduino via serial communication, triggering the corresponding LED actions.



### IDEs
<div style="display: flex; gap: 10px;">
    <a href="https://code.visualstudio.com/" target="_blank" rel="noreferrer">
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vscode/vscode-original.svg" alt="VS Code" idth="48" height="48">
    </a>
    <a href="https://www.arduino.cc/" target="_blank" rel="noreferrer">
        <img src="https://cdn.worldvectorlogo.com/logos/arduino-1.svg" alt="Arduino IDE" width="48" height="48">
    </a>
</div>




# Arduino Setup


1-Build the Circuit: Assemble your hardware by following the provided circuit diagram, ensuring all components are correctly connected.

![Untitled Sketch_bb](https://github.com/user-attachments/assets/c83823cc-7889-449b-9c12-f25c8498bf5a) 


2-Open the Arduino Sketch: Launch the Arduino IDE and open the LedController.ino file.

3-Connect the Arduino: Plug your Arduino Uno into your computer via a USB cable.

![port1](https://github.com/user-attachments/assets/a2c4f767-621b-48be-a5bf-0a0dd9ba9bd5)
 # python setup 
 > [!IMPORTANT]
> Before you run the Python code, ensure that you've closed the Serial Monitor in the Arduino IDE. This will prevent any port conflicts that could stop Python from sending data to your Arduino.

1. Install the necessary Python libraries:
```bash
   pip install opencv-python mediapipe pyserial
   ```

2. Update the Python script to use the correct serial port, ensuring it matches the one identified during Arduino setup.
![port2](https://github.com/user-attachments/assets/b1493e0a-a2ae-43e0-b355-3c8f44f69619)

3. Run `FingerCountSender.py`.



# video reference 

[View the project attachments on GitHub](https://github.com/user-attachments/assets/fcd7bd6f-6503-4471-9a6c-ab7cafcd9738)
