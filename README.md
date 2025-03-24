# lelit mara x shot Timer

This project is inspired by [alexrus' Mara X Shot Timer](https://github.com/alexrus/marax_timer) and offers an enhanced version of the software for the shot timer. It is designed specifically for the Lelit MaraX and introduces several new features to improve usability and extend the lifespan of the OLED screen.

## Features and Improvements

- **Standby Mode:** The display automatically turns off after 5 minutes of inactivity, conserving power and prolonging the lifespan of the OLED screen.
- **Rotated Display:** The display is rotated 180 degrees to fit better in alternative enclosures or cases.
- ***Color Inversion:*** (default: not set) The colors on display will change every 60 seconds to save oled from burn ins. just uncomment line 65-71 if you want to have it.

## Getting Started

## Shopping List

|What? |price |amazon-link (DE)|
|------|------|-----|
|ESP8266| 13.99€|[ESP8266 NodeMcu Lua V2]([https://www.amazon.de/AZDelivery-NodeMCU-ESP8266-ESP-12E-Development/dp/B06Y1ZPNMS?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=1BWLX72PEW1FP&dib=eyJ2IjoiMSJ9.Mgs1zj8gUN2ED79C59YCQDf0BdsvpkmUDhbXskcoaPnXS2nCW1GSK-JmJodfYIRwuE69oFJmhSLKFoo-ZcpjC1KlIQ7zqNpE5i5isguOc2VmR292nht57UpT-k1TJ7Z8wqpFBjYKl5-fuSG-ARsG26SzYaRPsEpOo45ZIm9dD1-jbaBVnt_ogGavLQbT4fH44gP6wtlmgpA0kT6dKS0cmO3qDDucUy_1cqGNCbDQ3ZgDIj74f_TabXte3A-nOlvQhNyqoIr1Mpk2VkFZR9PF4avdxnfCSIBFQPiQsTn2BjOjPU8DRxOJAszSTnLZeVKEZ9viEEWb3clI3LgXJBU-olw6DzsRMIwoy2m9xcZMuiA.A4bvkRMYWgsmNWJqHzPqObG4gQV9hEcC2wrwNkZmO5A&dib_tag=se&keywords=ESP8266%2BNodeMcu&qid=1737982754&s=ce-de&sprefix=esp8266%2Bnodemcu%2Celectronics%2C91&sr=1-5&th=1](https://www.amazon.de/dp/B0CLXZ9VN9?ref=ppx_yo2ov_dt_b_fed_asin_title))|
|wires|9.76€|[Akozon Jumper Wire](https://www.amazon.de/dp/B07GH3K671?ref=ppx_yo2ov_dt_b_fed_asin_title)|
|oled screen|7.99€|[Hailege 0.96" I2C IIC OLED](https://www.amazon.de/dp/B07Z8Q6V9C?ref=ppx_yo2ov_dt_b_fed_asin_title)|
|reed sensor|6.99€|[Guuzi 3pcs Verdrahteter Türsensor](https://www.amazon.de/dp/B09QFXHS46?ref=ppx_yo2ov_dt_b_fed_asin_title&th=1)|
|*optional - power adapter*|*7.99€*|[Anker Power](https://www.amazon.de/Anker-Ladeger%C3%A4t-Schnellladeger%C3%A4t-USB-Ladeger%C3%A4t-kompatibel-Schwarz/dp/B0CNPHQGXX?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=24SWTHV5MTLCC&dib=eyJ2IjoiMSJ9.vYvAUXmYN6-I82dEDKlt_BG2tIm56DADmF4DcOqa-ygDpnBcpqDgNSEHM3BDvbTsN90R7w2G9bf4kzgtmq8RS5yclQf6PQEXthX40mHkpvF2UGWtGcd8q4o0uTjauJh7jjgZIJ1quR29mesMGKc2-v-2MDz_kBQ0KrdT56HJ7hna1fFjMMP5YgrOje1uzmQ5bDtjitLtbiSeNHYzshkDUzrHPYup-YKzOTAGP28LTak.PgDwc7x7w8mW6YvQibraT9rbnxb7jsN4jXb6wZPopSU&dib_tag=se&keywords=anker%2Bpower%2Badapter%2Busb&qid=1737983131&sprefix=anker%2Bpower%2Badapter%2Busb%2Caps%2C96&sr=8-4&th=1)|
|*optional - micro usb cablepower adapter*|*4.59€*|[micro usb cable](https://www.amazon.de/Ladekabel-Schnellladekabel-Datenkabel-Samsung-Motorola/dp/B089K2GN5M?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=BLXJ5LVUWOJ&dib=eyJ2IjoiMSJ9.qgBvRJNWyv91zaqn_BfqUTXaD4u1HLLyh8MZnVFrZK3m1GxA-PPmQwymlTEG6buxaT20CoGMrhFOajSmjx2jeEdH-sfxtoE4VN2k-CT7XqBLZ_gUkZEQUM0MKyYWL5TYk8J0m75XKrTDTSfJtjpMx2XeWSDrMm4SH4ykTGvybdOSQsXRjX1gejfCrRMBfAnQzfs-ujYGj0uiFgVBQY94JZzIMLQd5_nBnFCc6FGQNjg._MtrucUwoPrP9KlFGnZxcTSrzQ9fX1zXdvvB1ZQXjKA&dib_tag=se&keywords=mikro+usb&qid=1737983071&sprefix=mikro+usb+%2Caps%2C129&sr=8-10)|
|sumup|32.73€|-|

### Prerequisites

To use this software, you will need to add the required libraries to the Arduino IDE. Notably:
- **Timer by JChristensen:** If this library cannot be found in the Arduino Library Manager, you can add it manually as a ZIP file. You can download it from its [GitHub repository](https://github.com/JChristensen/Timer).

### Installation

1. Clone this repository or download it as a ZIP file.
2. Open the `.ino` file in the Arduino IDE.
3. Add all required libraries, including the Timer library mentioned above. - see alexrus' github for reference
4. Compile and upload the code to your microcontroller.
5. assemble - i found this video for reference https://youtu.be/e9FXYfr5ro4?si=SsbZIPRW2_kH2V5F&t=484

## Credits

This project builds on the work of [alexrus](https://github.com/alexrus), whose original shot timer provided the foundation for this improved version.

---

If you have any issues or suggestions, feel free to create an issue or submit a pull request!
