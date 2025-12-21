# DigiKeyboard Library

A standalone Arduino library package of the original Digistump DigiSpark USB keyboard implementation.

This repository contains the **exact same source files from the latest available upstream version** (https://github.com/digistump/DigistumpArduino/tree/master/digistump-avr/libraries/DigisparkKeyboard). The only changes are the folder layout and metadata needed to ship it as a standard Arduino library, following the Arduino library format specification 1.5 (rev. 2.2), while keeping the original API and header name (`DigiKeyboard.h`).

I decided to package this as a standalone library because the original Digistump AVR core is deprecated, and maintained alternatives commonly used for Digispark/ATtiny projects (such as ATTinyCore) do not bundle DigiKeyboard. This repository makes it easy to install DigiKeyboard alongside your core without relying on the deprecated Digistump package.

To verify that the code matches upstream, compare file hashes or run a diff against the upstream folder linked above.

## Installation

### Option 1: Install using the Arduino IDE (ZIP)

1. Download this repository as a ZIP from GitHub
2. In Arduino IDE: Sketch > Include Library > Add .ZIP Library
3. Restart the Arduino IDE if needed

### Option 2: Manual installation (clone)

1. Clone this repository into your Arduino libraries folder:
   - Windows: Documents/Arduino/libraries
   - macOS: ~/Documents/Arduino/libraries
   - Linux: ~/Arduino/libraries
2. Restart the Arduino IDE

## Usage

Include the header as in the original library:

    #include <DigiKeyboard.h>

Check the `Examples` folder for usage examples.
