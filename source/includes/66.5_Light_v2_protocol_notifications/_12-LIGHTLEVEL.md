## LIGHT\_LEVEL

Used to inform the proxy that the light level has changed.


### Name

`LIGHT_LEVEL ()`



| Parameter | Type | Description                                    |
| --------- | ---- | ---------------------------------------------- |
| LEVEL     | INT  | Percent from 0-100 of the current light level. |


### Returns

`None`


### Usage Note

As of Operating System 3.3.0, drivers should no longer send incremental notifies of light level every 20ms, 500ms, 1000ms, etc, as the lights brightness ramps. Sending excessive incremental level updates caused performance issues including:

- Excessive slowness in Proxies, Director, and Navigators.
- Slow performance and inaccurate states for Advanced Lighting Scene tracking.
- Excessive Zigbee traffic and often incorrect keypad button LED status.
- Inconsistent slider movement in Navigators.
- Excessive triggering and sometimes incorrect Composer programming being fired.

See the [LIGHT\_BRIGHTNESS\_CHANGING][1] notification for additional information.

[1]:	https://snap-one.github.io/docs-driverworks-proxyprotocol/#light-v2-protocol-notifications-light_brightness_changing