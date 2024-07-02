# LED Switch Control with Interrupt

This project demonstrates how to control an LED using a switch with interrupt-driven programming in embedded C.

## Description

The pseudocode implements a simple system where an LED can be toggled ON and OFF by pressing a switch. It uses an interrupt-based approach, which allows the system to respond immediately to switch presses without constantly polling the switch state.

## Features

- Interrupt-driven switch detection
- LED toggle functionality
- Efficient use of microcontroller resources

## Hardware Requirements

- A microcontroller (specific model to be determined based on implementation)
- An LED
- A push-button switch
- Appropriate resistors for LED and switch (if needed)

## Pin Configuration

- LED_PIN: 5 (Output)
- SWITCH_PIN: 2 (Input with pull-up)

## Software Requirements

- Embedded C compiler compatible with your microcontroller
- Appropriate microcontroller SDK or libraries

## Implementation Notes

This code is provided as a pseudo-code example and needs to be adapted for your specific microcontroller. You will need to replace placeholder functions with the appropriate functions for your hardware:

- set_pin_mode()
- set_interrupt_trigger()
- attach_interrupt()
- read_pin()
- write_pin()
- clear_interrupt_flag()
- enable_global_interrupts()

## Usage

1. Set up your hardware according to the pin configuration.
2. Adapt the code for your specific microcontroller.
3. Compile and flash the code to your microcontroller.
4. Press the switch to toggle the LED state.

## Function Descriptions

- `main()`: Initializes the system and enters the main loop.
- `switch_ISR()`: Interrupt Service Routine for the switch.
- `init_GPIO()`: Initializes GPIO pins for LED and switch.
- `configure_switch_interrupt()`: Sets up the interrupt for the switch.
- `toggle_LED()`: Toggles the state of the LED.
