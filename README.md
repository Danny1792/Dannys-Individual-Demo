# Face-Recognition-Camera
Overview

For this project, we used Google’s Teachable Machine to develop a custom AI model capable of identifying basic facial emotions. The process began by activating the webcam and capturing a large set of images of ourselves displaying a range of expressions, including happy, sad, angry, and neutral. Each expression was organized into its own category so the model could clearly distinguish between different emotional states.

To build a strong and reliable dataset, we recorded many examples per category, making sure to include a wide variety of facial positions and subtle variations in expression. We also intentionally changed factors like camera angle, distance from the lens, and lighting conditions. These variations are important because they prevent the model from simply memorizing a single pose or lighting scenario. Instead, the model learns to recognize the general patterns and visual cues that define each emotion across different contexts.

By the end of training, the model wasn’t just matching exact images—it was learning the underlying features of each emotion. This allows it to make more accurate predictions when encountering new faces or slightly different environments, ultimately improving its real-world usefulness.



# Hardware Requirements


| Component                  | Specification / Details | Notes                          |
|---------------------------|--------------------------|---------------------------------|
| Potentiometer             | 10kΩ                     | Used for LCD contrast control   |
| Mega 2560 Controller Board| Any revision             | Main microcontroller board      |
| LCD 1602 Module           | Standard, HD44780        | Text display (16×2 characters)  |
| USB Cable                 | USB-A to USB-B           | Connects Mega 2560 to computer  |
| Breadboard                | 830 tie-points           | Circuit prototyping platform    |
| Jumper Wires              | Male-to-male             | For wiring connections          |
