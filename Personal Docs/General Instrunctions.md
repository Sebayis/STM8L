# The pins connected to the Logic Analyser

| LOGIC CHx | Board Pin | Function | Color  |
| --------- | --------- | -------- | ------ |
| CH1       | A2        | MOSI     | White  |
| CH2       | A3        | MISO     | Brown  |
| CH3       | C6        | Clock    | Red    |
| CH4       | C5        | Enable   | Orange |
| GND       | GND       | GND      | Black  |

# Turn On an LED

The LEDs on the board are considered normal pins.

This way we can simply set the C7 pin to high `GPIOC->ODR |= GPIO_Pin_7;` to turn ON the blue LED, and `GPIOC->ODR &= ~GPIO_Pin_7;` to turn it OFF

The green LED is on pin E7: `GPIOE->ODR |= GPIO_Pin_7;`, `GPIOE->ODR &= ~GPIO_Pin_7;`
