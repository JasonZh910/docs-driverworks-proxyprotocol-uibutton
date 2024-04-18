## CHANNEL\_CHANGED

Selected channel has changed


### Name

`CHANNEL_CHANGED ()`


| Parameter       | Type | Description       |
| --------------- | ---- | ----------------- |
| ChannelNumnber  | INT  | Channel value     |
| OutputBindingID | INT  | Output Binding ID |



### Returns

`None`


### Usage Note

If the BANDTYPE is not supplied, as in older drivers, the INPUT binding # will be used to determine which band the tuner is on. All DriverWorks drivers need to use the BANDTYPE parameter if they want the band to propagate up to Navigator to display the channel properly. If the DriverWorks driver does not know the current channel and the “has feedback” capability is not set to “True”, none of this matters and everything will keep working as it previously has.

A `CHANNEL CHANGED` must be issued immediately after the `INPUT_CHANGED` in order for the UI to update.

### Example


```lua
C4:SendToproxy(5002,'INPUTCHANGED' {INPUT=3009,BANDTYPE='FMBand',MINCHANNEL=8750,MAXCHANNEL=10790,CHANNELSPACING=20})
    C4:SendToProxy(5002,'CHANNELCHANGED',CHANNEL=10290)
```


Note that in the example to the right, 5002 is the ProxyBindingID for the Tuner. INPUT 3009 is the ID for the FM Antenna on the 5002 Tuner.

Navigator determines AM/FM/XM with the following rule:

- ID 3000 and 3001 are AM
- ID 3002 and 3003 are FM