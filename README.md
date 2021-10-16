# Ender5Plus
Ender 5 Plus

I, AND THE PARTIES INVOLVED, AM NOT RESPONSIBLE FOR ANY DAMAGE(S) CAUSED BY USING THE PROVIDED MODIFICATIONS. PROCEED AT YOUR OWN RISK!

Baseline firmware compiled from Kersey Fabrications 2.0.9.1-BTT-SKR-2-Ender5Plus-DualZ branch. Modifications made to work with my Ender 5 Plus with SKR 2 / TMC2209 / BLT / BMG direct drive extruder / E3D V6 hotend. This is not using Sensorless homing, but can be used. Still trying to figure it out myself. Please drop a comment if you know how to!

Modifications:

BMG Esteps - change to 415 (for BMG)
```
#define DEFAULT_AXIS_STEPS_PER_UNIT   { 80, 80, 800, 415 }
```
BMG Motor inverting - if your X axis moves the opposite way from the x-endstop change this to false
```
#define INVERT_X_DIR false
```
Thermistor - change for E3D V6 thermistor
```
#define TEMP_SENSOR_0 5
#define HEAT```ER_0_MAXTEMP 285

Nozzle to Probe Offset - changed for BLT with EVA carriage - https://contrib.eva-3d.page/printer-compatibility/ender-5/
```
#define NOZZLE_TO_PROBE_OFFSET { -28, -13, -3 }
```
