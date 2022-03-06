---
layout: post
title:  "Power_Consumption"
date:   2022-01-25 13:00:00 -0500
categories: design
---

Battery Life Calculation Analysis:
To calculate the battery life, the following formula is used:
Battery life (h) = Capacity (Ah) / Current (A)
We chose the battery with a capacity of 1400mAh

The Teensy 4.1 Development Board as our controller consumes approximately 100mA current and has a nominally 5V "Vin" pin that is limited to the range 3.6V to 5.5V. 
Since we are going to connect all the other components to the teensy board, we need to make sure that the total current draw does not exceed the 100mA limit and enough voltage will be supplied to all the components by the controller board. The total current draw of the system is summaries in the table below

| Component name        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| Current and voltage Consumption
MPU Sensor for Pen-Tip Localization:
MPU-6500        | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |



https://www.amazon.ca/gp/product/B07P5YZ7ZD/ref=ppx_yo_dt_b_asin_title_o05_s00?ie=UTF8&psc=1


3-5v (internal low dropout regulator)
1 Amps
Touch Sensor for Gesture Recognition:
Rasbee TTP223B Digital Touch Sensor Capacitive
https://www.amazon.ca/gp/product/B07CQB7DYB/ref=ppx_yo_dt_b_asin_title_o02_s00?ie=UTF8&psc=1


Power supply voltage VCC: 2.0--5.5 V(Typical 3V)
Output high VOH: 0.8VCC
Output low VOL: 0.3VCC
Output Pin Sink Current (@ VCC = 3V, VOL = 0.6V): 8mA
Output pin pull-up current (@ VCC = 3V, VOH = 2.4V): 4 mA
Bluetooth Pairing Hardware:
DSD TECH HC-06 Wireless Bluetooth Serial Transceiver Support Module Slave and Master
https://www.amazon.ca/gp/product/B01FCQZ8VW/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1


3.3V LDO input voltage 3.6 ~ 6V, current is about 30mA unpaired, paired about 10mA


