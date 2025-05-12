# CC3220S-LAUNCHXL Thermostat Project
      
## Overview

This project implements a basic thermostat on the Texas Instruments CC3220S-LAUNCHXL LaunchPad using C++ and the Texas Instruments SimpleLink CC3220S SDK. It demonstrates GPIO control for an LED (simulating a heater), temperature sensing using an I2C temperature sensor (TMP11X, TMP116, or TMP006), and UART communication for reporting data. The thermostat allows users to adjust the temperature set-point via button inputs.

## Features

* **Temperature Sensing:** Reads ambient temperature from an I2C-based temperature sensor (TMP11X, TMP116, or TMP006).
* **Set-Point Adjustment:** Allows increasing and decreasing the temperature set-point using GPIO button inputs.
* **Heat Control (LED Simulation):** Controls an LED to simulate the activation/deactivation of a heater based on the ambient temperature and the set-point.
* **UART Communication:** Reports temperature readings, set-point values, heating status, and elapsed time via UART.
* **Task Scheduling:** Implements a simple task scheduler to manage the periodic execution of different functions.
* **Interrupt-Driven Input:** Uses GPIO interrupts to handle button presses for set-point adjustment.

## Code Structure

* `src/gpiointerrupt.c`: Contains the main application logic, including:
    * Initialization of UART, I2C, GPIO, and Timer peripherals.
    * Task scheduling implementation.
    * Functions for reading temperature, adjusting the set-point, and controlling the simulated heater (LED).
    * GPIO interrupt handlers for button inputs.
* `src/main_nortos.c`: Provides the entry point for the application and initializes the NoRTOS environment.
* `ti_drivers_config.h`: Header file containing driver configurations for the target platform.

## Hardware Requirements

* Texas Instruments CC3220S-LAUNCHXL LaunchPad.
* I2C temperature sensor (TMP11X, TMP116, or TMP006).
* LED.
* Push buttons.
* Wiring (breadboard, jumper wires) (if necessary for external components).

## Software Requirements

* Texas Instruments SimpleLink CC3220S SDK.
* Compiler for CC3220S (e.g., TI Code Composer Studio or GCC).

## Setup

1.  **Hardware Setup:**
    * Connect the I2C temperature sensor, LED, and push buttons to the appropriate GPIO pins on the CC3220S-LAUNCHXL LaunchPad. Refer to the project's hardware schematic (if available) or the code (`ti_drivers_config.h` or comments in `gpiointerrupt.c`) for pin assignments.
2.  **Software Setup:**
    * Install the TI SimpleLink CC3220S SDK.
    * Install a compatible C++ compiler for the CC3220S.
    * Import the project into your IDE (e.g., Code Composer Studio) or set up a build environment.
3.  **Code Compilation:**
    * Compile the C++ code using the CC3220S compiler.
4.  **Code Upload:**
    * Flash the compiled code onto the CC3220S-LAUNCHXL LaunchPad.

## Usage

1.  Power on the CC3220S-LAUNCHXL LaunchPad.
2.  The program will start reading temperature data and controlling the LED.
3.  Use the push buttons to:
    * Increase the temperature set-point.
    * Decrease the temperature set-point.
4.  Observe the LED behavior:
    * LED ON: Simulated heater is active (ambient temperature is below the set-point).
    * LED OFF: Simulated heater is inactive (ambient temperature is at or above the set-point).
5.  View the UART output to see temperature readings, set-point values, heating status, and elapsed time.

## Important Notes

* The `ti_drivers_config.h` file contains hardware-specific configurations. Ensure that the pin assignments in this file match your hardware setup.
* The code includes a basic task scheduler to manage the periodic execution of temperature reading, set-point adjustment, and heat control logic.
* The I2C temperature sensor address may vary. The code attempts to detect the sensor's address, but verify that it matches your hardware.
* This project provides a basic thermostat implementation and can be extended with features such as:
    * More sophisticated control algorithms (e.g., PID control).
    * Displaying information on an LCD.
    * Adding network connectivity (the CC3220S supports this).

## Acknowledgments

* Texas Instruments for the SimpleLink CC3220S SDK and CC3220S-LAUNCHXL LaunchPad.
