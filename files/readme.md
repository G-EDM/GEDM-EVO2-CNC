The sensorboard and the pulseboard are connected with 3 JST connectors.

The connectors are placed at the exact same position. Don't use the wrong connector!
I shared a few images in the past where the PWM from the sensorboard was connected to the 5v output on the
pulseboard. It will burn the ESP32.

Sensorboard => Pulseboard

J10 => J8
J11 => J2
J9  => J7

Before connecting J9 to J7 make sure the voltage on J7 is below 5v! This is important. Use the Poti on the pulseboard to adjust it while
the PSU is ON. The output of J7 should remain a little below 5v at the max voltage provided from the DPM.

If a higher voltage is used adjust the Poti again. 
If 80v is used the output should be 4.8v while the big terminal is at 80v.
If 60v is used the output should be 4.8v while the big terminal is at 60v.

The board has 100v Zener diodes. Up to 90v should be ok.

The sensorboard provides 3.3v output and isolated 5v output. It is not used for anything yet.
The pulseboard provides 5v output that is also not used.

The pulseboard also provides a 12v output to connect a fan but it is not tested. Cheap high speed fans may introduce noise. There are flyback diodes
but if used connect a larger slow fan like a 120mm arctic fan.


# DPM to pulseboard

Connect the DPM8605 negative to the left side of the left big terminal (J19) and the positive to the right side of the same terminal.

The left side of the right terminal (J17) is bridged to the left terminals positive. The Shunt and wire is always hot and only GND is switched.
Connect the left side of J17 to one side of the shunt and the other side is the spark positive output.
The spark negative goes back into the right side of J17.

# Shunt to sensorboard
Connect both sides of the shunt to the sensorboard J5. It is no problem to wire it wrong here. If connected wrong it will not provide a feedback but will not destroy anything. Just swap the wire if there is no feedback.


