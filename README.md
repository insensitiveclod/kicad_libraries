# kicad_libraries

A collection of private/useful kicad libraries/footprints/etc, licensed under GPLv3

For both the schematic-symbols and the footprints, KICAD allows adding external libraries/paths. The same seems to not be true of extra 3d-packages, however.
This results in the situation that one has to hard-code paths to the .vrml-files that correspond to a specific footprint....rather unhandy.

As such, I have chosen to instead use the following approach:
- Find your kicad-installation's 'packages3d' directory
- make a symlink 'insensitiveclod' to this repo's 'parts/packages3d' dir
- All footprints with *custom* 3dpackage will use the 'insensitiveclod/*.vrml' syntax.

Part:
- 7 Segments display, common cathode, pin-layout according to TOS23101/SM22301
- BTS117 - Smart Low-side Power Switch ; Current-limiting FET-switch; TO-262-2 package
- Holtek HT16K33 LED-matrix/segment driver + keyboard scanner. 28-pin version
- MAXIM MAX31865AAP (20 pin SSOP version), RTD (PT100) to digital (SPI) convertor
- MAXIM MAX31865 module , adafruit-style; including screw-terminals as pins to connect to board

Footprint:
- 7-segment display, TOS23101/SM22301, 2.3" in size
- HT16K33, 28-pin SOP-A version; uses builtin SOIC28 3dpackge
- MAXIM MAX31865 Ardafruit module.

3D-package:
- 7-Segment display, TOS23101/SM22301, 2.3" in size

