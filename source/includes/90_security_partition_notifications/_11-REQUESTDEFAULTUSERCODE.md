## REQUEST\_DEFAULT\_USER\_CODE\_

The proxy code stores the default user code if it exists for the partition.  When the proxy is first bound to the protocol driver, it will send that code to the protocol driver.  However, we found that when a driver is updated, that call was not being made, so we added a mechanism for the protocol driver to initiate the communication to get that code.  This is new in 3.2

#### Available from 3.2.0


### Parameters

`None`


### Example

```lua
C4:SendToProxy(TargetBindingID, "REQUEST_DEFAULT_USER_CODE", {}, "NOTIFY")
```
