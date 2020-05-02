# DS3231 For PSoC

This is a library-ish thing for the DS3231 RTC and PSoC, with code based on and loosely ported from AdaFruit's RTClib.

It's tested on the PSoC 5LP CY8CKIT-059, but should work with any PSoC 5LP and I imagine other PSoCs have similar APIs for the I2C components. 

## How To Use
The most important part is to add `DS3231.c` and `DS3231.h` to your project. Then, this library relies on a I2C component called `I2CRTC` that should be connected to a DS3231 (might work with DS3232 too?). 

This comes with a `DateTime` struct that I adapted from AdaFruit's DateTime class. This comes with a few functions.
