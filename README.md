# Face-Recognition-Camera
Overview-

For this project, we used Google’s Teachable Machine to develop a custom AI model capable of identifying basic facial emotions. The process began by activating the webcam and capturing a large set of images of ourselves displaying a range of expressions, including happy, sad, angry, and neutral. Each expression was organized into its own category so the model could clearly distinguish between different emotional states.

To build a strong and reliable dataset, we recorded many examples per category, making sure to include a wide variety of facial positions and subtle variations in expression. We also intentionally changed factors like camera angle, distance from the lens, and lighting conditions. These variations are important because they prevent the model from simply memorizing a single pose or lighting scenario. Instead, the model learns to recognize the general patterns and visual cues that define each emotion across different contexts.

By the end of training, the model wasn’t just matching exact images—it was learning the underlying features of each emotion. This allows it to make more accurate predictions when encountering new faces or slightly different environments, ultimately improving its real-world usefulness.



# Hardware Requirements:


| Component                  | Specification / Details | Notes                          |
|---------------------------|--------------------------|---------------------------------|
| Potentiometer             | 10kΩ                     | Used for LCD contrast control   |
| Mega 2560 Controller Board| Any revision             | Main microcontroller board      |
| LCD 1602 Module           | Standard, HD44780        | Text display (16×2 characters)  |
| USB Cable                 | USB-A to USB-B           | Connects Mega 2560 to computer  |
| Breadboard                | 830 tie-points           | Circuit prototyping platform    |
| Jumper Wires              | Male-to-male             | For wiring connections          |


# Software Requirements:

| Software / Tool          | Version                 | Purpose / Description                               |
|--------------------------|-------------------------|------------------------------------------------------|
| Python                   | 3.11                    | Used for data processing, scripts, and integration   |
| Arduino IDE              | Latest Version          | Uploads code and manages the Mega 2560 board         |
| Google Teachable Machine | Latest Version          | Trains the facial-emotion recognition AI model       |
| Visual Studio            | Latest Version          | Development environment for coding and debugging     |

# Hidden / Easily Overlooked Details:

1. Lighting and Webcam Angle
Consistent lighting and camera positioning are crucial for reliable emotion recognition in Teachable Machine.

2. Button Debouncing
Physical push buttons may trigger multiple signals without software debouncing, causing unexpected Arduino behavior.

3. USB Power Limits
High current draw from connected components (LEDs, sensors) can cause instability if the USB port cannot supply enough power.

4. Serial Communication Timing
Sending data too frequently from Python to Arduino can overflow the serial buffer, resulting in missed or delayed signals.

5. Dataset Diversity / Bias
Limited angles, lighting conditions, or facial types reduce the AI model's ability to generalize to new faces.

# Diagram:

 Webcam Input
      |
      v
Teachable Machine (AI Model)
      |
      v
Python Script
      |
      v
Arduino Mega 2560
      |
      v
Indicator LED / screen LED

# Demo Video:


# License:

MIT License
