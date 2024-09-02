# GPIO control

This is a simple python wrapper for pinctrl sysfs interface.
It is intended to be used on a Raspberry Pi.

Currently it only supports set and get pin state operations.

Because of how pinctrl works, there is no need to initialize pin direction.

## Purpose

This wrapper was created to control a relay board using a Raspberry Pi.
Using bash command keeps pin's state after the script ends.

## Usage

```python
from gpiocontrol import get, set, State

print(get(4))  # Get pin 4 state
set(4, State.HIGH)  # Set pin 4 to HIGH
```
