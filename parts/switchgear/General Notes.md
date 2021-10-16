# General Notes

An assorted list of notes which may be useful for other folks building HV systems

## In general, it's better to use high voltage over high current.
It makes buying equipment much easier if you have a ~100v system over a ~48v system for the same number of cells and you'll still get the same overall power output.
Calculations for this for 15Ah, 3.2v cells run at 1536Wh for a 102.4v system (32 series cells), or the same cells in a 2p16s configuration for 30Ah per pair, gives the same 1536Wh but now we have to deal with 30Ah/cell (which in my case worked out to be a possible pulse current for 10C cells of 300A, a nightmare to source 300+A DC contactors, controllers, etc.)

Some example calculations, including working:
```
In Series (32s):

  P = I * V,
  P = (Cell Ah rating) * (32 * Cell Nominal Voltage)
  P = (15) * (32 * 3.2)
  P = 15 * 102.4
  P = 1536 Wh

In Parallel Pairs (16s2p):

  P = I * V,
  P = (2 * Cell Ah rating) * (16 * Cell Nominal Voltage)
  P = (2 * 15) * (16 * 3.2)
  P = 30 * 51.2
  P = 1536 Wh
```
