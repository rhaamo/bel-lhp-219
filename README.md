# BEP LHP 219

Notes and various about this indian military radio.

## Notes

All schematics are a "View From Top", like seeing in X-ray from the top. That was easier to reverse the PCBs.

Coil trimmers value is not known, markings on them are like "108 205", "108 201", etc.

Known values of caps might not be right, some have color code (top to bot: orange red red) or only military part number without a lookup table.

Unless determined by schematics, Test Points doesn't have indications on what they are.

## H6 - Filter In
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H6%20top.JPG" width="500px">
<br/>
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H6%20schematic.jpg" width="1000px">

TP
```
J3:
J4:
J5:
J6: RF in from pin3 (pin 3 of H14 connector, coax white/blue)
```

## H8 - A.G.C
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H8%20top.JPG" width="500px">
<br/>
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H8%20schematic.jpg" width="1000px">

## H11 - Summing Amplifier And 10V Regulator
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H11%20top.JPG" width="500px">
<br/>
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H11%20schematic.jpg" width="1000px">

## H12 - Transmitter IF
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H12%20top.JPG" width="500px">
<br/>
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H12%20schematic.jpg" width="1000px">

## H14 - Hinged PCB Modules (H6, H7, H8, H9A, H10, H11, H12, H13, Crystal Filters: CW and LSB)
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/hinged%20pcb.JPG" width="500px">
<br/>
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H14%20hinged%20pcb%20schematic.jpg" width="1000px">

## H25A - Voltage Regulator +18V +14V
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H25A%20top.JPG" width="500px">
<br/>
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H25A%20schematic.jpg" width="1000px">

Pins
```
1: +18V (TP J2)
4: +14V (TP J3)
7: In
10: GND
```

## H27 - Synthesizer assembly (H15, H16, H18, H20, H24-Y1, H21, H22, H25, H26)
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H27.jpg" width="500px">
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/scans/H27%20pt2.jpg" width="500px">

## H21 - Phase Comparator
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H21%20top.JPG" width="500px">
<br/>
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H21%20schematic.jpg" width="1000px">

## H4 - Tuned Amplifier Assembly
### H5-4
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H5-4%20top.JPG" width="500px">
<br/>
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H5-4%20schematic.jpg" width="1000px">

### H5-3
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H5-3%20top.JPG" width="500px">
<br/>
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H5-3%20schematic.jpg" width="1000px">

### H5-2
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H5-2%20top.JPG" width="500px">
<br/>
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H5-2%20schematic.jpg" width="1000px">

### H5-1
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H5-1%20top.JPG" width="500px">
<br/>
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H5-1%20schematic.jpg" width="1000px">

### Rotary selector and filters connection
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H5%20rotary.JPG" width="1000px">
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/scans/P1.jpg" width="500px"><br>
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/scans/P2.jpg" width="500px"><br>
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/scans/P3.jpg" width="500px"><br>

## Connectors

### H14 - Hinged PCB Connector
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/H14%20main%20connector.png" width="500px">

### Front panel (except frequency selectors)
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/scans/front%20panel.jpg" width="500px">

## Block diagrams
### HF
<img src="https://raw.githubusercontent.com/rhaamo/bel-lhp-219/master/RF%20block%20diagram.png" width="500px">


### Battery
24V.

```
A -
B +
C N/C
```

### Front power connector
Untested.

`+` goes to battery `+`, minus..., `?` are unknown.

```
+ -
 ? ?
? -
```

### Headsets

H189 or H250 might works, connector is a `U-183/U`, corresponding headset connector is `U-182B/U, U-229/U`.

## All modules
```
# Synthesizer                                               N 43547                             H27
BULOVA  A410181     TXCO-1 FREQ 3.5MHz      PIN 1. +18V, 2. OUT, 3. GND, 4. NC
Tuned Amplifier                                             N 43586                             H5
Coil Block                                                  N 43553                             H15
Voltage Controlled Oscillator                               N 43929                             H16 A
5 Bit D/A Converter And Summing & Buffer Amplifier          N 43847                             H18
Programmable Divider                                        1000 043 538 40                     H20
Phase Comparator                                            N 43537                             H21
Frequency Detector And Standard Divider                     N 43848                             H22
Voltage Regulator +18V +14V                                 1140 001 980 78                     H25A
Switching Regulator 5V                                      N 43531                             H26

# Main
Power Supply                                                N 43680                             H1
Driver                                                      N 43685                             H2
Aerial Filter, ALC & Metering Unit                          N 43655                             H3

# Hinged Module Assembly                                                                        H14
Filter In                                                   N 43706                             H6
Filter Out                                                  N 43707                             H7
A.G.C                                                       N 43708                             H8
Detector And Receive Audio                                  1140 006 871 52                     H9A
1750/1751KHz Generator                                      N 43710                             H10
Summing Amplifier And 10V Regulator                         N 43711                             H11
Transmitter IF                                              N 43712                             H12
Transmit Audio And Tone Generator                           N 43713                             H13
Crystal Filter CW Freq 1.75MHz
Crystal Filter LSB Freq 1.75MHz

# Front
Power Amp                                                   N 43668                             H4
```