## SPEAKER\_VOLUME\_CHANGED

This notification is issued by the protocol when the endpoint’s Speaker Volume setting has changed. 


### Signature

`SPEAKER_VOLUME_CHANGED ()`


| Parameter | Description                                                                                   |
| --------- | --------------------------------------------------------------------------------------------- |
| int       | The proxy device id of the intercom endpoint whose device state information is being returned |
| num       | speakerVol: Numeric indicating the current state for this setting. (0=false, 1=true)          |


### Example

```lua
<device_state proxyid =[10]>
    <speakerVol>[0]</speakerVol>
</device_state>
```

