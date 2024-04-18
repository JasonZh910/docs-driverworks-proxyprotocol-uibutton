## MIN\_ON

Used to inform the proxy that the hardware minimum On level has changed.  This is useful for hardware such as Control4’s Gen3 lighting where the hardware supports remapping where 1% brightness is when the light is on.  This does not change the available brightness percent range from 0-100%.  Note that with LED lights, the  usable minimum on range does change depending on bulb, age of bulb and other factors.  

### Name

`MIN_ON ()`



| Parameter | Type | Description                                                    |
| --------- | ---- | -------------------------------------------------------------- |
| int       | NUM  | Percent from 0-99 for the Min On brightness to be remapped to. |


### Returns

`None`