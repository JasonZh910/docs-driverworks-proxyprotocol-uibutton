## COLD\_START\_TIME

Note that this notification will be deprecated from the proxy in the near future. Control4 recommends using device specific properties for this value.

Used to inform the proxy that the hardware Cold Start level has changed.  This is useful for hardware such as Control4’s Gen3 lighting where the hardware supports temporarily setting the brightness to a level for this number of milliseconds in order to 'jump start' the capacitors/ballasts on LED and florescent lights.  This value changes over time as capacitors and ballasts age.

### Name

`COLD_START_TIME ()`



| Parameter  | Type | Description                                                                       |
| ---------- | ---- | --------------------------------------------------------------------------------- |
| BRIGHTNESS | INT  | Number of milliseconds that the light is turned on to the COLD START LEVEL value. |


### Returns

`None`