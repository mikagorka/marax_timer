# Marax Timer

This project is inspired by [alexrus' Mara X Shot Timer](https://github.com/alexrus/marax_timer) and offers an enhanced version of the software for the shot timer. It is designed specifically for the Lelit MaraX and introduces several new features to improve usability and extend the lifespan of the OLED screen.

## Features and Improvements

- **Standby Mode:** The display automatically turns off after 15 minutes of inactivity, conserving power and prolonging the lifespan of the OLED screen.
- **Color Inversion:** To prevent burn-in on the OLED display, the color scheme inverts every 60 seconds during operation.
- **Rotated Display:** The display is rotated 180 degrees to fit better in alternative enclosures or cases.

## Getting Started

### Prerequisites

To use this software, you will need to add the required libraries to the Arduino IDE. Notably:
- **Timer by JChristensen:** If this library cannot be found in the Arduino Library Manager, you can add it manually as a ZIP file. You can download it from its [GitHub repository](https://github.com/JChristensen/Timer).

### Installation

1. Clone this repository or download it as a ZIP file.
2. Open the `.ino` file in the Arduino IDE.
3. Add all required libraries, including the Timer library mentioned above.
4. Compile and upload the code to your microcontroller.

## Credits

This project builds on the work of [alexrus](https://github.com/alexrus), whose original shot timer provided the foundation for this improved version.

---

If you have any issues or suggestions, feel free to create an issue or submit a pull request!
