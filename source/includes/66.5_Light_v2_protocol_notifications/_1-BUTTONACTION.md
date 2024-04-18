## BUTTON\_ACTION

Used to inform the proxy that a button state has changed on the device.  Note that the Proxy expects a Release if it gets a Push. If it does not receive a Release, subsequent Pushes will not work and state/tracking will be off. 

### Name

`BUTTON_ACTION ()`



| Parameter | Type | Description                                      |
| --------- | ---- | ------------------------------------------------ |
| BUTTON ID | INT  | BUTTON ID: Index of the button being controlled. |
| ACTIO     | INT  | The Event Type which include:                    |
|           |      | 0 - Release                                      |
|           |      | 1 - Push                                         |
|           |      | 2 - Single Tap                                   |
|           |      | 3 - Double Tap                                   |
|           |      | 4 - Triple Tap                                   |


### Returns

`None`