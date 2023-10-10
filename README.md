# 277r

This repo contains improved source code for the Spin FV-1 DSPs in the 
Buchla format 288r Signal Delay module from Electronic Music Store.

This version contains the following improvements:

- All delay reads use linear interpolation, which greatly reduces
  digital artifacts when the delay time is modulated.
- A peak limiter is applied to the signal input, which controls
  runaway oscillation when the analog feedback mixer exceeds unity gain.
- A noise gate is applied to the audio modulation signal input,
  which reduces noise when no modulation signal is present.

## Usage

- The Spin source files can be used if you have the Spin IDE or another FV-1 compiler.
- The compiled hex file can be written to the EEPROMs with any EEPROM programmer.
- The module requires two identical EEPROMs

## DISCLAIMER

This code is not derived from the original source code, which I did not have access to.
The Buchla trademark is owned by Buchla U.S.A.
