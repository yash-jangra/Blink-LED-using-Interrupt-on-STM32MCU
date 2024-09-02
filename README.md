STM32F411CEU6 LED Blink on Button Press
Project Overview
This project demonstrates how to control an LED connected to the STM32F411CEU6 microcontroller using an external button. The LED will blink three times each time the button is pressed, and then turn off. This setup utilizes the STM32 HAL library for hardware abstraction.

Features
Button Press Detection: Uses the external interrupt feature to detect button presses.
LED Control: Blinks the LED three times in response to a button press.
Debouncing: Simple debouncing handled in the interrupt service routine to avoid multiple triggers from a single press.
Hardware Setup
Microcontroller: STM32F411CEU6
Button: Connected to PA0 (active low mode)
LED: Connected to PC13 (configured as a sink)
Software Requirements
STM32CubeIDE or any compatible IDE for STM32 development
STM32 HAL Library
Installation and Setup
Clone the Repository

bash
Copy code
git clone https://github.com/yourusername/stm32f411_led_blink.git
Open the Project Open the project in STM32CubeIDE or your preferred STM32 development environment.

Build the Project Compile the project to generate the firmware. Ensure that you have the STM32 HAL library properly set up.

Flash the Firmware Use an ST-Link or other compatible programmer to flash the firmware onto the STM32F411CEU6 board.

Usage
Power On: Connect the STM32F411CEU6 board to a power source.
Press the Button: Press the button connected to PA0.
Observe: The LED connected to PC13 will blink three times, each cycle lasting approximately 500 milliseconds.
Code Overview
main.c: Contains the main application code and initialization functions.
stm32f4xx_it.c: Contains the interrupt service routine for handling button presses and LED blinking.
Future Updates
This project will be updated with additional features and modifications, including:

PWM Control: Implement PWM for LED brightness control.
Additional Interrupts: Handling more complex interrupt scenarios.
Button Debouncing: Enhanced software or hardware debouncing techniques.
Additional Peripherals: Integration with other peripherals and sensors.
Contributing
Feel free to contribute to the project by opening issues or submitting pull requests. Contributions and suggestions are welcome!

License
This project is licensed under the MIT License - see the LICENSE file for detai
