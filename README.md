# Awesome Continuous Testing Actions [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

GitHub Actions with examples mostly around Continuous testing for Microcontroller things.

## Contents

- [General info](#general-info)
- [Code checks](#code-checks)
  - [Actions](#actions)
  - [Compiling examples of Arduino library](#compiling-examples-of-arduino-library)
  - [Compiling specific sketch](#compiling-specific-sketch)
- [Surrounding](#surrounding)

## General info

- [Wikipedia CI](https://en.wikipedia.org/wiki/Continuous_testing) - Continuous testing on Wikipedia.
- [GitHub.com](https://github.com/features/actions) - GitHub Actions.
- [Guide](https://mirzafahad.github.io/2021-03-09-github-cicd-for-arduino-projects/) - Blog post about how to create a working CI for Arduino.

## Code checks

### Actions

- [compile-sketches](https://github.com/arduino/compile-sketches) - Arduino / compile - sketches.
- [arduino-cli](https://github.com/arduino/setup-arduino-cli) - Arduino / Arduino cli for workflows.
- [arduino-lint](https://github.com/arduino/arduino-lint-action) - Arduino lint for workflows.

### Compiling examples of Arduino library

For Arduino librarys, this compiles all provided examples. If all compiles its considered a pass.

- [DS3231](https://github.com/NorthernWidget/DS3231/blob/master/.github/workflows/compile-examples.yml) - Compile all examples, bare minimum.
- [STM32_CAN](https://github.com/pazi88/STM32_CAN/blob/main/.github/workflows/compile-examples.yml) - Compile all examples for STM32.
- [ESP32-A2DP](https://github.com/pschatzmann/ESP32-A2DP/blob/main/.github/workflows/compile-examples.yml) - Compile all examples for ESP32.
- [EMUcan](https://github.com/designer2k2/EMUcan/blob/main/.github/workflows/compile-examples.yml) - Compile specific examples for Arduino, ESP32, Teensy4 and STM32.
- [Stepper](https://github.com/arduino-libraries/Stepper/blob/master/.github/workflows/compile-examples.yml) - Compile for many targets (13!).

### Compiling specific sketch

For any Arduino Project, a provided sketch is compiled. If it compiles its considered a pass.

- [BerlinUhr](https://github.com/designer2k2/BerlinUhr/blob/main/.github/workflows/main.yml) - Compile sketch for ATtiny167.
- [can-multidisplay](https://github.com/designer2k2/can-multidisplay/blob/main/.github/workflows/compile-sketch.yml) - Compile sketch with many libs for Teensy4.
- [xmas-tree](https://github.com/designer2k2/xmas-tree/blob/master/.github/workflows/compile_sketch.yml) - Compile sketch for Digistump, ESP32C3 and ESP32S2.
- [BSB-LAN](https://github.com/fredlcore/BSB-LAN/blob/master/.github/workflows/platformio.yaml) - Compile Platformio project.
- [Arduino-CLI](https://github.com/arduino/arduino-cli-example/blob/master/.github/workflows/test.yaml) - Example from Arduino cli on how how to compile the blink sketch.

## Surrounding

- [EMUcan Library](https://github.com/designer2k2/EMUcan/blob/main/.github/workflows/clang-format-check.yml) - Arduino formatting check like CRTL+T in Arduino IDE.
- [Ethernet](https://github.com/arduino-libraries/Ethernet/blob/master/.github/workflows/check-arduino.yml) - Check for Arduino compliant library format.
- [Spell check](https://github.com/designer2k2/EMUcan/blob/main/.github/workflows/spell-check.yml) - English spell check.
- GitHub Markdown check.
- [pyroscope](https://github.com/pyroscope-io/pyroscope/blob/main/.github/workflows/lint-markdown.yml) - Markdown check for not working links.

## Contributing

Contributions welcome! Please only suggest tools/samples if they are actively maintained. Read the [contribution guidelines](contributing.md) first for other details. Make sure to provide a name, link, description, in alphabetical order.
