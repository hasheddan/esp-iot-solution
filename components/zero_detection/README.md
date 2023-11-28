[![Component Registry](https://components.espressif.com/components/espressif/button/badge.svg)](https://components.espressif.com/components/espressif/button)

# Component: Zero_Detection
[Online documentation](https://docs.espressif.com/projects/esp-iot-solution/en/latest/input_device/button.html)

After creating a new zero detection object by calling function `zero_detect_create()`, the zero detection object can create many events.

List of supported events:
 * Button pressed
 * Button released
 * Button pressed repeat
 * Button press repeat done
 * Button single click
 * Button double click
 * Button multiple click
 * Button long press start
 * Button long press hold
 * Button long press up

![](https://dl.espressif.com/button_v2/button.svg)

There are three ways this driver can handle buttons:
1. Buttons connected to standard digital GPIO
2. Multiple buttons connected to single ADC channel
3. Custom button connect to any driver

## Add component to your project

Please use the component manager command `add-dependency` to add the `zero_detection` to your project's dependency, during the `CMake` step the component will be downloaded automatically

```
idf.py add-dependency "espressif/zero_detection=*"
```