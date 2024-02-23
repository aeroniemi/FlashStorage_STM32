# FlashStorage_STM32 Library but different

It's like the original library, except edited to match the API from the [RP2040 arduino implementation](https://arduino-pico.readthedocs.io/en/latest/eeprom.html). Designed to work with my port of Mobiflight for the STM32 series microcontroller.

Docs are same as the original library, but with the following changes:
- setCommitASAP/getCommitASAP are gone - there is no automatic commit to memory, so you must call commit() once you're done
- new dummy method EEPROM.begin(num) - doesn't do anything but keeps stuff designed for the RP2040 happy
