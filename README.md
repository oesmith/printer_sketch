# printer sketch

A slimmed-down version of the printer sketch for arduino available at
https://github.com/freerange/printer

## hardware

This runs on an [Arduino ethernet board](http://proto-pic.co.uk/arduino-ethernet-without-poe/),
connected to a [thermal printer](http://proto-pic.co.uk/thermal-printer/).

For best results, power the Arduino using a 9V 2A wall-wart.  Power the
printer from the Vin line of the Arduino.  Connect TX and RX of the
printer to digital pins 2 and 3 on the Arduino (or wherever you'd prefer,
but remember to update the sketch accordingly).

## operation

The Arduino will boot up and poll the print server (specified in the
sketch) for new print jobs.  See the
[print server project](https://github.com/oesmith/simple_printer) for
more info.

