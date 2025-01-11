# BM_Solar 

This little PCB uses a Texas Instruments bq25185 chip to act as a solar charge controller and battery managment system for single cell Lithium Polymer, Lithium Ion, or Lithium Phosphate batteries.

It was designed specifically to work as a hat for Waveshare RP2040-LoRa boards to improve charging and battery managment as a solar meshtastic router/repeater. It is the same footprint and will solder directly on the backside of a RP2040-LoRa board.

*(Though it was designed for the RP2040-LoRa, it will work with any other board that can run off of a 4.5V input.)*

# Specifications

- 1A max charge rate (limited by solar input)
- Stable 4.5V output to a device
- 3-18V solar input voltage
- Automatically switches to battery power once solar drops below 3V
- Uses a 10kOhm thermistor to stop charging below 0F/32C in order to prevent damage to the battery
- Much more efficient than built in solar charging on most Meshtastic boards with near MPPT efficiency
- Selectable charge profile between LiPo/LiIon and LFP with an easy jumper
- built in voltage divider for battery voltage monitoring
