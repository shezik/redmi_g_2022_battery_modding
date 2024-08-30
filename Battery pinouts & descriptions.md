# G16B01W for TM2135 Battery pinouts & descriptions

## Basic information
Model No.: G16B01W / 4ICP4/63/92
Manufacturer: Sunwoda Electronic Co.,Ltd.
Charge voltage limit: 17.4 V DC
Rated voltage: 15.2 V DC
Rated capacity: 3620 mAh / 55.02 Wh

## Battery pinouts
```
Front view of the battery-side connector.
For the connector on the motherboard, reverse the pin order.

               ┌──┐
┌──┬──┬──┬──┬──┼──┼──┬──┬──┬──┬──┐
│ 1│  │  │  │  │  │  │  │  │  │11│
└──┴──┴──┴──┴──┴──┴──┴──┴──┴──┴──┘

 1. RTC          Real-time clock power source
 2. SMBD         SMBus Data
 3. SMBC         SMBus Clock
 4. BAT_PRS#     Battery Presence (Low-active)
 5. P+           Battery Positive
 6. P+           Battery Positive
 7. P+           Battery Positive
 8. B/I          Battery Inserted?
 9. GND          Ground
10. GND          Ground
11. GND          Ground
```

## Pin descriptions
```
 1. RTC        O  3.347 V to ground, regardless of B/I
 2. SMBD       ?  Haven't tested
 3. SMBC       ?  Haven't tested
 4. BAT_PRS#   O  10K Ohm to ground, used to notify motherboard of battery presence?
 5. P+        IO  0.002 V w/o B/I; battery voltage w/ B/I
 6. P+        IO  Connected to 5
 7. P+        IO  Connected to 5
 8. B/I        I  When pulled to ground (usually 10K Ohm), activates P+ output.
                  10K Ohm pull-down resistor is present on motherboard.
 9. GND       IO  Ground
10. GND       IO  Connected to 9
11. GND       IO  Connected to 9
```
