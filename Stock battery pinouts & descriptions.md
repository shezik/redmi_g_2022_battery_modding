# G16B01W for TM2135 battery pinouts & descriptions

## Basic information
```
Model No.: G16B01W / 4ICP4/63/92
Manufacturer: Sunwoda Electronic Co.,Ltd.
Charge voltage limit: 17.4 V DC
Rated voltage: 15.2 V DC
Rated capacity: 3620 mAh / 55.02 Wh
```

## Battery pinouts & descriptions
```
Front view of the battery-side connector.
For the connector on the motherboard, reverse the pin order.

              ┌────┐
┌──┬──┬──┬──┬─┴┬──┬┴─┬──┬──┬──┬──┐
│ 1│  │  │  │  │  │  │  │  │  │11│
└──┴──┴──┴──┴──┴──┴──┴──┴──┴──┴──┘

 1. RTC           Real-time clock power source       O   3.347 V to ground, regardless of B/I
 2. SMBD          SMBus Data?                        ?   Haven't tested
 3. SMBC          SMBus Clock?                       ?   Haven't tested
 4. BAT_PRS#      Battery Presence (Low-active)      O   10K Ohm to ground, used to notify motherboard of battery presence. (Haven't tested)
 5. P+            Battery Positive                   IO  0.002 V w/o B/I; battery voltage w/ B/I
 6. P+            Battery Positive                   IO  Connected to 5
 7. P+            Battery Positive                   IO  Connected to 5
 8. B/I           Battery Inserted (Low-active)      I   When pulled to ground by 10K Ohm resistor on motherboard, P+ output is activated.
 9. GND           Ground                             IO  Ground
10. GND           Ground                             IO  Connected to 9
11. GND           Ground                             IO  Connected to 9
```
