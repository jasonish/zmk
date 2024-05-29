# Clickety Split | MNML v1.13

![MNML v1.13](https://clicketysplit.ca)

Keyboard Designer: [clicketysplit.ca](https://clicketysplit.ca) \
GitHub: [ClicketySplit](https://github.com/ClicketySplit) \
Hardware Supported: Seeed Studio XIAO BLE

MNML (pronounced Minimal) is a 3x5x5m split keyboard with 4 auxiliary keys; MNML leverages Seeed Studio XIAO BLE microcontrollers.

## Features

- 3x5x5m Split Keyboard with 4 auxiliary switches.
- Support for Kailh Low Profile Choc switches with 18mm x 18mm spacing.
- All switch locations are socketed.
- Per-key RGB LEDs with power management.
- Support for 110mAh, 600mAh, or 700mAh batteries.
- Support for JST PH-2 Battery Connectors

# Building MNML ZMK Firmware

ZMK Firmware: [Introduction to ZMK](https://zmk.dev/docs/) \
Installation: [Installing ZMK](https://zmk.dev/docs/user-setup) \
Customization: [Customizing ZMK](https://zmk.dev/docs/customization) \
Development Environment: [Basic Setup](https://zmk.dev/docs/development/setup)

Build commands for the default keymap of MNML v1.13:

```
west build -d build/MNML/left -p -b seeeduino_xiao_ble -- -DSHIELD=clickety_split_mnml_left

west build -d build/MNML/right -p -b seeeduino_xiao_ble -- -DSHIELD=clickety_split_mnml_right
```

Build commands for your custom keymap of MNML v1.13:

```
west build -d build/MNML/left -p -b seeeduino_xiao_ble -- -DSHIELD=clickety_split_mnml_left  -DZMK_CONFIG="/workspaces/zmk-config/[your name]/mnml_v1.13/config"

west build -d build/MNML/right -p -b seeeduino_xiao_ble -- -DSHIELD=clickety_split_mnml_right  -DZMK_CONFIG="/workspaces/zmk-config/[your name]/mnml_v1.13/config"
```

# Support

If you have any questions with regards to MNML, please [Contact Us](https://clicketysplit.ca/pages/contact-us).

Clickety Split
For the love of split keyboards.
