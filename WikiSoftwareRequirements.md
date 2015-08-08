This wiki tries to list the expected requirements for an ideal ESD dataanalysis tool.


## Browsing through large number of TLP measurements ##

  * Comparing several IV curves side by side within browser GUI
  * immediate loading of IV curve
  * Immediate automatic analysis of IV curves: Vt1, It2, …
  * Easy manual change of these extracted parameters were needed
  * Changes are stored for future data loading
  * Direct comparison possible between TLP measurements for extracted parameters
  * Show (corrected) load line on the graph

## Waveform analysis of the TLP data ##

  * Browsing through waveform data by selecting points on the IV curve
    1. Comparing waveform data between different IV measurements at same current level or same pulse voltage
    1. Aligned pulse edges for in depth comparison
    1. Show V\*I waveform data
  * Selecting new averaging windows – multiple windows may be required – sliders with immediate influence on IV curve
  * Select new IV curve based on maximum voltage (overshoot) versus pulse voltage or versus actual extracted ESD current (several options may be required)
  * Extract integral (energy) in waveform data between certain markers (full pulse or only overshoot and above certain voltage level)
  * Create IV curve from raw data measured by other equipment (e.g. homebuilt pulser setup, not commercial TLP system) – including conversion to standard python/ESDtool data format

## Database functionalities ##

  * Enable database querries